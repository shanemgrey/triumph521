# Land–Resource Dividend System: Core Specification

## 0. Purpose

This document defines the **system architecture** underlying the proposed economic model. It is not persuasive prose. It is a functional description of how the system operates, what constraints it obeys, how value flows, and how transitions occur.

The goal is to establish a stable source of truth against which narrative chapters can later be written.

---

## 1. Core Premise

All economic value arises from the interaction of three necessary components:

1. **Nature** – land, location, minerals, energy, ecosystems; not created by humans.
2. **Civilization** – infrastructure, institutions, knowledge, networks; collectively produced.
3. **Labor** – human effort, skill, creativity; individually attributable.

Only **labor** can be ethically credited to individuals. Value derived from **nature** and **civilization** must be treated as collectively owned.

---

## 2. Core Design Principles

* **No taxation on productive activity** (labor, exchange, capital formation).
* **Full capture of unearned rents** from land and natural resources.
* **Equal distribution** of captured rents to citizens.
* **Democratic control over public spending**, not administrative control.
* **Algorithmic, auditable valuation**, not discretionary assessment.
* **Gradual, compensatory transition** from legacy systems.

---

## 3. Economic Primitives

### 3.1 Land

* Defined as *location-exclusive space*.
* Fixed in total supply.
* **Land value is never assessed subjectively.**
* Value is inferred algorithmically from:

  * Verified market sale prices of nearby properties
  * Mandatory, standardized improvement assessments at time of sale
  * The *residual difference* between sale price and improvement value
  * Local vacancy rates

**Key mechanism:**

* Neither a property’s sale price nor its improvement assessment is used directly for that parcel’s fee.
* Instead, the residual land value implied by sales is fed into a rolling regional model.
* This model nudges surrounding Land Use Fees (LUF) upward or downward.

**Anti-corruption feedback loop:**

* Overstated improvement assessments artificially suppress inferred land value.
* This lowers LUF, increases occupancy pressure, and triggers vacancy-rate correction.
* Vacancy correction pushes LUF back upward and flags systematic assessment bias.

This creates a self-correcting, auditable land valuation system without discretionary judgment.

---

## 4. Institutional Components

### 4.1 Land & Resource Authority (LRA)

A public entity with **monopoly–monopsony powers** over land and natural resource rents.

**Characteristics:**

* Sole collector of land-use fees and resource rents.
* No discretionary pricing authority.
* Operates strictly via transparent algorithms.
* Cannot self-fund; budgeted via the People’s Budget.
* Fully auditable.

### 4.2 Citizen Dividend Pool

* Receives 100% of land-use fees and resource rents.
* Distributed equally to all citizens at fixed intervals.

### 4.3 People’s Budget System

A two-layer democratic funding mechanism:

1. **Budget Size Vote**

   * Citizens vote periodically on total public spending as a percentage or absolute amount.
   * Rate of change capped per period (e.g. ±5–10%).

2. **Allocation Vote**

   * Each citizen allocates their proportional share of the public budget across agencies/programs.
   * Granularity determined democratically.

---

## 5. Value Capture Mechanisms

### 5.1 Land Use Fee (LUF)

* Recurring fee paid for exclusive use of land.
* Assessed independently of improvements.
* Calculated algorithmically using:

  * Local vacancy rates
  * Transaction prices of comparable land
  * Infrastructure proximity
  * Zoning/use patterns
  * Geographic productivity (for rural land)

**Target:**

* Drive *transfer value of land toward zero* while maintaining full utilization.

**Market Signal:**

* High vacancy → fee decreases.
* Overutilization → fee increases.

### 5.2 Resource Rent Capture

Natural resources are divided into **finite extractive resources** and **regenerative resources**, with different treatment.

#### 5.2.1 Finite Extractive Resources (oil, gas, minerals)

* LRA operates a **true monopoly–monopsony market mechanism** per resource.
* LRA sets the *sale price* to maximize total net rent (citizen dividend), not to reflect physical scarcity.
* The chosen price corresponds to the **unitary elasticity point**: where price × quantity is maximized.

**Demand-side:**

* Sale price determines quantity demanded.

**Supply-side:**

* LRA purchases exactly the required quantity.
* Extractors compete to supply via market bidding.
* LRA pays the **minimum price necessary** to obtain that quantity.
* Extractors unable to supply profitably exit the market.

**Key properties:**

* Pricing reflects revenue maximization, not marginal scarcity.
* Consumers face prices intentionally above extraction cost, reducing throughput while maximizing citizen dividend.
* All surplus flows to the Citizen Dividend.

**Implementation variants:**

* Continued private extraction under monopsony purchase.
* Full nationalization with extraction contracted via bids.

**Transition protection:**

* Existing extraction rights holders are compensated via time-limited bonds reflecting the delta between legacy market pricing and post-transition monopsony pricing.

#### 5.2.2 Regenerative Resources (timber, biomass, agriculture)

* Treated contextually based on regeneration mechanism.
* Cultivated resources on private land are treated as **produced goods**, not extracted rents.

**Soil quality treatment:**

* Soil quality is treated as a **privately maintained and tradable asset** embedded in land transfer value.
* The system avoids pricing soil quality into LUF in ways that could reward depletion via lower fees.

**Public/captive ecology cases:**

* Public lands or natural forests harvested under contract are treated as extractive and subject to monopsony control.

**Externalities and metered commons:**

* Where feasible and politically acceptable, separate metered fees may apply to directly measurable commons usage (e.g., water extraction) or explicitly legislated ecological externalities.

---

## 6. Distribution Mechanism

### 6.1 Citizen Dividend

* Equal per-capita payment to all citizens.
* Unconditional.
* Funded exclusively from land and resource rents.
* Paid prior to any public budgeting.

**Effect:**

* Converts rising resource prices into net citizen benefit.
* Eliminates poverty at sufficient maturity.

---

## 7. Tax Replacement

### 7.0 Sequencing and Glide Path

**Core rule:** rents fund the Citizen Dividend first; government funding is then sourced from citizens via the People’s Budget.

In established states with ongoing budgets, taxes cannot be eliminated instantly. The replacement sequence is:

1. **Start Citizen Dividend** (LUF/NRR → CD).
2. **Instantiate the People’s Budget** (legal/technical infrastructure for citizen budget votes and allocations).
3. **Shift government funding onto the People’s Budget over time** (a glide path).
4. **Reduce legacy taxes only as the People’s Budget replaces their revenue role**, until distortionary taxes reach zero.

### 7.1 Tax Reduction Targets

As the People’s Budget replaces legacy revenue streams:

* Income taxes reduced to zero.
* Payroll taxes eliminated.
* Sales/VAT abolished.
* Capital gains taxes eliminated.
* Improvement/property taxes eliminated.

**Expected effect:**

* Reducing distortionary taxes increases overall economic efficiency; this tends to raise captured land/resource rents such that the Citizen Dividend rises by **at least as much** as taxes are reduced (and potentially more), because People’s Budget transfers are low-friction compared to legacy tax collection.

### 7.2 Service & Usage Fees

Governments may levy **non-distortionary fees** for:

* Government-provided services (e.g. inspections, permits, certifications).
* Government-operated infrastructure where usage is discrete or optional.

These fees:

* Must be cost-linked, not revenue-maximizing.
* Exist only where services are not universally required.
* Do not substitute for general taxation.

### 7.3 Excise (Risk) Fees

Governments may impose excise fees on activities that impose **predictable social risk**, including:

* Alcohol
* Tobacco
* Firearms
* Other legalized drugs

These fees:

* Are algorithmically tied to observed social costs (healthcare, accidents, enforcement).
* Internalize risk without penalizing unrelated economic activity.

---

## 8. Banking & Credit Implications

* Land ceases to function as speculative collateral.
* Mortgages **shrink but do not disappear**.
* Housing loans increasingly reflect depreciating improvements rather than appreciating land.

**Expected shifts:**

* Lower loan-to-value ratios.
* Higher interest rates reflecting real depreciation risk.
* Credit reallocates toward:

  * Business expansion
  * Productivity improvements
  * Consumer credit

**Net Effects:**

* Reduced systemic leverage.
* Higher capital productivity.
* Lower probability of asset bubbles.

---

## 9. Transition Strategy

### 9.1 Dividend-First Rule

* **All Land Use Fees (LUF) and Natural Resource Rents (NRR) flow directly and immediately to the Citizen Dividend.**
* No rent revenue may be used to fund government prior to passing through the Citizen Dividend.
* This protects public trust and prevents political capture.

### 9.2 Phased Introduction Options

Possible democratic transition mechanisms include:

* **Opt-in transition:** property owners voluntarily accept LUF in exchange for government bonds.
* **Transaction-based transition: LUF applies at point of sale. Buyer receives a government bond equal to the *implied land value* (sale price minus assessed improvements), not the full purchase price.
* **Stepped conversion:** incremental replacement (e.g. 25% per year) from legacy property taxes to LUF.

Partial implementation must follow a clear glide path.

### 9.3 Land Value Compensation

* Landholders receive government bonds equal to eliminated speculative land value at transition.
* Bonds:

  * Tradable
  * May be interest-free or interest-bearing
  * Serviced exclusively from LUF revenue

### 9.4 Political Lock-In

* Because LUF funds the Citizen Dividend rather than government budgets, voters are disincentivized from repealing it to inflate property prices.

---

## 10. Governance Safeguards

* Full algorithm transparency.
* Public audit trails for every assessment.
* Independent watchdogs.
* Budgetary control via citizens, not administrators.

---

## 11. Boundary Conditions

### Works Best When:

* Land scarcity exists.
* Institutional trust can be built.
* Democratic participation is feasible.

### Degrades Gracefully When:

* Partial implementation
* Conservative transition speeds

### Fails When:

* Rent capture is weakened by exemptions.
* Algorithms are politically distorted.
* Dividend is severed from rent source.

---

## 12. End State

* Zero speculative land value.
* High utilization of land.
* No taxes on productive activity.
* Universal citizen income from shared wealth.
* Government structurally accountable to citizens.
