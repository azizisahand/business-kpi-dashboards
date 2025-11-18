# Business KPI Dashboard Project (Looker & BigQuery)

  ![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white) ![Looker](https://img.shields.io/badge/Looker-4285F4?style=for-the-badge&logo=looker&logoColor=white) ![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?style=for-the-badge&logo=googlebigquery&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
## Overview
This repository provides comprehensive documentation for our critical **Business Key Performance Indicator (KPI)** dashboards. These dashboards are built using Looker on top of Google BigQuery, with a raw data source originating from a spreadsheet and a sales prediction model developed in Python. Given the temporary nature of some data within Google Cloud environments, this repository ensures all vital project assets, from raw data to final dashboards and analytical code, are preserved and easily accessible.

## Business Value & Purpose
This project aims to deliver clear, actionable insights into our business performance by presenting standardized KPI definitions and ensuring data consistency. It covers key areas such as revenue, profit, sales operations, and customer behavior, along with future sales predictions.

## Contents
- `dashboards/`: PDF exports of the primary Looker KPI dashboards.
- `bigquery_data_models/`: SQL queries used to retrieve and prepare data from BigQuery for various KPI calculations displayed in Looker.
- `raw_data/`: The original spreadsheet file(s) that serve as the initial source for some of the data loaded into BigQuery.
- `prediction_model/`: Google Colab Python code and documentation for the sales prediction model, including any generated outputs.

## Key Performance Indicators (KPIs)
The dashboards in this project visualize essential business KPIs, including but not limited to:
* **Revenue & Gross Profit:** Tracking overall financial performance.
* **Deal Value & Units per Deal:** Insights into sales transaction efficiency.
* **Order Methods:** Analysis of how customers place orders (e.g., Web, Telephone).
* **Geographical Performance:** Revenue breakdown by country.
* **Revenue Prediction & Churn Rate:** Forecasting future sales and identifying customer attrition.
* **Customer Lifetime Value (CLTV):** Identifying high-value customers.
* **Purchase Frequency & Lifespan:** Understanding customer engagement patterns.


## Data Sources & Flow
The core data for these dashboards originates from a `Data.xlsx` spreadsheet located in the `raw_data/` directory. This raw data was uploaded and transformed into persistent tables within Google BigQuery.

From BigQuery:
* Some Looker dashboards directly connect to these BigQuery tables.
* Other dashboard components retrieve data using specific SQL queries found in the `bigquery_data_models/` directory, which perform necessary transformations and aggregations for KPI calculation.
* The sales prediction model in the `prediction_model/` directory also utilizes data sourced from BigQuery.

## Dashboards
The main dashboard for this project is `Business-kpi-dashboard.pdf`. You can view it directly by clicking the link below:
* [Business KPI Dashboard](dashboards/Business-kpi-dashboard.pdf)


## Prediction Model
The `prediction_model/` directory contains the Python code `Sales_prediction.ipynb` used for forecasting future sales. This model employs the Holt-Winters prediction method.

## Setup and Usage
To explore this project:
1.  **View Dashboards:** Open the PDF in the `dashboards/` directory.
2.  **Understand KPIs:** Consult the markdown files in `kpi_definitions/` for detailed metric definitions.
3.  **Examine Data Preparation:** Review the SQL queries in `bigquery_data_models/` to see how data is prepared for KPIs.
4.  **Inspect Raw Data:** Access the initial spreadsheet data in `raw_data/`.
5.  **Explore Prediction Model:** Navigate to `prediction_model/` to view the Python code and its documentation.

## Contributors

This project was a collaborative effort. I would like to thank the following individuals for their valuable contributions:

*  [Carlos Montefusco](https://github.com/camontefusco/)
*  [Victoria Vasilieva](https://github.com/victoria-vasilieva)
*  [Olaf Bulas](https://github.com/Cebulva)

## 🤝 Contact

For any questions or feedback, feel free to reach out:

<p align="center">
  <a href="https://www.linkedin.com/in/sahandazizi/">
    <img 
      src="https://user-images.githubusercontent.com/74038190/235294012-0a55e343-37ad-4b0f-924f-c8431d9d2483.gif" 
      alt="LinkedIn"
      width="60"
    >
  </a>
  &nbsp;&nbsp;

  <a href="https://github.com/azizisahand">
    <img 
      src="https://user-images.githubusercontent.com/74038190/212257468-1e9a91f1-b626-4baa-b15d-5c385dfa7ed2.gif"
      alt="GitHub"
      width="50"
    >
  </a>
</p>
