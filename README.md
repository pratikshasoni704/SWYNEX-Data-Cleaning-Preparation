# Netflix Customer Churn Analysis

## Project Overview

This project focuses on analyzing Netflix customer churn data through a complete data analytics workflow.

The project was completed as part of a data analytics internship assignment and covers three major stages:

1. **Data Cleaning & Preparation**
2. **Exploratory Data Analysis (EDA)**
3. **Interactive Dashboard & Business Insights**

The objective is to transform raw customer data into meaningful insights that can help understand customer churn patterns and identify areas where customer retention can potentially be improved.

---

## Project Objectives

The main objectives of this project are to:

- Clean and prepare the customer churn dataset.
- Identify missing values, duplicate records, inconsistent values, and data quality issues.
- Perform exploratory data analysis to understand customer behavior.
- Analyze churn across different customer segments.
- Create an interactive Power BI dashboard.
- Identify important business insights from the analysis.
- Present the findings in a clear and understandable format.

---

## Dataset

The project uses a Netflix customer churn dataset containing information about customer demographics, subscription behavior, viewing activity, payment methods, and churn status.

### Dataset Size

- **Rows:** 5,000
- **Columns:** 14

### Main Columns

| Column | Description |
|---|---|
| `customer_id` | Unique customer identifier |
| `age` | Customer age |
| `gender` | Customer gender |
| `subscription_type` | Customer subscription plan |
| `watch_hours` | Total watch hours |
| `last_login_days` | Number of days since last login |
| `region` | Customer geographical region |
| `device` | Primary device used |
| `monthly_fee` | Monthly subscription fee |
| `churned` | Customer churn status |
| `payment_method` | Customer payment method |
| `number_of_profiles` | Number of profiles associated with the account |
| `avg_watch_time_per_day` | Average daily watch time |
| `favorite_genre` | Customer's preferred content genre |

---

# Project Workflow

The project follows a standard data analytics workflow:

```text
Raw Dataset
     ↓
Data Cleaning & Preparation
     ↓
Exploratory Data Analysis
     ↓
Data Visualization
     ↓
Power BI Dashboard
     ↓
Business Insights & Recommendations
```

---

# Task 1 — Data Cleaning & Preparation

### Notebook

```text
notebook/task1_data_cleaning.ipynb
```

### Dataset

Raw dataset:

```text
data/raw/netflix_customer_churn.csv
```

Cleaned dataset:

```text
data/processed/netflix_customer_churn_cleaned.csv
```

### Cleaning Process

The dataset was inspected and prepared for analysis by checking:

- Missing values
- Duplicate records
- Data types
- Categorical values
- Numerical values
- Churn distribution
- Basic data quality issues

### Initial Data Quality Findings

- Dataset contains **5,000 customer records**.
- Dataset contains **14 columns**.
- No missing values were identified in the initial null-value check.
- No duplicate records were identified during the duplicate check.
- Numerical and categorical columns were reviewed for analysis readiness.

The cleaned dataset was saved separately so that the original raw dataset remained unchanged.

---

# Task 2 — Exploratory Data Analysis

### Notebook

```text
notebook/task2_exploratory_data_analysis.ipynb
```

The second stage of the project focuses on understanding customer behavior and identifying patterns related to churn.

### Analysis Areas

The analysis explored:

- Customer demographics
- Subscription types
- Watch hours
- Last login activity
- Monthly fees
- Number of profiles
- Average daily watch time
- Regions
- Devices
- Payment methods
- Favorite genres
- Customer churn

### Churn Distribution

The dataset contains:

| Churn Status | Customers |
|---|---:|
| Churned | 2,515 |
| Not Churned | 2,485 |
| **Total** | **5,000** |

The overall churn rate is approximately **50.3%**.

This indicates that customer churn is a significant business issue within the analyzed dataset and requires further investigation.

---

# Task 3 — Power BI Dashboard

The third stage converts the analysis into an interactive business dashboard using Microsoft Power BI.

### Dashboard File

```text
task_3_dashboard/netflix_customer_churn_dashboard.pbix
```

### Dashboard Screenshot

```text
task_3_dashboard/dashboard_screenshot.png
```

## Dashboard Components

The dashboard contains KPI cards and multiple visualizations designed to provide a quick overview of customer churn.

The dashboard analyzes churn across dimensions such as:

- Overall customer churn
- Subscription type
- Region
- Device
- Customer segments
- Other customer behavior metrics

### Key Dashboard Features

- KPI cards for important metrics
- Customer churn distribution
- Subscription-level churn analysis
- Region-level churn analysis
- Device-level churn analysis
- Interactive visual analysis
- Business-focused presentation of customer churn

---

# Key Business Insights

Based on the exploratory analysis and Power BI dashboard, several important patterns were identified.

### 1. Customer churn is significant

The dataset contains approximately **50.3% churned customers**, showing that customer retention is an important area for business attention.

### 2. Subscription type affects churn

Churn varies across subscription types. Comparing subscription-level churn can help identify which plans may require better retention strategies.

### 3. Regional differences exist

Customer churn is not distributed equally across all regions. Some regions show higher churn volumes than others.

This indicates that customer retention strategies may need to consider regional behavior and preferences.

### 4. Device usage shows different churn patterns

The dashboard shows noticeable churn volumes among customers using different devices, including **mobile, laptop, and TV**.

Device-level analysis can help identify whether customer experience or engagement differs across platforms.

### 5. Customer engagement is important

Variables such as watch hours, last login activity, and average watch time provide useful indicators of customer engagement.

Customers with lower engagement may represent potential retention-risk segments.

---

# Business Recommendations

Based on the analysis, the following actions could help improve customer retention:

### 1. Identify high-risk customers

Use customer activity indicators such as:

- Last login days
- Watch hours
- Average daily watch time
- Subscription type

to identify customers who may be at higher risk of churn.

### 2. Improve retention strategies by subscription plan

Analyze high-churn subscription segments and consider:

- Personalized offers
- Plan upgrades or downgrades
- Targeted retention campaigns
- Improved plan value

### 3. Develop region-specific strategies

Regions with higher churn should be analyzed separately to understand differences in:

- Customer preferences
- Content consumption
- Pricing
- Engagement
- Payment behavior

### 4. Improve engagement

Customers with low viewing activity could receive personalized recommendations and engagement campaigns to encourage continued platform usage.

### 5. Monitor churn continuously

The Power BI dashboard can be used as a reporting tool to monitor churn KPIs and compare customer segments over time.

---

# Tools & Technologies

The following tools were used in this project:

- **Python**
- **Pandas**
- **Jupyter Notebook**
- **Microsoft Power BI**
- **Git**
- **GitHub**

### Python Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn

---

# Project Structure

```text
SWYNEX-Data-Cleaning-Preparation/
│
├── data/
│   ├── raw/
│   │   └── netflix_customer_churn.csv
│   │
│   └── processed/
│       └── netflix_customer_churn_cleaned.csv
│
├── notebook/
│   ├── task1_data_cleaning.ipynb
│   └── task2_exploratory_data_analysis.ipynb
│
├── task_3_dashboard/
│   ├── dashboard_screenshot.png
│   └── netflix_customer_churn_dashboard.pbix
│
└── README.md
```

---

# How to Use This Project

### 1. Clone the repository

Clone this repository to your local machine.

### 2. Explore the dataset

The raw dataset is available in:

```text
data/raw/
```

The cleaned dataset is available in:

```text
data/processed/
```

### 3. Run the notebooks

Open the notebooks inside:

```text
notebook/
```

Run them using Jupyter Notebook or JupyterLab.

### 4. Explore the Power BI dashboard

Open:

```text
task_3_dashboard/netflix_customer_churn_dashboard.pbix
```

using Microsoft Power BI Desktop.

---

# Skills Demonstrated

This project demonstrates practical skills in:

- Data Cleaning
- Data Preparation
- Exploratory Data Analysis
- Data Visualization
- Customer Churn Analysis
- Business Intelligence
- KPI Analysis
- Business Insight Generation
- Dashboard Development
- Python for Data Analysis
- Power BI
- Git & GitHub

---

# Conclusion

This project demonstrates an end-to-end data analytics workflow, starting from a raw customer dataset and progressing through data cleaning, exploratory analysis, visualization, dashboard development, and business recommendations.

The analysis highlights customer churn patterns across subscription types, regions, devices, and engagement-related metrics.

The final Power BI dashboard provides a visual business interface that can be used to monitor churn and support data-driven customer retention decisions.

---

## Author

**Pratiksha Soni**

Data Analytics Project  
SWYNEX Internship Assignment