# Metrics and report review

## Definitions to verify in Power BI Desktop

These are business definitions for review, not claims about the current model's exact DAX implementation.

| KPI | Intended definition | Validation needed |
| --- | --- | --- |
| Revenue | Sum of recorded line revenue | Confirm whether price is multiplied by quantity and how discounts/taxes are represented |
| Orders | Distinct order identifiers | Confirm use of an order ID rather than a line count |
| Pizzas sold | Sum of line quantities | Reconcile with source totals |
| Average order value | Revenue / distinct orders | Use matching filter context and a zero-denominator guard |
| Average pizzas per order | Quantity / distinct orders | Use the same order definition as the order KPI |

## Presentation improvements requiring Power BI Desktop

- Sort month labels by month number for chronological line charts. The supplied screenshots rank months by metric.
- Use full, readable product names or tooltips where axes truncate labels.
- Replace abbreviations and typos such as “Avg Ord Valus” and “Total Rev” with consistent titles.
- Specify the source period, currency, and last refresh date once confirmed.
- Compare weekday/weekend rates per day alongside total shares.
- Consider a higher-contrast, less saturated theme and consistent spacing.
- Export measure definitions and document table grain/relationships for auditability.

These are a review backlog. The existing PBIX and screenshots have not been visually redesigned or rendered in this Linux environment.

## Evidence status

Verified: PBIX ZIP CRC, nonempty embedded DataModel, three populated layout sections (13, 8, and 5 visual containers), and PNG chunk CRCs for all three screenshots. Visual-container counts include decorative and navigation elements.

Not independently verified: exact source totals, DAX evaluation, filter interactions, refresh, data provenance, and any business impact. No raw sales CSVs or source license are included in the repository.
