# Implementation Module 28 Spec — Land

## Module
- Number: 28
- Topic: Land (LEF mechanism details)
- Target length: ~2,500 words (variance allowed)
- Skippable: yes

## Who This Affects
- Everyone, but especially landholders, renters, farmers, builders, and local governments.

## Prerequisites
- LEF concept (Part I), land vs improvements, dividend-first ordering, and the “near-zero transfer value” objective.

## Module Job
Provide the implementable LEF mechanism options (valuation/auction paths) including adjustment caps, “land availability buffer” signals, and anti-corruption safeguards.

## Inputs / Measurability
- Stable states: market sales, registries, building assessments, vacancy/utilization signals.
- Greenfield: auction bids for land rights + minimal registry/enforcement assumptions.

## Fee Structure Choice
- Land is fixed-supply and excludable → recurring exclusion fee is the correct archetype.

## Mechanism Summary
Cover two implementation contexts:
- **Stable-state valuation** (sales-residual inference + utilization feedback; no parcel-level discretionary valuation).
- **Greenfield auctions** (rights allocated via competitive annual-payment bids).

Include the pricing signals:
- LEF too low: meaningful buyer→seller transfer value reappears.
- LEF too high: too much unused land; improved parcels trade below improvement value.

## Tunable Parameters
- Adjustment cap anchor (example: CPI + 10%).
- Target buffer/utilization bands (policy choice with warnings).

## Failure Modes & Safeguards
- Corruption via assessments → remove discretionary parcel valuation; publish audit trails.
- Exemptions → kill rent capture; warn explicitly.

## Interfaces
- Collection via LRA (or equivalent); dividend-first routing; People’s Budget only after dividend.
