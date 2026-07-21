# Bike Sales Excel Dashboard

## Project Overview

This project demonstrates an end-to-end data analysis workflow using Microsoft Excel. The objective is to analyze customer demographics and purchasing behavior to identify factors influencing bike purchases.

The project covers the complete analytics process, including data cleaning, feature engineering, pivot table analysis, data visualization, and dashboard development.

---

## Dataset Summary

|      Metric      |Value|
|------------------|-----|
| Total Records    |1,000|
| Total Features   |  13 |
| Missing Values   |  0  |
| Duplicate Records|  0  |
| Dashboard Charts |  3  |
| Pivot Tables     |  3  |

### Dataset Features

- ID
- Marital Status
- Gender
- Income
- Children
- Education
- Occupation
- Home Owner
- Cars
- Commute Distance
- Region
- Age
- Purchased Bike

---

## Tools Used

- Microsoft Excel
- Pivot Tables
- Pivot Charts
- Excel Dashboard
- Find & Replace
- IF Statements

---

## Project Workflow

### 1. Data Preparation

The original dataset consists of 1,000 customer records containing demographic and purchasing information.

To preserve the integrity of the raw data, a duplicate worksheet was created before performing any transformations.

### Dataset Preview

The image below shows a sample of the first few rows from the original dataset.

![Raw Dataset](images/raw_data.png)

---

### 2. Data Cleaning

Several data cleaning steps were performed:

- Created a duplicate worksheet to avoid modifying the original data.
- Standardized categorical values using Find & Replace:
  - M → Married
  - S → Single
- Verified data consistency across all columns.
- Checked for missing and duplicate records.

### Cleaned Dataset

![Cleaned Dataset](images/cleaned_data.png)

---

### 3. Feature Engineering

A new column called **Age Brackets** was created using Excel's IF function to categorize customers into age groups.

```excel
=IF(L5>54,"Old",
   IF(L5>=31,"Middle Age",
      IF(L5<31,"Adolescent","Invalid")))
```

Age categories:

| Age Range | Category |
|----------|----------|
| <31 | Adolescent |
| 31–54 | Middle Age |
| >54 | Old |

This additional feature allows for easier analysis of purchasing patterns by age group.

---

### 4. Pivot Table Analysis

Pivot Tables were created to summarize and analyze customer behavior.

#### Analysis Performed:

- Average Income by Gender and Purchase Status
- Customer Count by Commute Distance
- Customer Count by Age Bracket

### Pivot Table Preview

![Pivot Tables](images/pivot_tables.png)

---

### 5. Data Visualization

Three interactive charts were developed:

1. Average Income Per Purchase
2. Customer Commute Distance Analysis
3. Customer Age Bracket Distribution

These visualizations provide insights into customer demographics and purchasing trends.

---

### 6. Dashboard Development

An interactive dashboard was created using Pivot Charts and Slicers.

Dashboard filters include:

- Marital Status
- Region
- Education
- Occupation

### Dashboard Preview

![Dashboard](images/dashboard.png)

---

## Key Insights

- Customers aged 31–54 represent the largest customer segment.
- Male customers who purchased bikes have the highest average income.
- Customers with shorter commute distances are more likely to purchase bikes.
- Middle-aged customers account for the majority of bike purchases.
- Bike purchasing behavior varies across demographic groups such as occupation and education.

---

## Repository Structure

```text
excel-bike-sales-dashboard/
│
├── README.md
├── Bike Sales Dashboard.xlsx
│
└── images/
    ├── 1. raw_data.png
    ├── 2. cleaned_data.png
    ├── 3. pivot_income.png
    ├── 4. pivot_commute.png
    ├── 5. pivot_age_brackets.png
    └── 6. dashboard.png
```

---

## Skills Demonstrated

- Data Cleaning
- Data Transformation
- Feature Engineering
- Pivot Table Analysis
- Data Visualization
- Dashboard Development
- Business Insights Generation
- Microsoft Excel

---

## Author

**Sean Kenneth Handoyo**

- GitHub: https://github.com/seankh06
- LinkedIn: (Add your LinkedIn profile here)
