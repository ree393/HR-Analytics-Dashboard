# HR Analytics Dashboard – Employee Attrition Analysis

## 📌 Project Overview

This project presents an **HR Analytics Dashboard** built in **Power BI** to analyze employee attrition patterns and identify key factors contributing to workforce turnover.

Employee attrition is one of the most critical HR challenges, impacting productivity, recruitment costs, employee morale, and organizational growth. This dashboard helps HR teams and business leaders understand:

* Who is leaving the organization
* Which departments are experiencing the highest attrition
* How attrition varies across age groups and gender
* The relationship between employee tenure and turnover
* Job satisfaction trends across different job roles

The dashboard transforms raw HR data into actionable insights that support data-driven workforce planning and retention strategies.

---

## 🎯 Business Problem

Organizations often struggle to answer critical workforce questions such as:

* Why are employees leaving?
* Which employee segments are most at risk of attrition?
* Which departments require immediate retention efforts?
* How does tenure influence employee turnover?
* Is job satisfaction impacting employee retention?

This dashboard is designed to provide a centralized view of employee attrition metrics and help HR leaders proactively reduce turnover.

---

## 🔑 Key Performance Indicators (KPIs)

The dashboard tracks the following high-level HR metrics:

| KPI               | Description                          |
| ----------------- | ------------------------------------ |
| Overall Employees | Total workforce size                 |
| Attrition Count   | Total employees who left the company |
| Attrition Rate    | Percentage of employees who left     |
| Active Employees  | Current active workforce             |
| Average Age       | Average employee age                 |

---

## 📈 Dashboard Features

### 1. Overall Workforce Summary

Provides a quick overview of:

* Total Employees
* Attrition Count
* Attrition Rate
* Active Employees
* Average Age

---

### 2. Department-wise Attrition Analysis

Visualizes attrition across departments such as:

* Research & Development (R&D)
* Sales
* Human Resources (HR)

**Objective:** Identify departments with the highest employee turnover.

---

### 3. Employee Distribution by Age Group & Gender

Shows workforce composition across:

* Under 25
* 25–34
* 35–44
* 45–54
* Over 55

Further segmented by:

* Male
* Female

**Objective:** Understand workforce demographics and identify dominant employee groups.

---

### 4. Job Satisfaction Analysis

Displays job satisfaction ratings across various job roles:

Categories:

* Excellent
* Good
* Okay
* Poor

**Objective:** Identify roles where employee satisfaction may influence attrition.

---

### 5. Attrition by Working Years

Analyzes employee exits based on tenure ranges:

* 0–1 Years
* 1–2 Years
* 2–5 Years
* 5–10 Years
* 10–20 Years
* 20–30 Years
* 30–40 Years

**Objective:** Determine when employees are most likely to leave.

---

### 6. Attrition by Age Group and Gender

Provides a detailed breakdown of attrition patterns by:

* Age Group
* Gender

**Objective:** Detect high-risk employee segments for targeted retention strategies.

---

## 📌 Key Insights

### Department Attrition

* R&D contributes the highest share of attrition.
* Sales is the second-largest contributor.
* HR has relatively lower attrition.

### Age Group Trends

* Employees aged **25–34** experience the highest attrition.
* Attrition decreases with increasing age.

### Gender Analysis

* Male employees show higher attrition across most age groups.

### Tenure Analysis

* Employees with **5–20 years of experience** account for the highest attrition.
* Indicates potential challenges in retaining experienced talent.

### Job Satisfaction

* Several job roles display high counts in "Okay" and "Poor" satisfaction categories.
* Potential indicator of future attrition risk.

---

## 💼 Business Value

This dashboard enables organizations to:

* Reduce employee turnover
* Improve retention strategies
* Identify at-risk employee segments
* Enhance employee engagement initiatives
* Support workforce planning decisions
* Improve organizational performance through data-driven HR insights

---

## 🛠 Tools & Technologies

| Tool        | Purpose                                    |
| ----------- | ------------------------------------------ |
| Power BI    | Data Visualization & Dashboard Development |
| Excel       | Data Source                                |
| DAX         | Measures and KPI Calculations              |
| Power Query | Data Cleaning & Transformation             |

---

## 📂 Dataset Information

The dataset contains employee-related information including:

* Employee Demographics
* Department Information
* Age
* Gender
* Job Role
* Years at Company
* Attrition Status
* Job Satisfaction Ratings

---

## 📊 DAX Measures Used

### Attrition Count

```DAX
Attrition Count =
CALCULATE(
    COUNT(Employee[EmployeeID]),
    Employee[Attrition] = "Yes"
)
```

### Attrition Rate

```DAX
Attrition Rate =
DIVIDE(
    [Attrition Count],
    [Total Employees],
    0
)
```

### Active Employees

```DAX
Active Employees =
[Total Employees] - [Attrition Count]
```

### Total Employees

```DAX
Total Employees =
COUNT(Employee[EmployeeID])
```

### Average Age

```DAX
Average Age =
AVERAGE(Employee[Age])
```



## 👨‍💻 Author

Reeni

Data Analyst | Power BI Developer

### Connect With Me

LinkedIn: https://www.linkedin.com/in/reeni-32d/

GitHub:https://github.com/ree393?tab=repositories


