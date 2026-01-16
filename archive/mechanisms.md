# Mechanisms Appendix: Valuation, Pricing, and Transition

This appendix documents **operational mechanisms** referenced in the Core Specification. It is intentionally technical. Its purpose is to make the system *implementable*, auditable, and falsifiable without turning the main text into an engineering manual.

---

## A. Land Valuation Mechanism (Algorithmic, Non‑Discretionary)

### A.1 Data Inputs

Land Use Fees (LUF) are derived from **regional inference**, not parcel-level judgment. Inputs include:

1. **Verified Market Sales**

   * Arm’s-length transactions only
   * Time‑stamped and geocoded
   * Excludes distressed or non-market transfers

2. **Sale-Time Improvement Valuation (Land-Excluded)**

   * Conducted at time of sale
   * Purpose: estimate what a rational buyer would pay **assuming zero land value**
   * Valuation method may vary by property type (income-based, use-value, improvement-only comparables, etc.)
   * Explicitly excludes any location or land premium

3. **Residual Land Value Inference**

   * Residual = Sale Price − Assessed Improvements
   * Residuals are never applied to the transacting parcel

4. **Vacancy & Utilization Rates**

   * Zoning‑consistent vacancy
   * Under‑utilization signals

---

### A.2 Regional Model

* Land is partitioned into overlapping valuation regions.
* Residuals feed into a rolling regional estimate.
* LUF is adjusted incrementally to target:

  * High utilization
  * Minimal speculative holding
  * Stable occupancy

**Key Rule:**

> No human assessor may set or override a parcel’s land value.

---

### A.3 Anti‑Corruption Feedback Loop

* Overstated improvements → suppressed inferred land value
* Suppressed LUF → increased occupancy pressure
* Occupancy pressure → vacancy correction → LUF increase
* Persistent bias flags assessors and regions for audit

This creates a closed-loop correction system without discretionary power.

---

## B. Natural Resource Pricing Mechanisms

### B.1 Finite Extractive Resources

Each resource market operates independently.

**Pricing Objective:**

* Maximize total net rent for citizens, not throughput.

**Procedure:**

1. Model demand curve
2. Identify unitary elasticity point
3. Set monopoly sale price
4. Purchase required quantity via competitive supply bids

**Outcomes:**

* Intentional throughput reduction
* High rent capture
* Predictable citizen dividend

---

### B.2 Extractor Interface Models

Two permissible structures:

**Model 1: Monopsony Purchase**

* Existing extractors retain operations
* LRA purchases output
* Rights sunset over time

**Model 2: Contracted Extraction**

* Resources nationalized
* Extraction rights auctioned as service contracts
* Extractors paid per unit delivered

**Transition Protection:**

* Time‑limited bonds compensate lost legacy rents

---

### B.3 Regenerative Resources

Handled contextually:

* Cultivated biomass = production
* Fees attach to land, water, and commons use
* Public ecological assets treated as extractive

---

## C. Citizen Dividend Mechanics

### C.1 Distribution

* Equal per‑capita payment
* Paid at fixed intervals
* No means testing
* No conditionality

### C.2 Political Lock‑In

* Dividend receipt precedes budgeting
* Any reduction in rent capture is immediately visible
* Voters experience repeal as income loss

---

## D. People’s Budget Mechanics

### D.1 Budget Size Vote

* Periodic vote on total public spend
* Rate-of-change caps

### D.2 Allocation Vote

* Per-citizen proportional allocation
* Agency-level or program-level granularity

---

## E. Transition Programs

### E.1 Land Transition Options

1. **Opt‑In Conversion**

   * Owner accepts LUF
   * Receives bond equal to implied land value

2. **Transaction‑Triggered Conversion**

   * Conversion at sale
   * Buyer compensated for land residual only

3. **Stepped Conversion**

   * Scheduled percentage shifts

---

### E.2 Bond Design

* Tradable
* May be interest‑bearing or interest‑free
* Serviced exclusively from LUF revenue
* Designed to extinguish over time

---

## F. Banking & Credit Transition

* Land ceases to be primary collateral
* Mortgages reflect depreciating improvements
* Credit shifts toward productive investment
* Systemic leverage declines

---

## G. Failure Modes & Safeguards

### G.1 Known Failure Modes

* Political exemptions
* Dividend diversion
* Algorithm tampering

### G.2 Safeguards

* Mandatory transparency
* Public audit trails
* Independent verification
* Constitutional protection of dividend priority

---

## H. Scope Boundary

This appendix specifies mechanisms sufficient for feasibility analysis. It deliberately excludes:

* Legal drafting
* Software architecture
* Jurisdiction‑specific implementation details

These are downstream design problems.
