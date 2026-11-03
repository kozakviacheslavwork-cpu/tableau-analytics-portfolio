# Ecommerce Conversion Analysis
**SQL · BigQuery · GA4 sample data · Tableau Public**

![Ecommerce dashboard](../assets/tableau_ecommerce.jpg)

[Live Tableau dashboard](https://public.tableau.com/app/profile/viacheslav.kozak/viz/EcommerceConversionAnalysis_17830668997120/EcommerceConversionAnalysis) · [Submitted BigQuery query](https://console.cloud.google.com/bigquery?sq=578385795889:0e6e26b86c2542348ec8a620da0be80a)

## Business question

How do visitors progress from starting a session to making a purchase? Which stages, traffic sources and device categories should a marketing team investigate?

## Data

Public GA4 ecommerce sample: `bigquery-public-data.ga4_obfuscated_sample_ecommerce.events_*`. The dashboard covers November 2020–January 2021.

## My work

- Prepared event and session data with SQL in BigQuery.
- Built a seven-step funnel: Session Start → View Item → Add to Cart → Begin Checkout → Add Shipping Info → Add Payment Info → Purchase.
- Created session, purchase and conversion KPIs, plus session and conversion trends.
- Added country, Traffic Medium and Device Category views.
- Configured filters for session date, landing page, source, medium, campaign, device, language and operating system.
- Refined the funnel, layout, filters and purchase-conversion tooltips.

## Results

| Metric | Value |
| --- | ---: |
| Sessions | 354,857 |
| Purchases | 4,745 |
| Purchase conversion | ≈1.34% |
| SQL result rows, recorded in mentor review | 867,735 |

The overall conversion is approximately `4,745 / 354,857 × 100`. Sessions, purchases and SQL output rows are distinct units; the row count must not be presented as a user count.

## How to explore

Open the live dashboard, compare traffic and device segments, and inspect the funnel. Check the selected filters before comparing totals. Distinguish conversion from session start from conversion between consecutive stages.

## Scope

Final educational project completed at GoIT. No changes were implemented in a commercial store, and no uplift in sales or profit is claimed. The repository links to the submitted SQL query; an exported SQL file is not included.

[Back to portfolio](../README.md)
