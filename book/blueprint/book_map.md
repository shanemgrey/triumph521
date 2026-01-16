# Book Map (Outline + Modules)

This is the high-level arc for the whole volume: Prologue (vignette) + Part I (17 chapters) + Part II (implementation modules; optional).

Rules:
- Each chapter/module must have a unique job.
- Details live in the per-chapter spec files in `book/blueprint/`.

## Prologue (Outside Part I)

Target length: ~1–2 pages.

| Item | Working title | Job (1 sentence) | New terms | Spec |
|---:|---|---|---|---|
| P | Prologue (vignette) | Show the destination first (effects-first), convey the scale of change, then hand off to Chapter 01 for diagnosis. | (none) | `book/blueprint/00_Prologue.md` |

## Part I — Conceptual Journey (17 chapters)

Target length: ~2,500 words/chapter (variance allowed).

| Ch | Working title | Job (1 sentence) | Key claims | New terms (if any) | Spec |
|---:|---|---|---|---|---|
| 01 | The Broken Reward Signal | Establish that the problem is structural (not moral) and set the “treat it like engineering” frame. | C-002 | rent (preview), exclusion (preview) | `book/blueprint/01_The_Broken_Reward_Signal.md` |
| 02 | The Three Inputs | Define nature/civilization/labor as the primitives needed to reason clearly. | C-001 | nature, civilization, labor | `book/blueprint/02_The_Three_Inputs.md` |
| 03 | The Commons (as Accounting) | Define the commons as a value category and surface the accounting error in modern ownership. | C-003 | commons | `book/blueprint/03_The_Commons_as_Accounting.md` |
| 04 | Property Is Exclusion | Make exclusion legible as the mechanism behind property without villain framing. | C-002, C-019 | exclusion (formal) | `book/blueprint/04_Property_Is_Exclusion.md` |
| 05 | Rent: Income from Exclusion | Define rent precisely and distinguish it from wages and profit using simple contrasts. | C-002, C-003 | rent (formal) | `book/blueprint/05_Rent_Income_from_Exclusion.md` |
| 06 | Why Politics Can’t Fix It | Show why moral/political fights recur under the current mechanics and why partial fixes fail. | C-013 | capture (informal) | `book/blueprint/06_Why_Politics_Cant_Fix_It.md` |
| 07 | The Inversion Principle | Introduce the core inversion: charge exclusion, not productive activity. | C-004 | LEF (preview) | `book/blueprint/07_The_Inversion_Principle.md` |
| 08 | Compensation: The Citizen Dividend | Establish the dividend as compensation for exclusion (not charity) and why it stabilizes legitimacy. | C-006, C-019 | citizen dividend | `book/blueprint/08_Compensation_The_Citizen_Dividend.md` |
| 09 | Funding Government: The People’s Budget | Introduce the People’s Budget and show how it reduces capture vs tax-funded discretion. | C-008 | people’s budget | `book/blueprint/09_Funding_Government_The_Peoples_Budget.md` |
| 10 | The Land Exclusion Fee (LEF) | Explain LEF at a conceptual level and the “near-zero transfer value” objective. | C-004, C-005, C-020 | LEF | `book/blueprint/10_The_Land_Exclusion_Fee_LEF.md` |
| 11 | Resource Rents | Extend the same logic to finite resources and preview why different commons need different fee structures. | C-010, C-015 | resource rent | `book/blueprint/11_Resource_Rents.md` |
| 12 | No Taxes on Productivity | Make the end state explicit: replace productive taxes with commons fees; place externality/risk fees inside the framework. | C-009, C-016, C-020 | productive activity | `book/blueprint/12_No_Taxes_on_Productivity.md` |
| 13 | Transition Without Chaos | Present the stable-state glide path (sequencing, bonds, constraints) without pretending it’s one-size-fits-all. | C-011 | transition bonds (preview) | `book/blueprint/13_Transition_Without_Chaos.md` |
| 14 | Greenfield Adoption | Describe how rebuilding states can adopt the architecture quickly under minimal institutional assumptions. | C-018 | greenfield adoption | `book/blueprint/14_Greenfield_Adoption.md` |
| 15 | Safeguards and Failure Modes | Define the failure modes (exemptions, tampering, diversion) and the non-negotiable safeguards. | C-013 | dividend-first rule | `book/blueprint/15_Safeguards_and_Failure_Modes.md` |
| 16 | Objections and Hostile Paraphrases | Preempt the most dangerous misreadings and answer them with mechanisms, not motives. | (supporting) | (none) | `book/blueprint/16_Objections_and_Hostile_Paraphrases.md` |
| 17 | Triumph of the Commons | Synthesize the arc, set the final impression, and include an “edge of AI” section as a design agenda. | C-014 | (none) | `book/blueprint/17_Triumph_of_the_Commons.md` |

## Part II — Implementation Modules (Optional; Read in Any Order)

Each module should be readable standalone. Each should include: Who this affects, prerequisites, inputs/data, mechanism summary, tunable parameters, failure modes, and “where it touches the contract”.

| Module | Topic | Job (1 sentence) | Key claims | Spec |
|---:|---|---|---|---|
| 18 | Fee Structure Theory | Provide a taxonomy for fee structures across commons categories (behavior + measurability constraints). | C-015 | `book/blueprint/18_Fee_Structure_Theory.md` |
| 19 | Hydrocarbons | Specify rent capture and pricing options for oil/gas/coal under the framework. | C-010, C-015 | `book/blueprint/19_Hydrocarbons.md` |
| 20 | Fresh Water | Specify fee structures for water extraction, rights, and commons protection. | C-015, C-016 | `book/blueprint/20_Fresh_Water.md` |
| 21 | Durable Materials | Specify fees for durable finite materials (metals/minerals) with attention to recycling and stock vs flow. | C-015 | `book/blueprint/21_Durable_Materials.md` |
| 22 | Atmosphere | Specify measurable externality fees (emissions/pollution) as commons usage. | C-016 | `book/blueprint/22_Atmosphere.md` |
| 23 | Oceans | Specify fee structures for fisheries, seabed extraction, shipping commons, and enforcement constraints. | C-015, C-016 | `book/blueprint/23_Oceans.md` |
| 24 | Radio Spectrum | Specify allocation and pricing mechanisms for spectrum as a scarce commons. | C-015 | `book/blueprint/24_Radio_Spectrum.md` |
| 25 | Sunlight | Specify scarce/locational sunlight capture cases (where applicable) and where it’s not worth metering. | C-015 | `book/blueprint/25_Sunlight.md` |
| 26 | Biodiversity | Specify biodiversity protection as commons value with measurable proxies and hard limits. | C-016 | `book/blueprint/26_Biodiversity.md` |
| 27 | Organic Materials | Specify rent/externality fees for biomass, forests, soils, and regenerative resources. | C-015, C-016 | `book/blueprint/27_Organic_Materials.md` |
| 28 | Land | Specify the LEF mechanism details (auction/valuation paths, adjustment caps, land availability buffer, failure modes). | C-004, C-005, C-018 | `book/blueprint/28_Land.md` |
| 30 | Indicators of Success | Provide a bounded indicator set for economic/social/ecological outcomes and explicit measurement humility. | (supporting) | `book/blueprint/30_Indicators_of_Success.md` |
| 31 | To Powerful People | Speak directly to incumbents: what they give up vs gain, and why cooperation beats forced transition. | (supporting) | `book/blueprint/31_To_Powerful_People.md` |
| 32 | Adoption Paths | Give concrete greenfield and glide-path procedures, assumptions, and failure modes. | C-011, C-018 | `book/blueprint/32_Adoption_Paths.md` |

## Global Constraints
- Do not redefine glossary terms; update `book/registry/glossary.md` via tickets.
- Any major claim introduced in prose must map to a claim ID in `book/registry/claim_ledger.md`.
- Avoid idioms/wordplay that won’t translate; keep key terms consistent across chapters and languages.
