# The Real Cost of Being an Ojol Driver: What’s Left After a Day on the Road?

Evidence on earnings, deductions, costs, and work intensity among app-based motorcycle drivers in Indonesia.

## Final Answer

**The available evidence does not support one defensible daily net take-home figure for an ojol driver.**

For the aligned IDEAS 2023 Jabodetabek observations (n=186), the mean gross daily earnings used in the project derivation are **Rp168,000**. This corresponds to **Rp15,272.73 gross per source-reported working hour** and **Rp16,800 gross per completed order**.

Those figures are **gross, not net**. A driver may still face realized platform deductions and day-to-day or periodic outlays such as fuel, oil changes, motorcycle servicing, tires and spare parts, mobile/data costs, and parking or tolls where relevant. Food while working also reduces daily cash on hand, although the project treats personal food consumption separately from operating cost. Accident, illness, vehicle breakdown, and downtime add further economic risk.

The project does **not** subtract assumed values for those items. The matched evidence required to connect gross earnings, realized deductions, fuel, and other work-related costs on the same observation basis is unavailable. Therefore, the amount actually left after a day on the road is **not measured yet**—not zero, not Rp168,000, and not a value assembled from unrelated sources.

---

## Key Findings

- In a 2022 Polling Institute survey of 810 drivers, the share reporting less than Rp100,000 per day was 11.6% for the recalled pre-pandemic period, 66.0% for the recalled pandemic period, and 40.4% for the contemporaneous 2022 period. These are source-defined periods within one survey, not independent historical waves.
- The share reporting seven workdays per week was 49.3% in an IDEAS 2020 metropolitan source, 42.2% in the IDEAS 2023 metropolitan source, and 55.5% in the IDEAS December 2025 source. These figures are not a national time series.
- A reported 20% application-deduction category was selected by 52.9% of respondents in the IDEAS 2023 source and 50.3% in the IDEAS December 2025 source. These are driver-reported prevalence measures, not realized transaction-level deduction rates.
- Source-defined fuel plus food/drink spending represented 31.0% of gross daily earnings in the IDEAS 2023 metropolitan source and 46.0% in the IDEAS December 2025 source. The bundle includes personal food/drink expenditure, so it is **not** treated as a pure project operating-cost share.
- Drivers may also face periodic motorcycle expenses that are economically relevant but not jointly observed in the validated gross-to-net chain: oil changes, servicing, tires/spare parts, mobile/data costs, and parking or tolls where relevant. Work disruption from accidents, illness, vehicle breakdown, or downtime is also economically relevant but is not monetized without observed data.
- For aligned IDEAS 2023 source means from 186 observations in Jabodetabek, gross service earnings equal **Rp15,272.73 per source-reported working hour** and **Rp16,800 per completed order**. Both are ratios of source means and are gross, not net.
- **Project net operating earnings are not computable** because the validated evidence does not provide a complete same-observation chain containing driver receipts before operating costs, realized driver-side platform deductions, separate defensible fuel cost, and the other relevant work-cost components.

---

## Visual Results

### Source-defined daily-income distribution

![Daily-income distribution across source-defined periods](visualizations/stage5_src010_income_distribution.svg)

Pre-pandemic and pandemic values are retrospective recall within the 2022 Polling Institute survey. The income concept is not clearly identified as gross, receipt, or net income.

### Mixed fuel plus food/drink spending

![Mixed fuel plus food/drink spending share](visualizations/stage5_mixed_fuel_food_share.svg)

The measure combines work-related fuel with personal food/drink spending and therefore cannot be used as a pure project operating-cost share.

### Seven-day workweek prevalence

![Seven-day workweek prevalence](visualizations/stage5_seven_day_workweek_prevalence.svg)

The sources differ in period, geography, and sampling context. The comparison is descriptive and caveated, not a national trend.

### Reported 20% deduction-category prevalence

![Reported 20 percent deduction-category prevalence](visualizations/stage5_reported_twenty_percent_deduction_prevalence.svg)

These figures describe respondent-reported deduction categories rather than matched realized transaction deductions.

---

## Research Questions — Direct Outcomes

| Question | Direct answer |
|---|---|
| Gross earnings, deductions, costs, and net earnings | Gross earnings and several components can be described; **project net earnings are not computable**. |
| Which costs reduce earnings the most? | **Cannot be determined** from the available evidence. |
| Variation across workload/service/vehicle/platform/geography/period | **Source-bounded variation can be shown**, but not a pooled national trend or a platform/service/vehicle effect. |
| Net earnings per hour/order/km | **Not computable.** Only two valid gross SRC029 rates are available. |
| Activity required for net-income targets | **Not computable.** |
| Multi-input sensitivity analysis | **Not computable.** |
| Overall economic sustainability | **Cannot be determined overall from the current evidence.** |

See the [full research-question synthesis](data/analytical/stage6_research_question_synthesis.csv) for the evidence basis and remaining gaps behind each answer.

---

## Analytical Boundaries

The project does not treat these concepts as interchangeable:

```text
customer-facing charges
→ driver gross service earnings
− realized driver-side platform deductions
+ incentives/bonuses
+ tips
= driver receipts before operating costs
− defensible work-related operating costs
= project net operating earnings
```

Several rules are central to the analysis:

- Missing values are not zero.
- Source-defined “net income” is not substituted for project net operating earnings unless the components match.
- Personal and household expenditure is not operating cost.
- Customer payment minus driver receipt is not automatically platform commission.
- A regulatory ceiling or platform-stated policy is not a realized deduction.
- Paid-trip distance is not assumed to equal total work-related operating distance.
- Retrospective recalled values are not treated as independent panel waves.
- Convenience, purposive, and community samples are not treated as nationally representative by default.

Cross-source uses are classified only as:

`directly_comparable` · `comparable_with_transformation` · `comparable_with_caveat` · `context_only` · `not_comparable`

There are no `directly_comparable` cross-source numerical uses in the final evidence base.

---

## Regulatory Context

Legal rules, official implementation statements, platform-stated policies, driver-reported deductions, and realized transaction deductions are separate evidence layers.

The project therefore does **not** treat the 2023/2025 reported 20% deduction-category prevalence and a stated or planned 8% policy in 2026 as a measured commission decline. They differ in period, service, platform, calculation base, and evidence layer.

The [regulatory reconciliation record](metadata/stage6_regulatory_reconciliation.csv) documents why the available comparisons resolve only as `not_assessable` or `outside_reference_scope`, rather than as legal-compliance or realized-rate conclusions.

---

## Main Evidence Gaps

The final evidence-gap register documents eleven material limitations. The most consequential are:

- no complete same-observation gross-to-net chain;
- no matched transaction-level realized driver deduction evidence;
- no separate defensible driver fuel-cost observation for the project net chain;
- mixed fuel plus personal food/drink spending in the available cost bundle;
- unresolved working-hour definition for the validated hourly gross rate;
- unresolved total work-related distance for per-kilometer economics;
- zero directly comparable cross-source numerical uses;
- 24 unresolved metric-specific denominators;
- an internal 62-versus-67 kabupaten/kota discrepancy in the December 2025 IDEAS source;
- insufficient comparable platform-, service-, and vehicle-stratified economic outcomes;
- no single universal operative 2026 online-transport benchmark established by the available evidence.

See [metadata/stage6_evidence_gap_register.csv](metadata/stage6_evidence_gap_register.csv) for the complete record.

---

## Repository Structure

```text
data/
  analytical/        validated analytical result tables
  processed/         cleaned analytical inputs
  standardized/      harmonized source observations
  raw/               redistributable source material where permitted

docs/                research design and supporting documentation
metadata/            source, methodology, comparability, validation, and traceability records
notebooks/            analytical notebooks
visualizations/       validated figures used in the analysis
```

Key public artifacts include:

- [Research design](docs/stage0_research_design.md)
- [Source registry](metadata/stage1_source_registry.csv)
- [Gross unit-economics results](data/analytical/stage4_unit_economics_results.csv)
- [Evidence-linked findings](data/analytical/stage5_findings.csv)
- [Research-question synthesis](data/analytical/stage6_research_question_synthesis.csv)
- [Regulatory reconciliation](metadata/stage6_regulatory_reconciliation.csv)
- [Evidence-gap register](metadata/stage6_evidence_gap_register.csv)
- [Methodological decision log](metadata/stage6_methodological_decision_log.csv)
- [Synthesis validation](metadata/stage6_synthesis_validation.csv)

---

## Reproducibility and Traceability

The repository preserves source URLs, publishers, observation periods, geography, sample/population details, measurement definitions, comparability status, uncertainty, and value provenance where available.

Analytical values are classified as `observed`, `source_reported`, `derived`, `modelled`, or `scenario`. The synthesis relies on validated committed evidence rather than replacing missing components with assumptions.

The analytical notebooks and validation records provide a reproducible path from source evidence through standardized and processed data to findings and final synthesis.

---

## Final Verdict

**There is no defensible single daily net-income figure in the current evidence base.**

The strongest measured SRC029 figures are **Rp168,000 gross per day**, **Rp15,272.73 gross per source-reported working hour**, and **Rp16,800 gross per completed order**. They sit before a complete matched accounting of deductions and costs.

Drivers still face economic burdens after gross earnings: fuel; oil changes; servicing; tires/spare parts; mobile/data expenses; parking or tolls where relevant; food while working as a personal cash outflow; and work-disruption risks such as accidents, illness, vehicle breakdown, and downtime. The project does not guess the value of those missing components.

Therefore, the answer to “what is left after a day on the road?” is: **not measured yet with sufficient evidence**. That is a firm measurement conclusion, not a zero-income assumption and not an invitation to combine incompatible sources.
