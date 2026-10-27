# HyunJung Kwak — Portfolio V2 (review branch)

This is an independent review build. It does not replace or modify the existing published `index.html` or `index_monotone_portfolio.html`.

## Source and honesty notes
- AI video link was recovered from the existing `index_monotone_portfolio.html`. The site links directly to the original LinkedIn post, without claiming to embed or host it.
- Lidl BI `.pbit` was inspected. It includes `Market_Data`, `Lidl_KPIs (2)` and `Insight_Framework (2)`, report definition, DAX and M query references, but **not** the original Excel row data.
- The market share demo is **synthetic** until a user-supplied CSV is loaded. The browser does not upload CSV to a server and does not save it persistently.
- The commercial KPI simulator uses hypothetical inputs, not Lidl operational performance or company-held confidential information.
- Brand and trademark references are factual/identificational, with an explicit not-affiliated/not-endorsed disclaimer.

## Preview locally
Open `index.html` in a browser. No build or network access is required for the dashboard and simulator; the external LinkedIn link requires the internet.

## Replace demo data
Export the original Excel `Market_Data` sheet to UTF-8 CSV with columns `Retailer,Market Share (%),Period,Source`. Use the chart's CSV input. Every retailer-period pair must be unique; periods must use compatible definitions. The sample values should never be presented as real observations.

## True Power BI embed
For actual Power BI report interactions, the project needs a `.pbix` published to Power BI Service and a legitimate public `Publish to web` iframe, subject to licensing/admin settings and public-data review. `.pbit` is a template, not an embed URL. Do not expose confidential data. After a valid public URL is obtained, add it separately from the local SVG demonstration.

## Changes to original site
None. This review build is intentionally confined to a separate `portfolio-v2-review` branch and `v2` directory. Do not merge or deploy without review.