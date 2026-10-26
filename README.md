# Pizza Sales Performance Dashboard

**Power BI · DAX · Power Query · Sales Analysis**

A three-page Power BI report for exploring order demand, product mix, and revenue. The portfolio case focuses on how an analyst can translate a sales dashboard into staffing, assortment, and promotion questions.

![Pizza sales overview with order, revenue, category, and size KPIs](main%20dashboard.png)

## Business questions

- When is order demand highest, and how could that inform staffing?
- Which pizza categories and sizes contribute the most revenue and units?
- Which products merit a closer look before a promotion or menu change?

## Dashboard KPIs

These values are displayed in the saved overview screenshot and are rounded by the report.

| Metric | Displayed value |
| --- | ---: |
| Revenue | 817.86K |
| Orders | 21.35K |
| Pizzas sold | 50K |
| Average order value | 38.31 |
| Average pizzas per order | 2.32 |

Exact underlying totals, currency, source coverage, and measure expressions have not been independently reproduced from raw data. Rounded cards should not be used to reverse-engineer exact totals.

## Findings and decisions to explore

| Observation in the saved report | Decision it could inform | Further check |
| --- | --- | --- |
| Business days account for 68.64% of orders; weekends account for 31.36% | Evaluate weekday and weekend coverage | Compare orders per day and per staffed hour because the groups contain different numbers of days |
| Order demand has visible lunchtime and evening peaks | Review staffing and prep schedules around busy periods | Check hourly patterns by weekday and actual operating hours |
| Classic has the largest category revenue, while categories are relatively close in contribution | Compare assortment and promotions across categories | Add contribution margins and ingredient costs before prioritizing sales |
| Large pizzas lead both revenue and unit volume | Review size mix and inventory requirements | Check profit per pizza and ingredient usage rather than revenue alone |

Recommendations are proposals to investigate; this repository does not claim measured business improvements.

## Explore the three pages

| Page | What it shows | Preview |
| --- | --- | --- |
| Overview | KPI cards, demand by hour, category and size mix | [Main dashboard](main%20dashboard.png) |
| Orders | Best/worst-selling pizza selections, weekday units, day-type orders, monthly orders | [Order dashboard](order%20dashboard.png) |
| Revenue | Revenue by category/product and month/weekday | [Revenue dashboard](Rev%20dashboard.png) |

The saved monthly charts are sorted by metric, rather than calendar order. They support month comparisons, but the connecting line on the Orders page should not be interpreted as a chronological trend. See [review notes](docs/report-review.md) for the proposed presentation changes.

## Open the report

1. Download or clone this repository.
2. Open [Modeling.pbix](Modeling.pbix) in a current Windows installation of Power BI Desktop.
3. Inspect the existing model, relationships, and DAX before refreshing.
4. If refresh asks for a local source, provide the original dataset and update its connection in Power Query.

The separate raw source files and a refresh configuration are not included. The screenshots provide a browser-readable review path; this repository does not include a hosted interactive Power BI link.

## What this project demonstrates

Multi-page report navigation, KPI presentation, demand segmentation, product-mix exploration, and the distinction between a descriptive finding and a business recommendation. See [the case study](docs/case-study.md) for the reasoning and [metric definitions and review notes](docs/report-review.md) for validation limits.

The PBIX archive passes CRC checks, contains an embedded data model, and has three populated report pages. Those file checks do not prove DAX correctness, source-refresh success, or interactive behavior. The original PBIX and dashboard images are preserved.

## Related projects

[Retail SQL & Profitability Analysis](https://github.com/marwanfaisal14/retail-sales-analysis) · [Healthcare Billing Dashboard](https://github.com/marwanfaisal14/-Healthcare-Billing-Cost-Analysis-Dashboard-Power-BI-)
