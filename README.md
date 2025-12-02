# Data Quality Analysis of the BC Major Projects Inventory (MPI)

This repository contains the work for my **COMP 331 – Data Warehousing and Data Mining** final project.  
The goal is to evaluate the data quality of the **British Columbia Major Projects Inventory (MPI)** dataset using core data quality dimensions and data warehousing concepts.

---

## 📊 Project Overview

- **Dataset:** Major Projects Inventory – Economic Points (Q1 2025 extract)  
- **Publisher:** Government of British Columbia  
- **Source (BC Data Catalogue):**  
  https://catalogue.data.gov.bc.ca/dataset/major-projects-inventory-economic-points  

The dataset includes information on major capital projects across B.C., such as:

- Project name and description  
- Estimated cost  
- Region and municipality  
- Environmental assessment stage  
- Key dates (start and completion)  
- Latitude and longitude  

This project focuses on three data quality dimensions:

- **Completeness**  
- **Validity**  
- **Consistency**

---

## 🧠 Objectives

1. Assess data completeness for key fields such as municipality, descriptions, dates, and cost.  
2. Evaluate validity of numeric, geographic, and temporal fields (e.g., cost ranges, coordinate bounds, date logic).  
3. Identify consistency issues such as duplicate records and inconsistent geographic information.  
4. Connect findings to **data warehousing concepts** (ETL quality checks, dimension conformance, business-rule validation).  
5. Provide practical recommendations for improving the quality of the MPI dataset.

---

## 📁 Repository Structure

```text
.
├── MPI_DataQualityAnalysis.ipynb      # Main analysis notebook (Google Colab/Jupyter)
├── data/
│   └── mpi_dataset_q1_2025.xlsx       # MPI Q1 2025 extract (if size allows), otherwise see source link
├── results/
│   ├── missing_values_summary.csv
│   ├── invalid_cost.csv
│   ├── invalid_latitude.csv
│   ├── invalid_longitude.csv
│   ├── invalid_dates_detailed.csv
│   ├── duplicates.csv
│   ├── missing_municipalities.csv
│   ├── cost_outliers.csv
│   ├── data_quality_dashboard.png
│   ├── geo_validation_map.png
│   ├── date_timeline_chart.png
│   ├── cost_boxplot.png
│   └── (other supporting outputs)
└── README.md
