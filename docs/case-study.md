# Case study: turning pizza sales into operational questions

## Audience and problem

Restaurant managers need a consistent view of orders, revenue, and product mix before making staffing or promotion decisions. The report groups those questions into Overview, Orders, and Revenue pages.

## Analytical approach

The Overview page combines KPI cards with hourly demand and category/size comparisons. The Orders page highlights product extremes and day-type demand. The Revenue page compares category/product contribution and month/weekday combinations.

The portfolio evidence is the supplied PBIX and three screenshots. The author describes DAX and Power Query as the tools used; raw source tables and a separately exported measure catalog are not supplied, so exact cleaning steps and DAX formulas are not reconstructed here.

## Findings

The overview displays 817.86K revenue, 21.35K orders, and an average order value of 38.31. These are display-rounded values. The order screenshot shows business days at 68.64% of orders, but the five-day versus two-day split means this is not evidence that an individual weekday is busier than an individual weekend day.

Hourly order volume shows midday and evening peaks. Large pizzas lead the size charts. Both patterns are useful prompts for capacity and ingredient planning, with further validation needed against costs, availability, and operating hours.

## Recommendations to evaluate

- Compare order volume per operating hour before changing staffing.
- Combine sales mix with ingredient cost and contribution margin before promoting a category or size.
- Review low-volume products for margin, availability, and strategic role before removing them.
- Correct monthly ordering in the report before using the line chart to communicate seasonality.

No changes to sales, staffing cost, or revenue have been measured as a result of this report.

## Review path

Start with the overview image in the README, inspect the Orders and Revenue previews, then open Modeling.pbix on Windows for interaction and model inspection. The file integrity checks run in Linux do not replace that final Power BI review.
