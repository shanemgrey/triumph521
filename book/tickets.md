# Tickets

Tickets are how reviewers influence the manuscript. Reviewers do not edit prose directly; they file tickets with acceptance criteria.

## Ticket Template

```
ID: T-___
Type: drift | clarity | evidence | tone | redundancy | bridge | structure
Severity: must | should | nice
Target: path/to/file.md#section

Problem:
- ...

Requested change:
- ...

Acceptance criteria:
- ...
```

## Open Tickets

- ID: T-009
  Type: structure
  Severity: must
  Target: `book/book_contract.md` (Scope) + Book Two mechanisms
  Problem:
  - “Greenfield adoption” needs a concrete low-data pathway; the sales-residual valuation approach assumes strong registries and market sales data.
  Requested change:
  - In Book Two, define the minimal viable greenfield path (auctioned land rights with annual LEF, CPI+10% adjustment cap, land-availability buffer signal, resource rent capture, dividend distribution, safeguards) and state its assumptions/failure modes.
  Acceptance criteria:
  - Book Two includes a clear greenfield procedure and states its assumptions/failure modes.

- ID: T-015
  Type: tone
  Severity: should
  Target: Book Two module: “Estate recapture”
  Problem:
  - The estate/inheritance mechanism needs a name that fits the framework without triggering “tax” framing before the logic is established.
  Requested change:
  - Choose a public-facing name (and a second-choice synonym) and add it to the glossary.
  Acceptance criteria:
  - Glossary and Book Two module use the chosen name consistently.

- ID: T-016
  Type: structure
  Severity: should
  Target: Book Two module: “Indicators of success”
  Problem:
  - “Indicators of economic/social/environmental success” needs a crisp scope so it doesn’t become a generic metrics chapter.
  Requested change:
  - Define which indicators are in-scope and which are explicitly out-of-scope (especially to avoid claiming more measurability than exists).
  Acceptance criteria:
  - Book Two indicators module has a bounded list + explicit exclusions.

## Closed Tickets

- T-001 (2026-01-15): Title/subtitle/positioning added to `book/book_contract.md`.
- T-002 (2026-01-15): Target reader definition incorporated into `book/book_contract.md` (plus language constraint).
- T-003 (2026-01-15): Scope clarified (US lens, globally applicable; Part I/Book Two structure; greenfield vs glide path).
- T-004 (2026-01-15): Land fee label finalized as `LEF` and applied in `book/book_contract.md` and `book/registry/glossary.md`.
- T-005 (2026-01-15): Replaced “evidence anchor” requirement with logic-first posture; claim ledger updated to `ARGUED`/`OPEN`.
- T-006 (2026-01-15): Ethical framing set to compensation-for-exclusion (commons accounting).
- T-007 (2026-01-15): Dividend eligibility set to citizens-only default; defined “Citizen” in glossary/contract.
- T-008 (2026-01-15): Resource mechanism depth set to Book Two, with limited Part I intuition as needed.
- T-010 (2026-01-15): “Sustainable” defined as ecological sustainability in `book/book_contract.md`.
- T-012 (2026-01-15): Allowed fee categories clarified in `book/book_contract.md` (usage/service, externality, risk).
- T-011 (2026-01-15): AI section scope/placement clarified (Part I final chapter section); AI risk tracked as `OPEN` in `book/registry/claim_ledger.md`.
- T-013 (2026-01-15): Dividend cadence and minors handling set as tunable policy parameters (cadence examples given; options deferred to Book Two).
- T-014 (2026-01-15): Book Two module specs drafted in `book/blueprint/` and listed in `book/blueprint/book_map.md`.
