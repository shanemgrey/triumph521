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

- ID: T-021
  Type: structure
  Severity: should
  Target: `book/blueprint/book_map.md` (Part I outline)
  Problem:
  - Part I currently reads as a flat list of 17 chapters; the reader journey would benefit from 4–6 conceptual “parts” that act as orientation markers and pacing breaks.
  - Part boundaries should be visible to the reader, but parts are grouping labels only (no chapter renumbering).
  Requested change:
  - Propose a 4–6 part breakdown for Part I (aim ~5 parts) where each part has:
    - a short working title,
    - a one-sentence job (what the reader gains in this segment),
    - the included chapter numbers.
  - Treat parts as **grouping labels only**: keep chapter numbers unchanged.
  - Use part boundaries to mark conceptual shifts (example: “see the problem” → “understand mechanisms” → “explore solution changes”).
  - After author approval, update `book/blueprint/book_map.md` to include part headers and group the chapters accordingly.
  - Keep Part II un-partitioned (no additional parts inside the modules section).
  - Coordinate with `T-022` (Part I / Part II boundary copy) so the part grouping supports the “closure then optional modules” feel.
  Acceptance criteria:
  - `book/blueprint/book_map.md` contains clear Part I part headers (title + job) and chapters are grouped under them.
  - Part boundaries support the existing chapter jobs/transitions (no new job overlap; no reordering unless separately approved).
  - Part II remains a flat module list (no parts added).
  - The author explicitly approves the part breakdown before it is applied to `book/blueprint/book_map.md`.

- ID: T-027
  Type: clarity
  Severity: should
  Target: `book/blueprint/12_No_Taxes_on_Productivity.md`
  Problem:
  - The book promises accelerated productive outcomes, but it lacks a simple, translation-friendly model for why taxing productive activity damages compounding over time (beyond “taxes distort incentives”).
  Requested change:
  - Add a required section in Chapter 12 that introduces the glossary model “Compounding productive capacity” and uses it to explain:
    - why taxes on productive activity reduce reinvestment into tools/skills/durable capital, and
    - why pricing exclusion/usage/damage does not penalize productive compounding the same way.
  - Use neutral, non-moral examples (e.g., tools/training/infrastructure vs a large diamond) and explicitly state the point is structural over time, not aesthetic judgment about consumption.
  Acceptance criteria:
  - Chapter 12 spec lists `C-021` in Key Claims and references the glossary term “Compounding productive capacity”.
  - Chapter 12 spec requires one short example of chain-extending spending and one short example of non-compounding spending (no numbers required). Default example for non-compounding: a large diamond.
  - Chapter 12 spec explicitly warns against moralized “luxury shaming” language.

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
- T-017 (2026-01-16): Documented prompt-prefix role invocation in `spec/system.md` and clarified `Advisor:` in `spec/roles/advisor.md`.
- T-020 (2026-01-16): Adopted `NN_Title_With_Underscores.md` naming for specs/drafts/packs (including Prologue `00_Prologue.md` and Part II modules 18+), and updated workflow docs.
- T-022 (2026-01-16): Standardized reader-facing structure as `Part I` + `Part II: Implementation Modules (Optional; Read in Any Order)` across contract/blueprint and Chapter 17 handoff requirements.
- T-015 (2026-01-16): Canceled (estate/inheritance module deferred post-publication).
- T-026 (2026-01-16): Canceled (estate/inheritance module excluded from this book; no framing work needed).
- T-009 (2026-01-16): Added a concrete low-data greenfield adoption procedure to Part II (`book/book_contract.md`, `book/blueprint/32_Adoption_Paths.md`).
- T-018 (2026-01-16): Rewrote the Prologue vignette as scene-first and mechanism-free (`book/blueprint/00_Prologue.md`).
- T-023 (2026-01-16): Required “today vs People’s Budget” control-loop framing + failure modes/mitigations in Chapter 09 spec (`book/blueprint/09_Funding_Government_The_Peoples_Budget.md`).
- T-024 (2026-01-16): Integrated the structural poverty thread (C-019) into Chapter 04/08 specs and the Part I map (`book/blueprint/04_Property_Is_Exclusion.md`, `book/blueprint/08_Compensation_The_Citizen_Dividend.md`, `book/blueprint/book_map.md`).
- T-025 (2026-01-16): Required an explicit tax-vs-commons-fee contrast (C-020) in Chapter 12 and reinforced the framing in Chapter 10 (`book/blueprint/12_No_Taxes_on_Productivity.md`, `book/blueprint/10_The_Land_Exclusion_Fee_LEF.md`).
- T-028 (2026-01-16): Removed the Estate Transfer module from the blueprint and deferred the spec (`book/blueprint/book_map.md`, `archive/estate_transfer_deferred.md`).
- T-016 (2026-01-16): Replaced the placeholder “Indicators of Success” module with a bounded indicator set + explicit exclusions (`book/blueprint/30_Indicators_of_Success.md`).
- T-019 (2026-01-16): Expanded the Chapter 04 spec’s required “frontier → enclosure → closure” stylized model (land-first, then resources) and strengthened the bridge into Chapter 05 (`book/blueprint/04_Property_Is_Exclusion.md`).
