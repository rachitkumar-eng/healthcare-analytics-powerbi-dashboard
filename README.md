# Hospital Performance & Patient Experience Analytics Dashboard

## Project Overview

This project presents an end-to-end **Power BI dashboard** built to analyze hospital operations, staff performance, and patient experience using healthcare data.

The dashboard helps stakeholders identify:

* High-load departments
* Staff performance trends
* Treatment cost patterns
* Patient satisfaction levels

It transforms raw Excel data into **actionable business insights**.

---

##  Business Problem

Hospitals handle large volumes of patient and operational data but often lack clear visibility into:

* Department workload distribution
* Staff efficiency and contribution
* Impact of ER waiting time on patient satisfaction
* Cost trends across different regions and patient types

This dashboard solves these problems by providing a **centralized analytical view**.

---

##  Key Features

### 🔹 1. Hospital Overview

* Total Patients
* Total Revenue
* Average Treatment Cost
* Average ER Time
* Average Patient Rating

### 🔹 2. Department Performance

* Patient volume by department
* Revenue contribution by department
* Average ER time (efficiency indicator)
* Department-wise patient satisfaction

### 🔹 3. Staff / Doctor Performance

* Patients handled per staff
* Revenue generated per staff
* Average rating per staff
* Comparative performance analysis

### 🔹 4. Patient Experience Analysis

* Feedback distribution
* Rating trends
* Age group segmentation
* Patient type analysis (Inpatient vs Outpatient)
* Relationship between ER time and satisfaction

---

## Key Insights

* Departments with higher patient load often show increased ER time
* Longer ER time negatively impacts patient satisfaction
* Certain staff members contribute significantly more revenue
* Majority of patients fall into adult and middle-age categories
* Outpatients dominate overall hospital visits

---

##  Tools & Technologies Used

* **Power BI** → Dashboard development & visualization
* **Power Query** → Data cleaning & transformation
* **DAX (Data Analysis Expressions)** → KPI calculations
* **Microsoft Excel** → Data source
* **Data Modeling** → Relationships across multiple tables

---

##  Data Preparation Steps

* Cleaned and transformed raw Excel data using Power Query
* Standardized column names and data types
* Created derived columns:

  * Age Group
  * Year & Month
  * LOS Category (Length of Stay grouping)
* Removed null and inconsistent values
* Built relationships between:

  * Patient data
  * Staff details
  * Department data
  * Bed details

---

##  Key DAX Measures

```DAX
Total Patients = DISTINCTCOUNT('Detail data dataset'[Patient ID])

Total Revenue = SUM('Detail data dataset'[Treatment Cost])

Average ER Time = AVERAGE('Detail data dataset'[ER Time])

Average Rating = AVERAGE('Detail data dataset'[Rating])
```

---

## Project Structure

```
healthcare-analytics-powerbi-dashboard/
│
├── Hospital-Performance-Dashboard.pbix
├── Hospital_Health_Care_Management_Dataset.xlsx
├── README.md
└── screenshots/
    ├── overview.png
    ├── department-performance.png
    ├── staff-performance.png
    ├── patient-experience.png
    └── model-view.png
```

---

##  Dashboard Preview

[hospital-performance-patient-experience-analytics/overview.png](https://github.com/rachitkumar-eng/healthcare-analytics-powerbi-dashboard/blob/main/hospital-performance-patient-experience-analytics/overview.png?raw=true)
[hospital-performance-patient-experience-analytics/model-view.png](https://github.com/rachitkumar-eng/healthcare-analytics-powerbi-dashboard/blob/main/hospital-performance-patient-experience-analytics/model-view.png?raw=true)


---

##  How to Use

1. Download the `.pbix` file
2. Open in Power BI Desktop
3. Explore dashboard using slicers:

   * Year
   * Month
   * State
   * Department
   * Patient Type

---

##  Learning Outcomes

Through this project, I gained hands-on experience in:

* Data cleaning using Power Query
* Creating relationships and data models
* Writing DAX measures for KPIs
* Designing interactive dashboards
* Converting data into business insights

---

##  Inspiration

This project was inspired by a healthcare dashboard reference project and enhanced with:

* Improved data modeling
* Additional KPIs
* Multi-page analytical design
* Real-world business storytelling

---


---
