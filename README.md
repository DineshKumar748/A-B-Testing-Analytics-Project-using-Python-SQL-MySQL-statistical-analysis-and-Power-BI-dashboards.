# End-to-End A/B Testing Analytics Project

## Project Overview

This project demonstrates a complete end-to-end A/B Testing Analytics workflow using Python, MySQL, SQL, statistical testing, and Power BI.

The objective of this project was to analyze user conversion performance between control and treatment groups, evaluate uplift, measure statistical significance, and generate business recommendations using real-world analytics techniques.

The project follows a professional analytics pipeline from raw CSV data processing to dashboard reporting and business insight generation.

---

# Tech Stack

| Technology | Purpose |
|---|---|
| Python | Data cleaning and preprocessing |
| Pandas | Data transformation |
| MySQL | Database storage and SQL analysis |
| SQLAlchemy | Python-MySQL connection |
| SQL | Analytical querying |
| Statsmodels | Statistical significance testing |
| Power BI | Interactive dashboard reporting |
| Jupyter Notebook | End-to-end workflow documentation |

---

# End-to-End Analytics Workflow

```text
Raw CSV Files
     ↓
Python Data Cleaning
     ↓
MySQL Database
     ↓
SQL Analysis
     ↓
A/B Testing Metrics
     ↓
P-value Statistical Testing
     ↓
SQL View Creation
     ↓
Power BI Dashboard
     ↓
Business Insights & Recommendations
```

---

# Power BI Dashboard

![Dashboard Overview](screenshots/dashboard/ab_test_powerbi_dashboard_overview.png)

The dashboard provides:

- KPI summary cards
- Conversion analysis
- Country-level performance analysis
- User engagement analysis
- Interactive slicers
- Business recommendations

---

# Data Modeling

![Data Model](screenshots/modeling/data_model_relationships.png)

The Power BI model integrates:

- `ab_test`
- `countries_ab`
- `vw_ab_test_analysis`

using relational modeling for reporting and filtering.

---

# MySQL to Power BI Integration

## MySQL Connection

![MySQL Connection](screenshots/powerbi/mysql_powerbi_connection.png)

## Loading SQL View into Power BI

![Power BI Load](screenshots/powerbi/mysql_powerbi_connection_load.png)

A SQL reporting view was created in MySQL and directly connected to Power BI for dashboard reporting.

---

# SQL Analysis & Insights

---

## Conversion Rate Analysis

![Conversion Rate Analysis](screenshots/sql_analysis/ab_test_conversion_rate_analysis.png)

### Findings

- Control conversion rate: 12.04%
- Treatment conversion rate: 11.89%

The control group slightly outperformed the treatment group.

---

## Country-Level Conversion Analysis

![Country Conversion Analysis](screenshots/sql_analysis/ab_test_country_conversion_analysis.png)

### Findings

- UK treatment group showed slightly stronger conversion performance
- US and CA treatment groups underperformed compared to control

This suggests possible regional differences in user behaviour.

---

## User Engagement Analysis

![Engagement Analysis](screenshots/sql_analysis/ab_test_engagement_analysis.png)

### Findings

- Average session duration remained similar across groups
- Engagement time did not strongly influence conversion outcomes

---

## Page Performance Analysis

![Page Analysis](screenshots/sql_analysis/ab_test_page_performance_analysis.png)

### Findings

- The old page slightly outperformed the new page
- The treatment page failed to generate meaningful conversion improvement

---

## Uplift Analysis

![Uplift Analysis](screenshots/sql_analysis/ab_test_uplift_analysis.png)

### Findings

- Uplift Percentage: -1.23%

The treatment page reduced conversion performance compared to the control version.

---

## Statistical Significance Testing

![Statistical Significance](screenshots/sql_analysis/ab_test_statistical_significance.png)

### Findings

- P-value: 0.2161
- Result was NOT statistically significant

Since the p-value was greater than 0.05, the observed difference may have occurred due to random chance.

---

# Business Recommendation

Based on the analysis:

- The treatment page did not improve conversion performance
- Negative uplift was observed
- Statistical testing did not support rollout confidence
- User engagement remained similar across both groups

## Final Recommendation

Retain the existing control page and conduct further experimentation before deploying the treatment version.

---

# Key Skills Demonstrated

- A/B Testing
- SQL Analytics
- Statistical Testing
- Data Cleaning
- Business Intelligence
- Power BI Dashboarding
- Data Modeling
- Data Visualization
- KPI Reporting
- Business Insight Generation

---

# Project Structure

```text
A-B-Testing-Analytics-Project/
│
├── data_raw/
│   ├── ab_test.csv
│   └── countries_ab.csv
│
├── screenshots/
│   │
│   ├── dashboard/
│   │   └── ab_test_powerbi_dashboard_overview.png
│   │
│   ├── modeling/
│   │   └── data_model_relationships.png
│   │
│   ├── powerbi/
│   │   ├── mysql_powerbi_connection.png
│   │   └── mysql_powerbi_connection_load.png
│   │
│   └── sql_analysis/
│       ├── ab_test_conversion_rate_analysis.png
│       ├── ab_test_country_conversion_analysis.png
│       ├── ab_test_engagement_analysis.png
│       ├── ab_test_page_performance_analysis.png
│       ├── ab_test_uplift_analysis.png
│       └── ab_test_statistical_significance.png
│
├── ab_test.ipynb
├── fintech_analytics.pbix
├── fintech_analytics_demo.mp4
└── README.md
```

---

# Author

## Dinesh Kumar Muthusamy

- GitHub: https://github.com/DineshKumar748
- LinkedIn: https://linkedin.com/in/dinesh-kumar-muthusamy-856399333/
