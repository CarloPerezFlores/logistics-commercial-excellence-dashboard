# Data inventory and publication notes

The Power BI Fields pane showed these eight loaded tables:

| Power BI table | Uploaded file identified | Notes |
|---|---|---|
| `delivery_events` | `delivery_events.csv` | Detailed event records; do not publish raw without review. |
| `dim_driver` | `dim_driver.csv` | Contains personal and license-related fields; keep private. |
| `dim_route` | `dim_route.csv` | Route dimension; verify data rights before publishing. |
| `dim_truck` | `dim_truck.csv` | Includes vehicle identifiers; review before publishing. |
| `fact_loads` | `fact_loads.csv` | Detailed commercial transactions; verify data rights. |
| `Revenue Monthly Forecast` | `Revenue_Monthly_Forecast.csv` | Aggregated monthly revenue output. |
| `Revenue_Forecast_12_Months` | `Revenue_Forecast_12_Months.csv` | Forecast output with `ds`, `yhat`, `yhat_lower`, `yhat_upper` columns. |
| `vw_kpi_loads` | `vw_kpi_loads.csv` | Aggregated KPI output by date and load type. |

Other uploaded files appear to be additional source tables, alternate versions, or backups. They are not included by default. In particular, do not include `fact_loads_backup*.csv` unless you establish which version is authoritative and necessary.

The forecast output has Prophet-style column names, but the CSV alone does not prove which script or environment generated it. Include Python source only if the original code is found and validated.
