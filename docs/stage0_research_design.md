# Stage 0 Research Design and Evidence Architecture

**Project:** The Real Cost of Being an Ojol Driver: What’s Left After a Day on the Road?  
**Stage:** 0 — Research Design & Evidence Architecture  
**Status:** Locked for Stage 1 acquisition, subject only to explicit documented revision  
**Date:** 2026-08-27

## 1. Research objective

This project estimates and decomposes the economics of app-based motorcycle drivers in Indonesia without presuming hardship, adequacy, platform impact, or economic sustainability. The analysis separates customer-facing charges, driver earnings, platform-side deductions, incentives, tips, operating costs, vehicle-capital treatment, time commitment, activity, and estimated net operating earnings.

The project may assess affordability or purchasing-power context, but household expenditure is not treated as an operating cost of driving.

## 2. Primary research universe

The primary analytical universe is app-based **motorcycle** work in Indonesia, including where evidence supports:

- motorcycle passenger transport;
- motorcycle food delivery;
- motorcycle parcel/courier delivery;
- other motorcycle app-based delivery services that can be clearly classified.

Car/taxi-online work is not pooled with the primary universe. It may be retained as a separate analytical universe or context if useful.

Platforms are not preselected as an exhaustive list. Platform inclusion is evidence-led and must be bound to service, geography, and observation period.

## 3. Core research questions

1. What are driver gross earnings, deductions, operating costs, and estimated net earnings?
2. Which costs most reduce earnings?
3. How do outcomes vary by workload, service, vehicle, platform, geography, and period?
4. What net earnings per hour, order, and kilometer are defensible?
5. What activity is required to reach specified net-income targets?
6. How sensitive are results to tariffs, fuel prices, incentives, deductions, utilization, maintenance, and working hours?
7. What can and cannot be concluded about economic sustainability?

## 4. Economic flow and accounting boundaries

No single generic `income` field is sufficient. Monetary concepts must remain distinct.

Preferred flow:

`customer-facing charges`
→ `driver gross service earnings`
− `driver-side platform deductions`
+ `incentives/bonuses`
+ `tips`
= `driver receipts before operating costs`
− `fuel/charging`
− `maintenance/consumables`
− `work-related parking/tolls`
− `work-related mobile/data allocation`
− `vehicle cost under the applicable capital treatment`
− `other defensible work-related operating costs`
= `estimated net operating earnings`

A source-reported value is preserved under its original definition even when one or more bridge components are unavailable. Missing bridge components are not reconstructed silently.

### 4.1 Tips and incentives

Tips and incentives are separate from core service earnings wherever evidence permits. Analyses may show both core-earnings economics and total-receipts economics to identify dependence on non-core components.

### 4.2 Household and personal expenditure

Food for the household, housing, electricity, school costs, household debt, and other personal consumption are not driver operating costs. They may be used only in a separately labelled affordability or welfare analysis.

## 5. Analytical units, activity measures, and denominators

The canonical stored unit is a **source measurement observation** identified by source, population/sample, period, geography, platform, service, vehicle, metric definition, and measurement basis.

Analytical units may include transaction/order, driver-day or work shift, driver-week/month, and source-level aggregate. Values are not converted across time units unless the required denominator is observed or explicitly documented.

### 5.1 Time

Time concepts must remain separate:

- `online_hours`: time logged in/available for app-based work;
- `productive_or_engaged_hours`: time directly associated with orders or source-defined productive activity;
- `working_hours_source_reported`: source term retained when a more precise definition is unavailable.

For time-commitment analysis, online/available hours are preferred when measured. Productive-hour earnings may be reported separately as a utilization-related metric. One is never substituted for the other without an explicit transformation and caveat.

### 5.2 Orders and distance

Distance concepts must remain separate:

- paid-trip/delivery distance;
- pickup distance;
- repositioning/deadheading distance;
- total work-related operating distance.

Total work-related distance is preferred for vehicle operating-cost and fuel allocation. Paid-trip distance must not silently stand in for total distance.

### 5.3 Fuel

Fuel/charging is an operating cost, while fuel volume, fuel efficiency, fuel price, and distance are activity/input measures.

Observed or source-reported fuel expenditure is retained as observed evidence. Modelled fuel cost is allowed only when inputs are explicit:

`modelled fuel volume = work-related distance / fuel efficiency`

`modelled fuel cost = modelled fuel volume × fuel price`

Modelled fuel is labelled as derived/modelled and is not mixed with observed fuel expenditure.

## 6. Vehicle capital and financing policy

Capital costs are handled through explicit views to avoid double counting.

### 6.1 Economic-cost view

For an owned vehicle, economic vehicle cost may include depreciation plus financing interest/fees when separately measured. Financing principal is not an additional economic expense when depreciation is already charged.

### 6.2 Cash-flow view

For cash-flow analysis, actual loan installment or lease/rental payment may be treated as a cash outflow. Depreciation must not be deducted again in the same cash-flow metric.

For rented/leased vehicles, rental/lease cost is the driver’s vehicle-access cost and driver-level depreciation is not additionally imposed.

When a source reports only an undivided installment, it may be used as a cash financing outflow but must not be reclassified as depreciation or financing interest.

## 7. Deduction, fee, and regulatory-implementation framework

Regulation and realized driver economics are different evidence layers. The project does not infer realized deductions from a regulatory ceiling, an official announcement, or a platform statement.

Required layers are:

1. `regulatory_deduction_rule` — applicable legal or regulatory rule;
2. `official_implementation_statement` — regulator/government statement about implementation;
3. `platform_stated_deduction` — company-stated policy or implementation;
4. `observed_driver_deduction` — transaction/admin evidence of driver-side deductions;
5. `driver_reported_deduction` — driver or driver-study report when transaction evidence is unavailable;
6. `customer_to_driver_gap` — customer payment minus driver receipt, which is **not automatically platform commission**.

Preferred realized deduction formula:

`realized driver deduction rate = driver-side platform deductions / driver gross earnings before deductions`

The project must not calculate platform commission as:

`(customer payment - driver receipt) / customer payment`

unless the source explicitly establishes that the entire gap is a driver-side commission.

Every fee-rule comparison must be reconciled through:

`legal text → effective date → covered service → geography/scope → platform-stated implementation → observed transaction → reconciliation status`

Default reconciliation statuses:

- `consistent_with_reference`;
- `apparent_difference_requires_reconciliation`;
- `not_assessable`;
- `outside_reference_scope`.

The project does not default to legal conclusions such as `compliant` or `non_compliant`.

### 7.1 Current regulatory issue to verify in Stage 1

As of the Stage 0 design date, Kemenhub JDIH lists KP 1001/2022 as in force. Official presidential communication on 1 May 2026 described Perpres No. 27/2026 and a new transport-online protection policy. An official DPR communication on 23 June 2026 stated that Gojek and Grab would implement an 8% commission for two-wheel passenger services from 1 July 2026. However, a later official DPR communication dated 18 August 2026 described the broader online-transport Perpres as still being finalized and harmonized, including passenger, goods, and food services.

These official communications are not treated as interchangeable legal evidence. Their apparent status/scope tension is itself a Stage 1 verification requirement. The project must obtain or reverify the operative legal text, effective provisions, calculation base, covered services, implementing instruments, and status at each observation date before coding a regulatory benchmark as authoritative.

Stage 1 must therefore preserve dated legal text, official implementation statements, platform statements, and realized driver evidence as separate records. An announced or stated 8% policy must never be substituted for transaction-level realized deductions.

Stage 0 verification references (to be formally registered and revalidated in Stage 1):

- Kemenhub JDIH, KP 1001/2022: https://jdih.dephub.go.id/peraturan/detail?data=EnUUAwj5fOs9ium7YhAKlt8W6K3JcfTsq4q9Hw34l1Nu8lwtPpgEiGM4qBqHiJ4Jwy4fWjw2I3DXw8LWNSqx1TL18Wzka8SnDqn8bURev8f7IX7AC8OA8cmUx5i52nkQsfqO6qLy6TaIsnXJGCELssy2iq
- President of the Republic of Indonesia, 1 May 2026 communication: https://presidenri.go.id/siaran-pers/presiden-prabowo-perkuat-perlindungan-ojol-pangkas-potongan-aplikator-dan-tingkatkan-kesejahteraan/
- DPR RI, 23 June 2026 implementation announcement: https://jdih.dpr.go.id/berita/detail/id/66332/
- DPR RI, 18 August 2026 finalization/harmonization update: https://jdih.dpr.go.id/berita/detail/id/68124/

## 8. Evidence architecture

There is no universal source ranking. Evidence quality is assessed relative to the claim.

Preferred evidence by question:

- legal tariff/rule: official legal text/JDIH;
- official implementation/status: relevant ministry/regulator/government record;
- platform policy: platform terms, driver documentation, or official company statement;
- realized deduction/earnings: transaction/admin records, systematic driver records, or methodologically documented studies;
- working time/distance: administrative/telemetry evidence where available, then documented study or clearly defined self-report;
- fuel prices/regulation: official regulator/supplier records bound to date, location, and product;
- national socioeconomic context: BPS or other authoritative official statistics;
- company aggregate claims: retained as `company_reported`.

Convenience/community/self-reported samples are retained with their recruitment, sample size, geography, period, platform/service coverage, and limitations. They are not treated as nationally representative without support.

## 9. Comparability framework

Each cross-source comparison receives one status:

- `directly_comparable`;
- `comparable_with_transformation`;
- `comparable_with_caveat`;
- `context_only`;
- `not_comparable`.

Before pooling or direct comparison, audit at minimum:

- customer fare vs driver earnings concept;
- gross vs post-deduction vs net;
- period and regulatory regime;
- geography;
- platform;
- service;
- motorcycle/vehicle specification;
- online vs productive vs source-reported hours;
- paid-trip vs total operating distance;
- tips/incentive treatment;
- sampling and population;
- nominal vs inflation-adjusted currency;
- observed vs source-reported vs derived/modelled/scenario evidence.

Incompatibility is a valid result.

## 10. Inflation, purchasing power, and affordability

Source monetary observations are preserved in nominal IDR.

Inflation-adjusted values are derived only when cross-period analysis requires them. The CPI series, geography, base/reference period, transformation, and retrieval source must be documented. The original nominal value is never overwritten.

Basic-needs prices and household expenditure are not operating costs. Affordability analysis, if evidence permits, is a separate analytical layer using defensible official indicators such as CPI, poverty-line components, household expenditure statistics, or other clearly defined cost-of-living indicators.

The project does not construct an arbitrary basic-needs basket and present it as a welfare threshold unless a dedicated scenario is explicitly defined and justified.

## 11. Benchmark policy

UMP/UMK, poverty lines, household expenditure, or other income benchmarks are contextual measures and must be used according to their definitions.

UMP/UMK comparison requires period and geography matching and explicit time-conversion assumptions. A converted benchmark is not legal proof that an independent/platform driver is "paid below minimum wage."

Target-income values used for break-even or activity requirements are labelled scenarios unless they correspond to a documented benchmark.

## 12. Value provenance classes

Every analytical value is classified as one of:

- `observed`;
- `source_reported`;
- `derived`;
- `modelled`;
- `scenario`.

Derived, modelled, and scenario values must retain links to their input observations and assumptions.

## 13. Validation gates

Critical gates are:

1. **Concept gate** — earnings, receipts, deductions, costs, and net concepts are not conflated.
2. **Provenance gate** — source, publisher, period, retrieval date, methodology, geography, population/sample, and redistribution status are documented where applicable.
3. **Definition gate** — units, numerator, denominator, and measurement basis are known.
4. **Comparability gate** — cross-source use has an explicit comparability status.
5. **Capital-cost gate** — depreciation, financing, lease, and acquisition treatment does not double count capital.
6. **Metric-eligibility gate** — per-hour/order/km metrics have compatible denominators.
7. **Calculation gate** — derived values reconcile to documented inputs.
8. **Scenario gate** — assumptions remain separate from observed/source-reported evidence.
9. **Regulatory-reconciliation gate** — normative rule, implementation statement, platform policy, and realized transaction evidence are not conflated.
10. **Synthesis gate** — only validated evidence can support final findings.

Recommended validation outcomes are `pass`, `pass_with_caveat`, `fail_critical`, and `not_applicable`. Critical failures block affected synthesis.

## 14. Stage 1 acquisition requirements

Stage 1 will discover and evaluate sources without assuming compatibility. The source registry must capture at minimum:

- source ID and title;
- publisher/organization;
- URL or stable identifier;
- retrieval date;
- publication date;
- observation period;
- geography;
- platform and service;
- vehicle scope;
- sample/population and recruitment;
- measurement method;
- unit and definition;
- value provenance class;
- redistribution/licensing status;
- uncertainty and limitations;
- regulatory regime where relevant;
- accessibility status.

Raw redistributable evidence is preserved unchanged. Non-redistributable or inaccessible evidence is registered without unlawful redistribution.

## 15. Stage 0 completion criteria

Stage 0 is complete when:

- research universe and accounting boundaries are locked;
- time, distance, order, fuel, and activity measures are defined;
- capital-cost treatment is locked;
- deduction/regulation implementation layers are separated;
- inflation and affordability boundaries are defined;
- evidence architecture and comparability rules are explicit;
- validation gates are defined;
- Stage 1 source-registry requirements are specified.

No analytical finding is produced at Stage 0.
