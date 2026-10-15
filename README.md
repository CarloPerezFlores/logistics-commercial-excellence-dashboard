# Logistics Commercial Excellence Dashboard

An interactive Power BI portfolio project focused on logistics commercial performance, shipment activity, customer contribution, route performance, and revenue forecasting.

## Project overview

The dashboard brings together commercial and logistics indicators to support executive reporting and planning. It is organized into four report pages:

- **Executive Overview** — headline KPIs, revenue trends, service-type contribution, customer and route rankings, and a revenue forecast view.
- **Operational Performance** — shipment volume, revenue contribution, load type comparisons, revenue over time, and route-level summaries.
- **Customer Performance** — customer revenue ranking, customer revenue trends, and revenue-versus-shipment-volume analysis.
- **Route Performance** — route revenue, shipment volume, revenue per load, and route-level summaries.

## Dashboard previews

### Executive Overview
![Executive Overview](./01-executive-overview.png)

### Operational Performance
![Operational Performance](./02-operational-performance.png)

### Customer Performance
![Customer Performance](./03-customer-performance.png)

### Route Performance
![Route Performance](./04-route-performance.png)

## Tools and methods represented

- **Power BI** for interactive reporting and visualization.
- **Power Query** for data preparation where used in the report.
- **DAX** for KPI calculations where implemented in the semantic model.
- **Relational/star-schema concepts** for organizing fact and dimension data.
- **Revenue forecast output** imported into the report for visualization.
- **SQL concepts** for customer, route, and monthly revenue aggregations.

> Note: The original Python source code and the Power BI `.pbix` file are not included in this repository package. The forecast CSVs are provided as output artifacts; the exact code and validation methodology used to generate them have not been verified here.

## Repository structure

```text
.
├── assets/
│   └── dashboard/          # Original dashboard screenshots
├── data/
│   └── aggregated/         # Aggregated KPI and forecast outputs
├── docs/
│   └── database-schema.txt # Database schema reference
└── README.md
```

## Data and privacy note

Only selected analytical datasets and reporting outputs are included in this repository. Source data should be shared only when permitted by applicable licensing, ownership, and privacy requirements.

## Limitations

Revenue analysis does not necessarily reflect profitability, as transportation costs are not included in the revenue metrics. Forecast outputs should be evaluated against actual results before drawing conclusions about predictive accuracy.

## Business questions supported

- How does revenue change over time?
- Which customers contribute the most revenue?
- Which routes lead in revenue and shipment volume?
- How do load types compare in revenue and shipment activity?
- What does the provided revenue forecast output indicate for planning?

## Limitations

- Revenue contribution is not the same as route profitability. Profitability requires relevant transportation costs.
- Forecast performance should be evaluated against a holdout period and suitable error metrics before describing it as accurate.
- Findings and recommendations should be interpreted in the context of the underlying data and its quality.

## Status

Portfolio documentation and dashboard screenshots prepared. Add the validated `.pbix` file and any shareable source code only after confirming that the files are available and safe to publish.
