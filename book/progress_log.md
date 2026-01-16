# Progress Log

This is the decision log and build history. Keep it short and factual.
Current snapshot: `book/project_status.md`.

## Milestones
- [x] Contract drafted
- [ ] Contract locked
- [x] Blueprint drafted
- [ ] Blueprint frozen
- [ ] Chapter loop started
- [ ] Manuscript locked

## Decisions

### 2026-01-15 — Seeded initial contract from `archive/`
- Decision: Use the “Land–Resource Dividend + People’s Budget” system as the baseline book proposal.
- Rationale: `archive/onepage.md` provides the reader-facing framing; `archive/core_spec.md` and `archive/mechanisms.md` provide implementable mechanics.
- Impacted artifacts: `book/book_contract.md`, `book/registry/glossary.md`, `book/registry/claim_ledger.md`.

### 2026-01-15 — Open questions tracked as tickets
- Decision: Track unresolved interview items as tickets rather than inline TODO prose.
- Rationale: Keeps the contract readable and creates an explicit queue for follow-up.
- Impacted artifacts: `book/tickets.md`.

### 2026-01-15 — Interview round 1 (title, reader, scope, non-negotiables)
- Decision: Working title set to “Triumph of the Commons” with subtitle “A Path to a Sustainable Future at the Edge of AI”.
- Decision: Target reader defined as cross-ideological and mechanics-first; avoid identity-threat and moralized rhetoric; assume many readers have English as a second language.
- Decision: Book structure set as two parts in one volume (Part I conceptual journey; Book Two implementation modules).
- Decision: Book Two is skippable and modular by domain; chapters must be readable standalone for readers who only care about specific mechanisms.
- Decision: Scope stance set to “US experience lens, universally applicable” with both a greenfield path (rebuilding states) and a glide-path transition (stable states).
- Decision: Non-negotiable end state set to “no taxes on productive activity”; finance via exclusion/usage fees on the commons + citizen dividend + people’s budget.
- Decision: Evidence posture set to logic/thought-experiment first; real-world references are optional and used sparingly (not as “proof it works”).
- Decision: AI-era risk explicitly included as an end-of-book design agenda (acknowledged as open).
- Impacted artifacts: `book/book_contract.md`, `book/registry/glossary.md`, `book/registry/claim_ledger.md`, `book/tickets.md`.

### 2026-01-15 — Interview round 2 (Book Two modules, greenfield, governance)
- Decision: Land fee label finalized as **Land Exclusion Fee (LEF)**.
- Decision: Book Two module list set (fee-structure theory; domain modules: hydrocarbons, fresh water, durable materials, atmosphere, oceans, radio spectrum, sunlight, biodiversity, organic materials, land; plus estate-recapture, indicators, and optional “powerful people” chapter).
- Decision: Greenfield minimum assumptions set: citizen ID, payments rails, courts/enforcement, land registry; land rights begin as competitive auctions for annual LEF payments with algorithmic annual adjustment rules aimed at keeping land transfer value near zero.
- Decision: People’s Budget cadence set: annual budget size vote; quarterly allocation updates; UX is hierarchical/drill-down; allocation privacy is desired (privacy-preserving cryptography allowed; blockchain optional).
- Decision: “Sustainable” in the subtitle is defined primarily as **ecological** sustainability.
- Decision: Allowed fee categories expanded to include measurable **externality** fees and **risk** fees (in addition to usage/service fees), with the constraint that they cannot become backdoor taxes on productive activity.
- Impacted artifacts: `book/book_contract.md`, `book/registry/glossary.md`, `book/registry/claim_ledger.md`, `book/tickets.md`.

### 2026-01-15 — Interview round 3 (Book Two reading model, caps, placement)
- Decision: `LEF` confirmed as the final land fee label (not `LHF`/`LUF`).
- Decision: Book Two is explicitly skippable and designed for “jump to your domain” reading (farmers → land; coal/oil workers → resource modules; etc.).
- Decision: Greenfield LEF adjustment cap default set to CPI + 10% and the “land availability buffer” is adopted as a price signal to keep transfer value near zero.
- Decision: People’s Budget may include a rate-of-change cap (example starting cap ±10% per year), but the cap is treated as a tunable parameter decided by the polity; allocation privacy is optional (a design choice, not a requirement).
- Decision: AI risk appears as a section within the final chapter of Part I (not a standalone chapter); the “powerful people” chapter is included in Book Two as practical transition politics.
- Decision: Dividend cadence and minors handling are treated as tunable policy parameters; Book Two will present options and incentive tradeoffs rather than prescribing a universal rule.
- Impacted artifacts: `book/book_contract.md`, `book/registry/glossary.md`, `book/registry/claim_ledger.md`, `book/tickets.md`.

### 2026-01-15 — Architect: Chapter map + specs drafted
- Decision: Part I set to 17 chapters with distinct jobs and ~2,500 words/chapter target (variance allowed) toward a 70–90k total manuscript target.
- Decision: Book Two structured as skippable, domain-targeted modules with standalone readability requirements.
- Impacted artifacts: `book/blueprint/book_map.md` and chapter/module specs in `book/blueprint/`.

### 2026-01-16 — Opener strategy: prologue vignette + effects-first framing
- Decision: Add an unnumbered Prologue vignette (outside the 17 chapters) that hands off to Chapter 01 for diagnosis.
- Decision: The opener is effects-first: do not name `LEF`, the dividend, or the People’s Budget in the Prologue; terms arrive later in the arc.
- Decision: Any frontier/enclosure material is explicitly framed as a stylized model/pattern (not a literal or geographically specific history claim).
- Impacted artifacts: `book/blueprint/book_map.md`, `book/blueprint/00_Prologue.md`, `book/blueprint/01_The_Broken_Reward_Signal.md`, `book/blueprint/04_Property_Is_Exclusion.md`.

### 2026-01-16 — Process: treat prior edits as Architect; Advisor is tickets-only
- Decision: Treat the Prologue/opener changes applied directly in `book/blueprint/` as an Architect action (not an Advisor ticket pass).
- Decision: When a prompt begins with `Advisor:`, follow `spec/roles/advisor.md` and influence changes via `book/tickets.md` (no direct edits to contract/blueprint).
- Impacted artifacts: `book/tickets.md` (process ticket `T-017`).

### 2026-01-16 — Prologue + model integration parameters (author answers)
- Decision: Prologue vignette should foreground **work/leisure** as the primary “felt difference”, with **ecology** as a secondary implication.
- Decision: Prologue vignette viewpoint anchor: mid-skill “white collar” worker doing creative work on a flexible schedule.
- Decision: Prologue vignette setting: dense green city (fresh air, high rises, park-like multi-level walkways, clean transit, convenient personal mobility).
- Decision: Frontier/enclosure section should explain **land scarcity first**, then extend to resources as a parallel case.
- Decision: Prologue voice is delegated to the drafting pass, constrained to be scene-first and trust-preserving (no mechanism explanation; no named system components).
- Decision (superseded): Preferred chapter artifact naming scheme: `Book_Part_Chapter_Title.md` (example: `1_1_12_No_Taxes_on_Productivity.md`).
- Impacted artifacts: `book/tickets.md` (`T-018`, `T-019`, `T-020`).

### 2026-01-16 — Part I part labels (author answers)
- Decision: Book One is the Part I arc (~17 chapters) and should be grouped into ~5 conceptual parts as orientation markers (no chapter renumbering).
- Decision: Part labels should reflect conceptual shifts: “see the problem” → “understand mechanisms” → “explore the changes that solve it” (and subsequent shifts as needed).
- Decision: Part II is implementation modules and should not be split into parts.
- Impacted artifacts: `book/tickets.md` (`T-021`, `T-020`).

### 2026-01-16 — Reader-facing structure + filenames (author answers)
- Decision: Use reader-facing labels: `Part I` (main journey; read in order; complete argument) and `Part II: Implementation Modules (Optional; Read in Any Order)`.
- Decision: File naming convention: `NN_Title_With_Underscores.md` (example: `04_Property_Is_Exclusion.md`).
- Decision: Part II modules should not restart numbering; continue numbering after Chapter 17 for consistent ordering.
- Decision: Part II content is labeled “Implementation Modules” in reader-facing headings/TOC (avoid “Chapter 18” language even if filenames use numeric prefixes).
- Impacted artifacts: `book/tickets.md` (`T-020`, `T-022`).

### 2026-01-16 — Added core framing requirements (People’s Budget, poverty, tax vs fee)
- Decision: The People’s Budget must be framed as a citizen-controlled control loop (budget authority downstream of citizen choices on a predictable cadence), not as “we vote sometimes”; show how this reduces capture without promising capture-proof governance.
- Decision: Poverty should be treated as an emergent condition of enforceable exclusion from the commons; define “poverty” as a cross-cultural material-insecurity concept before first use (avoid income-below-$X thresholds unless explicitly labeled as local examples).
- Decision: The book must draw a crisp conceptual distinction between taxes (compulsory payments set by budget decisions) and commons fees (prices for exclusion/usage/damage) to prevent “this is just another tax” misreads.
- Impacted artifacts: `book/book_contract.md`, `book/registry/glossary.md`, `book/registry/claim_ledger.md`, `book/tickets.md` (`T-023`–`T-025`).

### 2026-01-16 — Deferred inheritance / estate transfer topic
- Decision: Exclude inheritance/estate-transfer mechanisms from this book to preserve reader trust and avoid political distraction; revisit post-publication if the core book succeeds.
- Impacted artifacts: `book/registry/claim_ledger.md` (`C-017` marked `REMOVE`), `book/registry/glossary.md` (removed estate term), `book/tickets.md` (`T-028`; `T-015`, `T-026` closed).

### 2026-01-16 — Added “compounding productive capacity” model for productivity framing
- Decision: Use a time-based model of growth (income reinvested into tools/skills/durable capital compounding future productivity) to support the “no taxes on productive activity” argument.
- Impacted artifacts: `book/registry/glossary.md` (new term), `book/registry/claim_ledger.md` (`C-021`), `book/tickets.md` (`T-027`).
