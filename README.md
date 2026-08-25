# Healthcare Patient & Financial Analysis Dashboard

## Dashboard Overview

This project presents an interactive **Healthcare Analytics Dashboard** developed to analyze patient admissions, hospital operations, clinical patterns, and treatment costs.

The project follows an end-to-end analytics workflow, starting with data exploration and validation using **PostgreSQL** and transforming the data into interactive dashboards using **Microsoft Excel, Power Query, PivotTables, PivotCharts, and Data Model relationships**.

The dashboard is designed to help stakeholders understand:

* Patient and admission trends
* Patient distribution across age groups and wards
* Hospital-wise treatment costs
* Readmission patterns
* Insurance and BPL patient distribution
* Admission and discharge patterns
* Treatment cost across insurance types
* Cost categories and billing patterns
* Government subsidy and patient out-of-pocket contribution

The report consists of two dashboard sheets:

* **Dashboard 1 – Hospital Overview**
* **Dashboard 2 – Patient & Financial Analysis**

---

# 🎯 Project Objective

The objective of this project is to analyze healthcare data and create a business-oriented dashboard that provides meaningful insights into **hospital operations, patient demographics, admissions, readmissions, and healthcare costs**.

The dashboard helps answer questions such as:

* How many patients and admissions are recorded?
* How are patients distributed across different age groups?
* Which wards have the highest number of patients?
* How do admissions change throughout the year?
* What is the difference between 7-day and 30-day readmission rates?
* Which hospitals have the highest average treatment cost?
* How are patients distributed across different insurance types?
* What is the average treatment cost for different insurance types?
* What percentage of treatment costs is covered through government subsidy?
* What percentage is paid out-of-pocket by patients?
* How are admissions distributed across different admission and discharge types?
* Which cost categories contribute to the highest number of bills?

---

# 🛠️ Tools & Technologies Used

* **PostgreSQL** – Data exploration, SQL queries, validation, and understanding relationships
* **Microsoft Excel** – Dashboard development and analysis
* **Power Query** – Data transformation and preparation
* **PivotTables** – Data aggregation and analysis
* **PivotCharts** – Interactive visualizations
* **Excel Data Model** – Relationships between multiple tables
* **Slicers** – Interactive filtering
* **GitHub** – Project documentation and version control

---

# 📊 Dataset

The healthcare dataset contains multiple related tables covering different aspects of hospital and patient information.

The major data areas include:

* Patient information
* Hospital information
* Admission records
* Diagnosis information
* Billing and treatment costs

The data contains fields related to:

* Patient demographics
* Age
* Hospital
* State and hospital tier
* Admission date
* Admission type
* Ward type
* Diagnosis category
* Diagnosis rank
* Discharge type
* Insurance type
* BPL card status
* Teaching hospital status
* Length of stay
* Number of procedures
* Total treatment cost
* Government subsidy
* Out-of-pocket expenditure
* Cost category
* Readmission indicators

---

# 🔄 Project Workflow

### Step 1 – Data Exploration

The healthcare dataset was initially explored to understand the available tables, columns, relationships, and business context.

### Step 2 – SQL Analysis

The data was loaded into **PostgreSQL** and SQL queries were used to:

* Explore the data
* Verify relationships
* Check patient and admission records
* Analyze hospital-level metrics
* Understand diagnosis and billing information
* Validate important business calculations

### Step 3 – Data Preparation

The required data was brought into Excel and prepared using **Power Query**.

Data preparation included:

* Checking data types
* Handling inconsistent values
* Creating useful analytical fields
* Creating age groups for patient distribution analysis
* Preparing fields required for dashboard analysis

### Step 4 – Data Modeling

Relationships between the different healthcare tables were established using common identifiers such as:

* Hospital ID
* Admission ID
* Patient ID

### Step 5 – PivotTable Analysis

PivotTables were created to calculate important metrics such as:

* Patient counts
* Admission counts
* Average length of stay
* Average treatment cost
* Hospital-wise average cost
* Insurance-wise patient distribution
* Admission and discharge distribution

### Step 6 – Dashboard Development

Two interactive dashboard sheets were designed using:

* KPI Cards
* Bar Charts
* Column Charts
* Donut Charts
* Line Charts
* Slicers

### Step 7 – Interactive Filtering

Interactive slicers were added to allow users to filter the dashboard based on:

* State
* Admission Year
* Tier
* Diagnosis Category
* Teaching Hospital Status

---

# 📌 Dashboard 1 – Hospital Overview

The first dashboard focuses on **hospital operations, patient demographics, admissions, and readmission performance**.

## KPIs

* **Total Patients**
* **Total Admissions**
* **Total Hospitals**
* **Average Length of Stay**
* **Total Beds**

## Visualizations

### 1. Total Patients by Age Group

Shows the distribution of patients across different age groups such as:

* Children
* Young Adults
* Adolescents
* Adults
* Senior
* Middle-aged

This helps identify the major patient demographic groups.

### 2. Average LOS by Admission Type

Compares the average **Length of Stay (LOS)** across different admission types:

* OPD
* Elective
* Emergency

### 3. Top 10 Hospitals by Average Cost

Identifies hospitals with the highest average treatment cost per admission.

### 4. Total Patients by Ward Type

Shows patient distribution across different hospital wards such as:

* General
* ICU
* HDU
* NICU

### 5. Monthly Admission Trend

Displays the number of admissions across different months to identify admission patterns and fluctuations throughout the year.

### 6. 7-Day vs 30-Day Readmission Rate

Compares short-term and 30-day readmission rates to understand patient readmission patterns.

---

# 💰 Dashboard 2 – Patient & Financial Analysis

The second dashboard focuses on **patient characteristics, insurance, billing, treatment costs, and financial burden**.

## KPIs

* **Total Treatment Cost**
* **Average Cost per Admission**
* **Government Subsidy %**
* **Out-of-Pocket %**

## Visualizations

### 1. Total Patients by Insurance Type

Shows the distribution of patients across different insurance categories such as:

* ESI
* Private
* None
* Ayushman

### 2. BPL Card Distribution

Shows the distribution of patients based on BPL card status.

### 3. Total Patients by Ward Type

Compares patient counts across different hospital ward types.

### 4. Average Cost by Insurance Type

Compares the average treatment cost across different insurance categories.

### 5. Discharge Type Distribution

Shows how admissions are distributed across different discharge outcomes such as:

* Recovered
* LAMA
* Expired
* Referred

### 6. Total Bills by Cost Category

Shows the distribution of billing records across different cost categories such as:

* Pharmacy
* Procedure
* Room
* Lab

### 7. Total Admissions by Admission Type

Compares the number of admissions across:

* OPD
* Elective
* Emergency

---

# 🎛️ Dashboard Filters

Interactive slicers are provided to allow users to dynamically explore the dashboard.

### Available Filters

* **State**
* **Admission Year**
* **Tier**
* **Diagnosis Category**
* **Teaching Status**

These filters allow stakeholders to perform focused analysis, such as comparing patient and financial performance across different states, hospital tiers, diagnosis categories, and teaching/non-teaching hospitals.

---

# 📈 Key Metrics & Calculations

Some important calculations used in the project include:

### Total Patients

Count of unique patients in the healthcare dataset.

### Total Admissions

Total number of admission records.

### Average Length of Stay

Average number of days patients stayed in the hospital.

### Average Cost per Admission

Average treatment cost associated with an admission.

### Government Subsidy %

Government subsidy as a percentage of total treatment cost.

```text
Government Subsidy % =
Total Government Subsidy / Total Treatment Cost
```

### Out-of-Pocket %

Patient-paid treatment cost as a percentage of total treatment cost.

```text
Out-of-Pocket % =
Total Out-of-Pocket Cost / Total Treatment Cost
```

Together, these metrics help understand the distribution of the financial burden between government support and patients.

---

# 🔍 Key Business Insights

## Hospital & Patient Analysis

* Identified the distribution of patients across different age groups.
* Compared patient volumes across different hospital ward types.
* Analyzed monthly admission trends.
* Compared admission patterns across OPD, elective, and emergency admissions.
* Identified hospitals with the highest average treatment costs.
* Compared 7-day and 30-day readmission rates.

## Patient & Financial Analysis

* Analyzed patient distribution across different insurance types.
* Compared average treatment costs across insurance categories.
* Examined BPL card distribution.
* Analyzed discharge outcomes.
* Compared billing records across different cost categories.
* Measured the share of treatment costs covered through government subsidies.
* Measured the financial contribution paid out-of-pocket by patients.

---

# ⭐ Dashboard Features

* Interactive KPI Cards
* Dynamic Slicers
* Multi-sheet Dashboard
* Excel Data Model
* Power Query Transformations
* PivotTable Analysis
* PivotChart Visualizations
* Cross-filtered Dashboard Analysis
* Business-oriented Data Visualization
* Patient Demographic Analysis
* Hospital Performance Analysis
* Financial Analysis
* Readmission Analysis

---

# 💡 Analytical Highlights

The dashboard combines **operational and financial analysis** in one solution.

### Hospital Overview

Focuses on:

> **Who are the patients? → Where are they treated? → How many admissions occur? → How long do patients stay? → What are the readmission patterns?**

### Patient & Financial Analysis

Focuses on:

> **Who pays for treatment? → What does treatment cost? → How does insurance affect cost? → How much is subsidized? → How much is paid out-of-pocket?**

This separation makes the dashboard easier to navigate and allows different business questions to be analyzed independently.

---

# 🚀 Future Improvements

Potential future enhancements include:

* Connecting the dashboard to a live database
* Automating data refresh
* Adding year-over-year comparisons
* Adding hospital performance benchmarking
* Adding advanced readmission analysis
* Adding predictive analysis for admissions
* Adding treatment cost forecasting
* Publishing the dashboard through a BI platform
* Adding drill-down and drill-through analysis

---


# 🖼️ Dashboard Preview

## Hospital Overview Dashboard

This dashboard provides an overview of patient demographics, hospital operations, admission trends, hospital costs, ward utilization, and readmission performance.

```markdown
![Hospital Overview Dashboard](Images/hospital_overview.png)
```

---

## Patient & Financial Analysis Dashboard

This dashboard focuses on insurance coverage, patient characteristics, treatment costs, billing categories, discharge outcomes, government subsidy, and out-of-pocket expenditure.

```markdown
![Patient & Financial Analysis Dashboard](Images/patient_financial_analysis.png)
```

---

# 📌 Project Outcome

This project demonstrates a complete healthcare analytics workflow, from **data exploration and SQL analysis in PostgreSQL to data transformation, modeling, and interactive dashboard development in Excel**.

The final dashboard provides a consolidated view of:

* Hospital performance
* Patient demographics
* Admission trends
* Ward utilization
* Readmission patterns
* Insurance distribution
* Treatment costs
* Billing categories
* Government subsidy
* Patient out-of-pocket expenditure

The project demonstrates practical skills in **SQL, PostgreSQL, Excel, Power Query, data modeling, PivotTables, PivotCharts, KPI development, data visualization, and business analytics**.

---

