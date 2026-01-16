# Book Contract

This file is the canonical truth source for the book: thesis, audience, voice, and non-negotiables. If it isn’t here, it isn’t “real”.

## Working Title
- Title: Triumph of the Commons
- Subtitle: A Path to a Sustainable Future at the Edge of AI
- Positioning: a mechanics-first redesign of property, rents, and public finance that replaces taxes on productive activity with exclusion/usage fees on the commons.

## Thesis (1 sentence)
Charging for exclusion from the commons (land and natural resources), distributing the proceeds equally as a citizen dividend, and funding government through citizen-directed budgeting can preserve markets and private title while eliminating taxes on productive activity—and create a stable foundation for a future where human labor is less central.

## Promise to the Reader (1 paragraph)
You’ll get a legible model of where value comes from (nature, civilization, labor), why modern economies misattribute that value through exclusion-based income (rent), and how a concrete institutional design can convert land/resource scarcity from a private windfall into shared income—without abolishing private ownership, profit, or markets. The book is structured as Part I (a conceptual journey you can’t “unsee”) and Part II (optional implementation modules you can read in any order). It is written from lived experience in the US but designed to be usable both as a safe transition path in stable countries and as a “fresh start” architecture for states rebuilding governance.

## Audience
- Primary: cross-ideological readers who believe incentives matter more than intentions and want a non-moralized, mechanical explanation (libertarian, progressive, socialist, market reformer, institutional skeptic, systems thinker).
- Secondary: institutional designers and implementers evaluating feasibility (policy staff, economists, civic technologists), especially in contexts rebuilding governance.

Reader baseline beliefs (entering):
- Outcomes feel disconnected from effort/contribution.
- Political camps talk past each other; the fight is part of the failure.
- A real solution must be structural, not moral.

Rejection trigger (must be actively prevented):
- “This is an ideological project disguised as neutral analysis.”

Not for:
- readers seeking moral validation, villains, or partisan identity reinforcement
- readers who want academic-status signaling or activist rhetoric
- readers who want empirical debates before conceptual clarity
- readers who want jurisdiction-specific legal drafting in the core text

Language constraint:
- This book will be translated into many languages using AI translation.
- Complex language is acceptable when it increases precision, but avoid idioms, puns, culturally specific metaphors, and wordplay that won’t translate cleanly.
- Keep core terms consistent (prefer defined glossary terms over stylistic synonyms).

Full reader model: `book/reader_model.md`.

## Non-Goals / Exclusions
- This book will not be a partisan manifesto, moral indictment, or culture-war argument.
- This book will not propose abolishing markets, private ownership, or profit.
- This book will not be jurisdiction-specific legal drafting or software architecture.
- This book will not overload the core narrative with implementation mechanics (those go in Part II).
- This book will not rely on “proof by case study” for its core claims; the primary support is logic, incentives, and thought experiments.
- This book will not prescribe jurisdiction-specific parameter values as “the policy”; it defines rule-structures and highlights tunable parameters and failure modes.

## Tone & Voice Constraints
- Temperature: calm, precise, non-tribal.
- Avoid: ideology signaling, moralizing, jargon without definitions, “activist” framing.
- Default move: explain mechanisms → show implications → invite the reader to notice the pattern.
- Voice should feel: “explaining clearly because it matters, not because it wins points.”
- Terminology discipline:
  - Prefer: “Land Exclusion Fee (LEF)”, “resource rent”, “citizen dividend”, “people’s budget”.
  - Avoid as default labels: “tax”, “welfare/handout”, “nationalization” (unless explicitly discussing variants).
  - When contrast matters: treat taxes as compulsory payments not anchored to a specific price for exclusion/usage/damage; treat fees as prices for exclusion/usage/damage (a value exchange).

## Core System Names (for consistency)
- **Nature / Civilization / Labor**: the three necessary inputs to production.
- **Exclusion**: control of access (the ability to say “you cannot use this”).
- **Land Exclusion Fee (LEF)**: recurring charge for exclusive control of land (improvements excluded).
- **Land & Resource Authority (LRA)**: the public collector/pricer of land/resource rents, operating via auditable algorithms.
- **Citizen Dividend**: equal per-capita distribution of captured rents.
- **People’s Budget**: citizen-controlled public budget sizing + allocation.
- **Dividend-First Rule**: rent revenue must pass through the dividend before any public budgeting.
- **Transition bonds**: compensation mechanism for legacy land/resource rightsholders during conversion.

## Sustainability Definition (for this book)
“Sustainable” primarily means **ecological sustainability**: aligning incentives so prosperity does not require accelerating depletion, pollution, or irreversible damage to shared natural systems.

## Structure (Part I + Part II)

Length targets:
- Total: ~70,000–90,000 words.
- Part I: ~17 chapters; target ~2,500 words/chapter on average (variance allowed).
- Part II: implementation modules; optional and skippable; module lengths vary by topic.

Part I — Conceptual journey:
- Diagnose the structural distortion (rent via exclusion).
- Make the alternative feel inevitable: price exclusion, pay the dividend, fund government via citizens.
- Keep mechanisms legible; avoid “engineering manual” detail.

Part II — Implementation Modules (optional; read in any order):
- Written so readers can skip around by domain (land, oil/gas, minerals, spectrum, water, etc.).
- Each module should be readable standalone and include: “Who this affects”, prerequisites, inputs, mechanism summary, failure modes, and where it touches the contract/non-negotiables.
- Start with a “fee structure theory” module: why land is priced one way, hydrocarbons another, durable materials another (economic behavior + measurability constraints).
- Domain modules:
  - Hydrocarbons
  - Fresh water
  - Durable materials
  - Atmosphere
  - Oceans
  - Radio spectrum
  - Sunlight
  - Biodiversity
  - Organic materials
  - Land
- Framework modules:
  - Indicators of economic, social, and environmental success (what to measure, what not to pretend to measure)
  - A direct chapter addressed to “powerful people” about transition incentives, stability, and why cooperation beats forced redistribution
- Adoption paths:
  - Greenfield adoption (fresh start) vs transition in stable states (glide path, compensation, safeguards).

## Non-Negotiable End State
- No taxes on productive activity (labor, exchange, investment, capital formation).
- Mandatory exclusion/usage fees on non-produced inputs (location/land, natural resources).
- Allowed fee categories (must not become backdoor productive taxes):
  - Cost-linked usage/service fees for commons infrastructure where practical (e.g., toll bridges, rail, power/communication lines).
  - Externality fees where commons usage/damage is measurable (pollution, extraction, depletion).
  - Risk fees tied to predictable, measurable social costs (e.g., alcohol harms, driving accidents, smoking-related care).

## Legitimacy Frame (Property + Compensation)
- Private title and exclusive use are preserved as enforceable rights.
- Exclusive control is treated as exclusion from the commons, and exclusion must be compensated at a recurring market rate (the land fee is the price of exclusion, not a tax on work).
- If no one pays the fee, exclusive control lapses and the land returns to commons availability until someone does.

## People’s Budget (Cadence + UX + Privacy)
- Intent: restructure the public-finance control loop so budget size and allocation are citizen-set on a predictable cadence and agency funding becomes downstream of those signals.
- Budget Size Vote: annual.
- Allocation Vote: allow quarterly changes so people can respond to perceived agency performance.
- UX intent: a hierarchical view of agencies/programs with drill-down detail; mobile-first.
- Rate-of-change cap: treat as a tunable governance parameter (example starting cap: ±10% per year to avoid shocks).
- Transparency and privacy: public totals should be auditable; allocation privacy is a design choice for the polity (privacy-preserving cryptography may be used; blockchain is optional and must not add friction).

## AI / Robotics Boundary (Explicitly Addressed)
As machine intelligence and robotics reduce the role of human labor, capturing only land/resource rents may be insufficient: value creation could concentrate in the hands of those who own/operate the machines.

The book will:
- treat this as a real risk and an open design space (not a solved claim)
- propose directions (e.g., stronger anti-monopoly powers, new commons definitions for critical AI infrastructure/capital, governance constraints on concentration)
- frame the core system as necessary groundwork for a “future without work”, not the final word
- include this as a section in the final chapter of Part I (alongside the overall synthesis), not as a standalone “AI chapter”

## Greenfield Adoption (Minimum Assumptions)
For a “fresh start” polity, assume:
- citizen ID
- payments rails
- courts/enforcement
- land registry

Minimal viable greenfield procedure (low-data path):
1. Establish the ordering rule: commons revenue routes to an equal per-capita dividend first, and only then to budgeting.
2. Allocate land rights via competitive auctions for annual payments (strong security of exclusive use; no discretionary parcel-by-parcel assessment).
3. Put an explicit annual adjustment rule in the land-rights contracts (default change-cap anchor: CPI + 10%) so fees can move toward the “near-zero transfer value” objective without shocks.
4. Use simple public pricing signals (not sales-data-heavy inference):
   - Availability buffer: some land must remain available at the posted algorithmic fee with no buyer at any given time.
   - Too low: meaningful buyer→seller transfer value reappears.
   - Too high: too much land sits unused, or improved parcels trade below improvement value.
5. Start resource rent capture with simple, auditable rules (auctioned rights and/or published schedule fees for exclusion/extraction) and expand sophistication only as capacity grows.
6. Pay the dividend on a predictable cadence; treat cadence/implementation details as tunable parameters (but the ordering is not).
7. Introduce a minimal People’s Budget loop (annual size vote + coarse allocation), then increase granularity over time.

Assumptions and failure modes must be explicit:
- If enforcement is weak or exemptions proliferate, rent capture collapses.
- If the dividend can be diverted or delayed, political capture returns immediately.
- If fee-setting becomes discretionary or opaque, legitimacy and auditability fail.

## Hostile Paraphrase Test
- Likely hostile paraphrase: “This is just socialism/UBI dressed up as a land grab—an anti-property tax that crashes housing and politicizes the economy.”
- Short rebuttal (mechanism-based, not motive-based): “It prices exclusion rather than taxing work: land and resource rents are treated as socially generated value, collected transparently, and returned equally. Private ownership and markets remain; what changes is that exclusive control carries a recurring price, with a compensatory transition path and a dividend-first safeguard that reduces political capture.”

## Success Criteria (Measurable)
- A journalist can summarize it accurately in 90 seconds.
- A skeptical expert can argue the mechanisms (not dismiss motives).
- Each chapter is compressible to 5 bullets without losing the point.
- The core idea survives hostile paraphrase without requiring moral appeals.

## Evidence Policy (Nonfiction Safety)
- No invented citations. If a source isn’t known yet, write `SOURCE NEEDED` and add a ticket.
- Claims with evidence requirements must appear in `book/registry/claim_ledger.md`.
- Separate “definition/architecture” statements from “empirical/predictive” claims; the latter need real evidence.
- Default posture: prefer argument-by-mechanism and thought experiments; avoid “proof by case study”. If real-world references appear, they are used sparingly and mainly to illustrate failure modes of current systems (not “proof that the proposal works”).

## Dividend Eligibility (Policy Intent)
- Default: citizens only (to reduce uncontrolled migration incentives).
- “Citizen” definition is a polity choice; the book will name the tradeoff and avoid pretending there is a universal rule.

## Citizen Dividend (Cadence + Minors)
- Cadence: a tunable policy parameter (e.g., monthly or quarterly), but must be on a predictable schedule and always paid before any People’s Budget funding.
- Minors: a tunable policy parameter; Part II should outline options (e.g., full share held in trust/guardian, partial share, or other rule) and the incentive/fraud risks of each, without pretending there is a universal default.

## Change Control
- Contract edits after blueprint freeze require a ticket in `book/tickets.md` and a decision note in `book/progress_log.md`.
