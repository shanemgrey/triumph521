# Progress Log

This is the decision log and build history. Keep it short and factual.

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
