# The Real Cost of Being an Ojol Driver: What’s Left After a Day on the Road?

Evidence on earnings, deductions, costs, and work intensity among app-based motorcycle drivers in Indonesia.

This repository examines a deceptively simple question: **after earnings, deductions, and operating costs, what can we defensibly say is left for an ojol driver?**

The answer is not one national net-income number. The available evidence supports several source-specific findings and two transparent gross unit-economics rates, but it does not contain a complete, comparable, same-observation chain from gross earnings to project net operating earnings.

---

## Key Findings

- In a 2022 Polling Institute survey of 810 drivers, the share reporting less than Rp100,000 per day was 11.6% for the recalled pre-pandemic period, 66.0% for the recalled pandemic period, and 40.4% for the contemporaneous 2022 period. These are source-defined periods within one survey, not independent historical waves.
- Source-defined fuel plus food/drink spending represented 31.0% of gross daily earnings in an IDEAS 2023 metropolitan source and 46.0% in an IDEAS December 2025 source. The bundle includes personal food/drink expenditure, so it is **not** treated as project operating cost.
- The share reporting seven workdays per week was 49.3% in an IDEAS 2020 metropolitan source, 42.2% in the IDEAS 2023 metropolitan source, and 55.5% in the IDEAS December 2025 source. These figures are not a national time series.
- A reported 20% application-deduction category was selected by 52.9% of respondents in the IDEAS 2023 source and 50.3% in the IDEAS December 2025 source. These are driver-reported prevalence measures, not realized transaction-level deduction rates.
- For aligned IDEAS 2023 source means from 186 observations in Jabodetabek, gross service earnings equal **Rp15,272.73 per source-reported working hour** and **Rp16,800 per completed order**. Both are ratios of source means and are gross, not net.
- Project net operating earnings remain **not computable** because the validated evidence does not provide a complete same-observation chain containing driver receipts before operating costs, driver-side platform deductions, and separate defensible fuel cost.

---

## Visual Results

### Source-defined daily-income distribution

![Daily-income distribution across source-defined periods](visualizations/stage5_src010_income_distribution.svg)

Pre-pandemic and pandemic values are retrospective recall within the 2022 Polling Institute survey. The income concept is not clearly identified as gross, receipt, or net income.

### Mixed fuel plus food/drink spending

![Mixed fuel plus food/drink spending share](visualizations/stage5_mixed_fuel_food_share.svg)

The measure combines work-related fuel with personal food/drink spending and therefore cannot be used as a project operating-cost share.

### Seven-day workweek prevalence

![Seven-day workweek prevalence](visualizations/stage5_seven_day_workweek_prevalence.svg)

The sources differ in period, geography, and sampling context. The comparison is descriptive and caveated, not a national trend.

### Reported 20% deduction-category prevalence

![Reported 20 percent deduction-category prevalence](visualizations/stage5_reported_twenty_percent_deduction_prevalence.svg)

These figures describe respondent-reported deduction categories rather than matched realized transaction deductions.

---

## Research Questions

The project evaluates seven questions:

1. What are driver gross earnings, deductions, operating costs, and estimated net earnings?
2. Which costs most reduce earnings?
3. How do outcomes vary by workload, service, vehicle, platform, geography, and period?
4. What net earnings per hour, order, and kilometer are defensible?
5. What activity is required to reach specified net-income targets?
6. How sensitive are results to tariffs, fuel prices, incentives, deductions, utilization, maintenance, and working hours?
7. What can and cannot be concluded about economic sustainability?

The final synthesis produces the following evidence-bounded outcomes:

| Question | Outcome |
|---|---|
| Gross earnings, deductions, costs, and net earnings | `partially_supported` |
| Ranking of operating-cost components | `not_assessable` |
| Variation across workload/service/vehicle/platform/geography/period | `partially_supported` |
| Net earnings per hour/order/km | `not_computable` |
| Activity required for net-income targets | `not_computable` |
| Multi-input sensitivity analysis | `not_computable` |
| Overall economic sustainability | `not_assessable` |

See the [full research-question synthesis](data/analytical/stage6_research_question_synthesis.csv) for the evidence basis and remaining gaps behind each outcome.

---

## Analytical Boundaries

The project does not treat these concepts as interchangeable:

```text
customer-facing charges
→ driver gross service earnings
− driver-side platform deductions
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

Legal rules, official implementation statements, platform-stated policies, driver-reported deductions, and realized transaction deductions are preserved as separate evidence layers.

The project therefore does **not** interpret the 2023/2025 reported 20% deduction-category prevalence against a stated or planned 8% policy in 2026 as a measured commission reduction. The observations differ in period, service, platform, calculation base, and evidence layer.

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

## Scope of the Conclusion

This project does not produce a single national estimate of ojol driver net operating earnings. It also does not produce a realized national platform deduction rate, a defensible ranking of operating-cost components, a per-kilometer net rate, a target-income activity model, or an overall economic-sustainability verdict.

The strongest conclusion is narrower and more useful: the available evidence can measure several important parts of driver economics, but the complete gross-to-net accounting chain remains unavailable on a comparable same-observation basis.
