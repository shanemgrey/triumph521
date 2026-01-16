# Inspectable Book Compiler v2 (System + Workflow)

This is a **systemized workflow for writing one nonfiction book** using multiple specialized agents. The goal isn’t “clever prompting”; it’s **inspectability**: every agent action produces artifacts you can review, and agents are constrained by explicit contracts.

Treat the book like software:
- **Specs** (contracts, blueprints, registries) define the system.
- **Build loop** drafts one chapter at a time from a compiled “packet”.
- **Quality gates** are checklists + tickets with acceptance criteria.

---

## 1) Design Goals (What Makes This Trustworthy)

1. **Role boundaries are enforceable**
   - Each role has allowed edits and forbidden edits.
   - Review roles never edit prose; they only file tickets.

2. **Stateless drafting**
   - Chapter Writer instances don’t “remember the book”.
   - They draft only from a chapter packet compiled by the Librarian.

3. **Traceability (especially for nonfiction)**
   - Major claims are tracked in a claim ledger.
   - Evidence status is explicit (`SUPPORTED`, `SOURCE NEEDED`, `REMOVE`).

4. **Change control**
   - The book contract and chapter blueprints have freeze points.
   - Changes happen via tickets + a decision log entry.

---

## 2) Repository Layout (Single Book, Systemized)

Suggested layout for this repo:

```text
spec/                       # this workflow + reusable role prompts
book/                       # the one book project (artifacts + drafts)
  book_contract.md
  blueprint/
    book_map.md
    chapter_template.md
    00_Prologue.md
    01_The_Broken_Reward_Signal.md
  registry/
    glossary.md
    claim_ledger.md
  continuity/
    continuity_ledger.md
  chapters/
    01_The_Broken_Reward_Signal.md
  packs/                    # compiled packets for stateless writers/reviewers
    01_The_Broken_Reward_Signal_pack.md
  project_status.md         # current snapshot (where we are + next actions)
  tickets.md
  progress_log.md
  interviews/               # optional: raw interview notes/transcripts
```

In this repository, `spec/role.md` is a usable baseline for the writing voice/persona; treat `book/book_contract.md` as the canonical “truth source”.

---

## 3) Canonical Artifacts (What Must Exist)

### A. `book/book_contract.md` (the “constitution”)
Contains: thesis, promise, audience, non-goals, tone/voice, exclusions, hostile-paraphrase test, measurable success criteria.

Freeze point: once approved, edits require a ticket + `book/progress_log.md` entry.

### B. `book/blueprint/book_map.md` (the arc)
Chapter list with entry/exit state, chapter job, dependencies, transitions, and “what not to do”.

### C. `book/blueprint/NN_Title_With_Underscores.md` (spec file)
For each Prologue/chapter/module: purpose, reader entry/exit, key claims, required evidence, terms to introduce/reuse, examples, constraints, and the target 5-bullet summary.

### D. `book/registry/glossary.md` (definitions)
Canonical terms + allowed synonyms + forbidden synonyms/metaphors + first-introduced-in.

### E. `book/registry/claim_ledger.md` (claims → evidence → chapters)
Each major claim gets an ID and:
- statement
- support type required
- evidence status (no invented citations)
- where it appears (chapter mapping)

### F. `book/continuity/continuity_ledger.md` (what’s already covered)
Per-chapter: 5-bullet summary, introduced terms, resolved/created open loops, and “do not repeat” notes.

### G. `book/tickets.md` (the only cross-role control surface)
All review feedback and change requests live here with acceptance criteria.

### H. `book/packs/NN_Title_With_Underscores_pack.md` (compiled context)
The Librarian compiles this packet. The Chapter Writer drafts using **only** this.

---

## 4) Role Contracts (Inputs, Outputs, Allowed Edits)

### Role Invocation (Prompt Prefixes)
To invoke a specific role contract, start your prompt with the role prefix (example: `Advisor:`). The agent must follow that role’s allowed edits and constraints.

### 0) Advisor / Development Editor (Optional)
Goal: help the author resolve open questions and improve mass-market readability **without** violating the contract.

- Inputs: `book/book_contract.md`, `book/reader_model.md`, `book/blueprint/book_map.md`, `book/tickets.md`, `book/progress_log.md`.
- Outputs: tickets (and decision notes once the author confirms choices).
- Must not: draft chapter prose or directly edit the contract/blueprint; influence happens through tickets.

### 1) Interviewer / Spec Builder
Goal: extract the book from the author via structured questions.

- Inputs: author interviews/notes, prior materials (optional).
- Outputs: `book/book_contract.md` v1, initial `glossary.md`, initial `claim_ledger.md`.
- May edit: contract + registries (early only).
- Must not: outline chapters or write chapter prose.

### 2) Architect / Blueprint Compiler
Goal: design the persuasion path and chapter jobs.

- Inputs: `book/book_contract.md`, registries, interview notes.
- Outputs: `book/blueprint/book_map.md`, spec files in `book/blueprint/`.
- May edit: blueprint files.
- Must not: draft chapter prose or redefine glossary terms (file a ticket instead).

### 3) Continuity Librarian / Packet Compiler
Goal: keep the project coherent and compile “safe context” for stateless writers.

- Inputs: latest locked artifacts, latest chapter drafts, tickets.
- Outputs: updates to `continuity_ledger.md`, registry updates, compiled `packs/NN_Title_With_Underscores_pack.md`.
- May edit: continuity + registries + packs.
- Must not: change chapter jobs or the book contract (tickets only).

### 4) Chapter Writer (Stateless Instance)
Goal: draft one chapter that satisfies its chapter spec.

- Inputs: `book/packs/NN_Title_With_Underscores_pack.md` only.
- Outputs: `book/chapters/NN_Title_With_Underscores.md` + a self-audit section at the end.
- Must not: edit blueprint/registry/continuity directly (tickets only).

Self-audit must include:
- 5-bullet summary
- new terms introduced (if any)
- claim checklist (which claim IDs were used)
- “SOURCE NEEDED” callouts (if evidence is missing)

### 5) QA Panel (Tickets Only)
This is three separate review lenses. They may be separate agents or sequential runs.

- Drift Auditor: checks adherence to `book_contract.md` + chapter spec constraints.
- Reader Simulator: checks comprehension, pacing, objections, persuasion path.
- Line Editor: checks clarity, voice, compression, redundancy.

Output: tickets in `book/tickets.md` only.

### 6) Reviser (Applies Accepted Tickets)
Goal: implement tickets without “helpfully changing the book”.

- Inputs: chapter draft + accepted tickets + current pack.
- Outputs: revised chapter draft; closes tickets with evidence.
- Must not: expand scope beyond ticket acceptance criteria.

---

## 5) The Workflow (Phases + Gates)

### Phase A — Intake → Contract Lock
1. Interviewer produces `book_contract.md` v1 + seed registries.
2. Human author reviews and edits contract until it’s correct.

Gate: the book can be explained from `book_contract.md` alone.

### Phase B — Blueprint → Blueprint Freeze
1. Architect produces `book_map.md` and chapter specs.
2. Reader Simulator reviews the blueprint (tickets only).
3. Human approves blueprint freeze (changes after this are ticketed).

Gate: every chapter has a unique job; the arc matches the contract.

### Phase C — Chapter Loop (repeat per chapter)
1. Librarian compiles `NN_Title_With_Underscores_pack.md`.
2. Chapter Writer drafts `chapters/NN_Title_With_Underscores.md` + self-audit.
3. QA Panel files tickets.
4. Reviser applies accepted tickets.
5. Librarian updates continuity + registries + claim ledger mappings.

Gate: chapter passes its spec, has a valid 5-bullet summary, and doesn’t introduce undefined jargon.

### Phase D — Integration Audit (every 3–5 chapters)
Run a structural drift pass across recent chapters:
- repetition
- missing bridges
- concept order violations
- voice drift

Output: tickets only.

### Phase E — Manuscript Lock (later)
When all chapters are “locked”, run final passes (compression, clarity, evidence tightening). Packaging/press-kit work is optional and intentionally out of scope for now.

---

## 6) Chapter Packet Spec (What the Writer Receives)

Each `book/packs/NN_Title_With_Underscores_pack.md` should include:
- Contract excerpt: thesis, audience, tone, “do not do” list.
- Chapter spec: job, entry/exit state, constraints, transitions.
- Required claim IDs + evidence status from `claim_ledger.md`.
- Relevant glossary subset (terms allowed in this chapter).
- Continuity summary: last 1–3 chapter 5-bullet summaries + “already covered” list.
- Open tickets that constrain this chapter.
- Output checklist (self-audit format).

The point: the writer cannot “drift” because they never see ambiguous or irrelevant context.

---

## 7) Ticket System (How Change Happens)

Ticket fields (recommended):
- `ID` (e.g., `T-014`)
- `Type` (`drift`, `clarity`, `evidence`, `tone`, `redundancy`, `bridge`, `structure`)
- `Target` (file + section)
- `Problem`
- `Requested change`
- `Acceptance criteria` (explicit)
- `Severity` (`must`, `should`, `nice`)

Rule: if a change isn’t ticketed, it didn’t happen.
