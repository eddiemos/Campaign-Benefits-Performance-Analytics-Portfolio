# Campaign Benefits & Performance Analytics

An anonymized Power BI business-intelligence case study for monitoring multi-market campaign execution, customer conversion, digital-channel adoption and financial outcomes.

> **Portfolio disclosure:** This repository documents an anonymized enterprise dashboard case study. Organization names, market identities, campaign identifiers and all displayed figures have been generalized or replaced with synthetic examples. The original PBIX, source data, customer records, proprietary definitions and organization-specific assets are **not included**.

## Project overview

The dashboard brings campaign execution and business outcomes into a single reporting experience. It is designed to help business and marketing stakeholders understand whether targeted campaigns are converting into product uptake and measurable financial activity, and how performance varies by market, campaign and time period.

The report combines an executive performance view with more detailed market and campaign monitoring. Its reporting themes include:

- Audience targeting and product uptake
- Lead-to-conversion performance
- Average products per converted customer
- Loan characteristics and disbursement monitoring
- Digital-channel adoption
- Campaign-generated and projected revenue
- Market-level comparisons
- Daily and monthly campaign execution trends

## Business problem

Campaign teams need to connect execution metrics (who was targeted and when) with outcome metrics (who converted, what product was taken up and what financial activity followed). When these measures are fragmented across separate reports, it becomes difficult to compare campaign performance, spot weaker conversion funnels or monitor the contribution of different markets and channels.

This case study illustrates a consolidated BI approach to that problem.

## Analytical objectives

1. Monitor the size of campaign audiences and the volume of resulting product conversions.
2. Compare conversion performance across markets and campaign categories.
3. Track financial outcomes separately from operational activity.
4. Understand the contribution of digital channels to campaign conversions.
5. Monitor campaign activity over time using daily and monthly views.
6. Give stakeholders interactive filters to focus on campaign, period, market, product and channel.

## Dashboard experience

The source report contains multiple report pages. The portfolio summary groups them into these functional areas:

| Reporting area | What it helps stakeholders examine |
|---|---|
| Executive benefits tracker | Headline KPIs, revenue summaries, projections and overall trends |
| Market performance | Targeting, conversion, product uptake and financial outcomes by market |
| Daily campaign tracker | Campaign activity and conversions over time, with campaign-level breakdowns |
| Advanced campaign analysis | Comparative campaign/channel performance |
| Execution calendar | Campaign timing and execution context |
| Summary and simplified views | Condensed reporting for quick review |
| Metric glossary | Business meaning and calculation notes for reported indicators |

The preview in [`screenshots/dashboard-preview.png`](screenshots/dashboard-preview.png) and the additional [executive overview](screenshots/executive-overview-synthetic.png), [region performance](screenshots/region-performance-synthetic.png) and [daily activity](screenshots/daily-activity-synthetic.png) illustrations are newly drawn synthetic mockups. They use generic labels and fabricated values and contain no pixels, company marks or reported figures from the source screenshots.

## KPI framework

The dashboard's KPI framework covers the following categories:

| Category | Example measures | Analytical purpose |
|---|---|---|
| Reach | Customers targeted | Quantifies campaign audience |
| Conversion | Products sold, lead conversion | Measures response from the targeted audience |
| Product uptake | Products per customer | Indicates depth of product uptake |
| Lending profile | Average loan amount, average term, average interest rate | Describes the profile of converted lending activity |
| Digital adoption | Digital adoption, digital marketplace adoption | Tracks conversion through selected digital routes |
| Financial outcomes | Loan disbursement, campaign revenue, lifetime revenue, projected revenue | Monitors financial activity associated with campaign performance |

**Metric interpretation:** The source glossary defines lead conversion as conversions divided by targeted customers. It describes digital adoption using a set of digital routes, and loan disbursement as the sum of gross payouts associated with conversions. Exact metric definitions and time windows can vary by organization and campaign; this repository intentionally avoids publishing proprietary calculation details.

## Analytical observations

The report design supports several useful lines of investigation:

- **Market variation:** Compare reach and conversion together; a large audience does not necessarily produce a high conversion rate.
- **Campaign mix:** Examine whether campaign categories differ in their ability to convert targeted customers.
- **Channel adoption:** Compare digital adoption with overall conversion to understand channel contribution.
- **Time effects:** Review monthly targeting and conversion patterns alongside campaign execution dates.
- **Financial interpretation:** Keep disbursement, revenue generated to date, lifetime revenue and projected revenue distinct. They represent different business concepts and should not be treated as interchangeable.

These are analytical questions supported by the dashboard structure, not claims that a particular campaign caused a particular outcome.

## Data and privacy approach

The public repository uses a synthetic example dataset in [`data/synthetic_market_kpis.csv`](data/synthetic_market_kpis.csv).

- Market labels are generic (`Market A`, `Market B`, etc.).
- Campaign labels are generic.
- Values are fabricated for demonstration and do not reproduce the source report.
- Dashboard illustrations are newly drawn with synthetic data; source screenshot pixels and company branding are not included.
- No customer-level records, personal identifiers, original organization names, original campaign IDs or source-system connection details are included.
- The original PBIX is intentionally excluded because a Power BI file can retain underlying data, model metadata, query definitions, connection details, hidden objects and other information even when visible report labels are changed.

Do not add the original PBIX, raw exports, customer-level data, credentials, connection strings or unapproved screenshots to this repository.

## Tools and techniques represented

- Microsoft Power BI — interactive reporting and dashboard design
- DAX — KPI and measure logic (the original expressions are not redistributed)
- Data modelling — organizing campaign and outcome information for analysis
- Data transformation — preparing reporting data for analysis
- Business intelligence — KPI design, performance monitoring and stakeholder reporting

The list describes the techniques represented by the case study; it is not a claim that this repository contains the original model or transformation scripts.

## Repository structure

```text
campaign-benefits-portfolio/
├── README.md
├── .gitignore
├── data/
│   └── synthetic_market_kpis.csv
├── docs/
│   └── business-overview.md
└── screenshots/
    ├── dashboard-preview.png
    ├── executive-overview-synthetic.png
    ├── region-performance-synthetic.png
    └── daily-activity-synthetic.png
```

## Using the synthetic data

The CSV is provided only to demonstrate the shape of a market-level KPI dataset. It can be opened in Excel, imported into Power BI, or explored with Python.

Suggested exercises:
1. Calculate conversion rate as `conversions / customers_targeted`.
2. Compare conversion rates across markets.
3. Compare digital adoption with conversion rate.
4. Visualize monthly targeting and conversion trends after adding your own synthetic time-series data.
5. Build a summary page with cards, a market comparison chart and a trend chart.

## Limitations

- This repository does not contain the original PBIX or source dataset.
- The preview, additional dashboard illustrations and CSV contain synthetic content.
- The source PDF provides report-level descriptions and selected KPI definitions, but not the complete underlying data model, all DAX expressions or Power Query scripts.
- The case study describes dashboard capabilities; it does not establish causal campaign impact.

## Attribution and portfolio context

This is an anonymized portfolio case study based on the structure and reporting themes of an enterprise campaign-benefits dashboard. It is presented for demonstrating business intelligence analysis and documentation. It does not claim ownership of the original enterprise solution or its proprietary materials.
