Employee Attrition Analysis Dashboard (Power BI)

## Project Overview

This Power BI project focuses on **analyzing employee attrition** — the rate at which employees leave an organization. The goal is to identify key factors influencing attrition and provide data-driven insights to help HR teams make better retention strategies.

## Objective

To design an **interactive Power BI dashboard** that visualizes employee attrition patterns based on various factors such as:

* Job Role
* Age Group
* Gender
* Department
* Education Field
* Years at Company
* Monthly Income
* Marital Status

## ⚙️ Key Insights & Metrics

The dashboard highlights:

* **Attrition Count:** Total number of employees who left the company.
* **Attrition Rate (%):** Percentage of employees who left compared to the total workforce.
* **Average Monthly Income:** Comparison between employees who stayed vs. those who left.
* **Average Age & Years at Company:** To understand experience and age distribution of attrition cases.
* **Attrition by Job Role / Department:** Identifies departments or roles with the highest attrition.
* **Demographic Analysis:** Gender and marital status breakdown of attrition.

## 📈 Tools & Technologies

* **Power BI Desktop:** For data visualization and dashboard creation
* **Data Cleaning:** Performed using Power Query
* **DAX Measures:** Used for calculating KPIs such as Attrition Rate, Average Age, and Income

## 🧮 DAX Measures Used

* **Attrition Count:**
  `Attrition Count = CALCULATE(COUNT(Employee[Attrition]), Employee[Attrition] = "Yes")`

* **Total Employees:**
  `Total Employees = COUNT(Employee[EmployeeNumber])`

* **Attrition Rate (%):**
  `Attrition Rate = DIVIDE([Attrition Count], [Total Employees], 0) * 100`

* **Average Monthly Income / Age / Years at Company:**
  `AVERAGE(Employee[MonthlyIncome])`, etc.

Insights Summary

* Higher attrition observed in **Sales and HR** departments.
* Employees with **1–3 years** at the company have higher turnover.
* **Lower-income groups** tend to leave more frequently.
* **Younger employees** (aged 25–35) show higher attrition tendencies.

Learning Outcomes

From this project, I learned how to:

* Clean and transform HR data using Power Query.
* Create KPIs and DAX measures for HR metrics.
* Build interactive dashboards with slicers and filters.
* Present insights clearly using visuals such as bar charts, pie charts, and stacked visuals.

Acknowledgment

This project was completed under the guidance of **Harshit Bhatia**, during a Power BI workshop where I learned data visualization techniques and dashboard storytelling.

---

**📁 Repository Contains:**

* Power BI `.pbix` file
* IBM attrition dataset
* Screenshots of the dashboard
* README file (this one)
