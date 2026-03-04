
# Marketing Channel Performance Analysis
### BigQuery Public Dataset | Google Analytics Sample

---

## Project Overview

This project analyses marketing channel performance to identify where traffic volume does not translate into session quality and where optimisation efforts should focus.

The objective was to evaluate whether high-traffic channels deliver proportional business value and uncover optimisation opportunities.

---

## Business Question

Which marketing channels drive the most sessions, and which deliver the highest-quality sessions relative to their traffic contribution?

---

## Data Source

Dataset:  
`bigquery-public-data.google_analytics_sample`  
(Google BigQuery Public Dataset)

Data was queried directly in BigQuery and aggregated at channel level.

The processed dataset used for visualisation is included in:

```
/data/marketing_channel_performance.csv
```

---

## Methodology

### 1. Data Extraction (BigQuery)

Channel-level session data was extracted and aggregated using SQL.

The query used for aggregation and metric creation is available in:

```
/sql/channel_performance_query.sql
```

---

### 2. Derived Metrics

Traffic Share
```
Channel Total Sessions / Overall Total Sessions
```

Quality Share
```
Channel High Quality Sessions / Overall High Quality Sessions
```

Performance Gap
```
Quality Share − Traffic Share
```

This metric identifies:

- Underperforming channels (high traffic but lower proportional quality)
- Overperforming channels (higher efficiency relative to size)

---

## Key Findings

- Google / Organic drives approximately 31% of traffic but under-indexes on quality relative to its traffic share.
- Direct traffic shows a similar underperformance pattern.
- Referral channels demonstrate stronger relative efficiency.
- Smaller segments generate disproportionately high-quality contributions.

---

## Strategic Recommendations

### Improve Organic Quality
Segment organic traffic by intent and landing page to identify low-yield segments.

### Investigate Direct Attribution
Assess whether direct traffic includes misclassified sessions due to missing tracking parameters.

### Scale High-Performing Referrals
Identify and expand high-efficiency referral sources.

### Model Budget Reallocation
Simulate shifting optimisation focus toward higher-yield channels.

---

## Visualisation

The interactive dashboard was built in Tableau Public.

View Interactive Dashboard:  
PASTE_YOUR_TABLEAU_LINK_HERE

---

## Tools and Technologies

- Google BigQuery — Data querying and aggregation
- SQL — Metric derivation and performance modelling
- Tableau Public — Data visualisation
- PowerPoint — Stakeholder presentation

---

## Project Structure

```
marketing-channel-performance-analysis/
│
├── assets/          # Dashboard images
├── data/            # Processed aggregated dataset (CSV)
├── slides/          # Final presentation (PDF)
├── sql/             # BigQuery SQL query
└── README.md
```

---

## What This Project Demonstrates

- Translating business questions into measurable metrics
- Querying structured public datasets using SQL
- Creating derived performance indicators
- Identifying optimisation opportunities
- Communicating insights clearly to stakeholders
- Delivering a complete end-to-end analytics workflow

---

## Notes

This project uses publicly available sample data from Google BigQuery.
All analysis and derived metrics were created independently for portfolio demonstration purposes.
