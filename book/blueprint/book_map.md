# Book Map (Outline + Modules)

This is the high-level arc for the whole volume: Part I (17 chapters) + Book Two (skippable modules).

Rules:
- Each chapter/module must have a unique job.
- Details live in the per-chapter spec files in `book/blueprint/`.

## Part I — Conceptual Journey (17 chapters)

Target length: ~2,500 words/chapter (variance allowed).

| Ch | Working title | Job (1 sentence) | Key claims | New terms (if any) | Spec |
|---:|---|---|---|---|---|
| 01 | The Broken Reward Signal | Establish that the problem is structural (not moral) and set the “treat it like engineering” frame. | C-002 | rent (preview), exclusion (preview) | `book/blueprint/chapter_01.md` |
| 02 | The Three Inputs | Define nature/civilization/labor as the primitives needed to reason clearly. | C-001 | nature, civilization, labor | `book/blueprint/chapter_02.md` |
| 03 | The Commons (as Accounting) | Define the commons as a value category and surface the accounting error in modern ownership. | C-003 | commons | `book/blueprint/chapter_03.md` |
| 04 | Property Is Exclusion | Make exclusion legible as the mechanism behind property without villain framing. | C-002 | exclusion (formal) | `book/blueprint/chapter_04.md` |
| 05 | Rent: Income from Exclusion | Define rent precisely and distinguish it from wages and profit using simple contrasts. | C-002, C-003 | rent (formal) | `book/blueprint/chapter_05.md` |
| 06 | Why Politics Can’t Fix It | Show why moral/political fights recur under the current mechanics and why partial fixes fail. | C-013 | capture (informal) | `book/blueprint/chapter_06.md` |
| 07 | The Inversion Principle | Introduce the core inversion: charge exclusion, not productive activity. | C-004 | LEF (preview) | `book/blueprint/chapter_07.md` |
| 08 | Compensation: The Citizen Dividend | Establish the dividend as compensation for exclusion (not charity) and why it stabilizes legitimacy. | C-006 | citizen dividend | `book/blueprint/chapter_08.md` |
| 09 | Funding Government: The People’s Budget | Introduce the People’s Budget and show how it reduces capture vs tax-funded discretion. | C-008 | people’s budget | `book/blueprint/chapter_09.md` |
| 10 | The Land Exclusion Fee (LEF) | Explain LEF at a conceptual level and the “near-zero transfer value” objective. | C-004, C-005 | LEF | `book/blueprint/chapter_10.md` |
| 11 | Resource Rents | Extend the same logic to finite resources and preview why different commons need different fee structures. | C-010, C-015 | resource rent | `book/blueprint/chapter_11.md` |
| 12 | No Taxes on Productivity | Make the end state explicit: replace productive taxes with commons fees; place externality/risk fees inside the framework. | C-009, C-016 | productive activity | `book/blueprint/chapter_12.md` |
| 13 | Transition Without Chaos | Present the stable-state glide path (sequencing, bonds, constraints) without pretending it’s one-size-fits-all. | C-011 | transition bonds (preview) | `book/blueprint/chapter_13.md` |
| 14 | Greenfield Adoption | Describe how rebuilding states can adopt the architecture quickly under minimal institutional assumptions. | C-018 | greenfield adoption | `book/blueprint/chapter_14.md` |
| 15 | Safeguards and Failure Modes | Define the failure modes (exemptions, tampering, diversion) and the non-negotiable safeguards. | C-013 | dividend-first rule | `book/blueprint/chapter_15.md` |
| 16 | Objections and Hostile Paraphrases | Preempt the most dangerous misreadings and answer them with mechanisms, not motives. | (supporting) | (none) | `book/blueprint/chapter_16.md` |
| 17 | Triumph of the Commons | Synthesize the arc, set the final impression, and include an “edge of AI” section as a design agenda. | C-014 | (none) | `book/blueprint/chapter_17.md` |

## Book Two — Implementation (Skippable Modules)

Each module should be readable standalone. Each should include: Who this affects, prerequisites, inputs/data, mechanism summary, tunable parameters, failure modes, and “where it touches the contract”.

| Module | Topic | Job (1 sentence) | Key claims | Spec |
|---:|---|---|---|---|
| 01 | Fee Structure Theory | Provide a taxonomy for fee structures across commons categories (behavior + measurability constraints). | C-015 | `book/blueprint/book_two_01_fee_structure_theory.md` |
| 02 | Hydrocarbons | Specify rent capture and pricing options for oil/gas/coal under the framework. | C-010, C-015 | `book/blueprint/book_two_02_hydrocarbons.md` |
| 03 | Fresh Water | Specify fee structures for water extraction, rights, and commons protection. | C-015, C-016 | `book/blueprint/book_two_03_fresh_water.md` |
| 04 | Durable Materials | Specify fees for durable finite materials (metals/minerals) with attention to recycling and stock vs flow. | C-015 | `book/blueprint/book_two_04_durable_materials.md` |
| 05 | Atmosphere | Specify measurable externality fees (emissions/pollution) as commons usage. | C-016 | `book/blueprint/book_two_05_atmosphere.md` |
| 06 | Oceans | Specify fee structures for fisheries, seabed extraction, shipping commons, and enforcement constraints. | C-015, C-016 | `book/blueprint/book_two_06_oceans.md` |
| 07 | Radio Spectrum | Specify allocation and pricing mechanisms for spectrum as a scarce commons. | C-015 | `book/blueprint/book_two_07_radio_spectrum.md` |
| 08 | Sunlight | Specify scarce/locational sunlight capture cases (where applicable) and where it’s not worth metering. | C-015 | `book/blueprint/book_two_08_sunlight.md` |
| 09 | Biodiversity | Specify biodiversity protection as commons value with measurable proxies and hard limits. | C-016 | `book/blueprint/book_two_09_biodiversity.md` |
| 10 | Organic Materials | Specify rent/externality fees for biomass, forests, soils, and regenerative resources. | C-015, C-016 | `book/blueprint/book_two_10_organic_materials.md` |
| 11 | Land | Specify the LEF mechanism details (auction/valuation paths, adjustment caps, land availability buffer, failure modes). | C-004, C-005, C-018 | `book/blueprint/book_two_11_land.md` |
| 12 | Estate Transfer (Name TBD) | Show how inheritance/estate recapture can fit the framework without taxing productive activity. | C-017 | `book/blueprint/book_two_12_estate_transfer.md` |
| 13 | Indicators of Success | Provide a bounded indicator set for economic/social/ecological outcomes and explicit measurement humility. | (supporting) | `book/blueprint/book_two_13_indicators.md` |
| 14 | To Powerful People | Speak directly to incumbents: what they give up vs gain, and why cooperation beats forced transition. | (supporting) | `book/blueprint/book_two_14_powerful_people.md` |
| 15 | Adoption Paths | Give concrete greenfield and glide-path procedures, assumptions, and failure modes. | C-011, C-018 | `book/blueprint/book_two_15_adoption_paths.md` |

## Global Constraints
- Do not redefine glossary terms; update `book/registry/glossary.md` via tickets.
- Any major claim introduced in prose must map to a claim ID in `book/registry/claim_ledger.md`.
- Avoid idioms/wordplay that won’t translate; keep key terms consistent across chapters and languages.
