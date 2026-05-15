# 📊 HR Analytics Dashboard – Power BI Project

## 📌 Project Overview

This project is an Advanced HR Analytics Dashboard developed using:

- Power BI Desktop
- Microsoft Excel
- MySQL
- DAX (Data Analysis Expressions)

The objective of this project is to analyze employee attrition, workforce demographics, salary trends, job satisfaction, and employee retention patterns using interactive visualizations and business intelligence techniques.

The dashboard helps HR teams and management identify key factors affecting employee attrition and make data-driven decisions.

---

# 🚀 Project Features

## ✅ KPI Metrics

The dashboard includes the following KPIs:

- Total Employees
- Attrition Count
- Attrition Rate %
- Average Salary
- Average Age
- Average Years at Company
- Average Job Satisfaction

---

# 📊 Dashboard Visualizations

## 🔹 Attrition by Department
Analyzes which department has the highest employee attrition.

## 🔹 Attrition by Job Role
Displays employee attrition across different job roles.

## 🔹 Attrition by Age Group
Analyzes employee turnover based on age categories.

## 🔹 Salary vs Attrition
Scatter plot showing salary impact on attrition.

## 🔹 Overtime vs Attrition
Shows relationship between overtime and employee resignation.

## 🔹 Job Satisfaction Analysis
Visualizes employee satisfaction levels.

## 🔹 Attrition by Education Field
Analyzes attrition based on educational background.

## 🔹 Years at Company vs Attrition
Shows retention trends across employee experience levels.

## 🔹 Key Influencers Visual
AI-powered analysis identifying major factors affecting attrition.

## 🔹 Decomposition Tree
Advanced root cause analysis for attrition.

---

# 🛠️ Tools & Technologies Used

| Tool | Purpose |
|------|----------|
| Power BI Desktop | Dashboard Development |
| Excel | Data Cleaning & Preparation |
| MySQL | Database Management |
| DAX | KPI Calculations & Measures |

---

# 🧹 Data Cleaning Process

The following preprocessing steps were performed:

- Removed duplicate records
- Checked missing/null values
- Corrected data types
- Removed unnecessary columns
- Created calculated columns
- Verified data consistency

---

# 📌 Calculated Columns

## Attrition Flag

```DAX
Attrition Flag =
IF('Sheet1'[Attrition] = "Yes", 1, 0)
```

---

## Age Group

```DAX
Age Group =
SWITCH(
    TRUE(),
    'Sheet1'[Age] <= 25, "18-25",
    'Sheet1'[Age] <= 35, "26-35",
    'Sheet1'[Age] <= 45, "36-45",
    "45+"
)
```

---

# 📌 DAX Measures

## Total Employees

```DAX
Total Employees =
COUNT('Sheet1'[EmployeeNumber])
```

---

## Attrition Count

```DAX
Attrition Count =
SUM('Sheet1'[Attrition Flag])
```

---

## Attrition Rate

```DAX
Attrition Rate =
DIVIDE([Attrition Count], [Total Employees])
```

---

## Average Salary

```DAX
Avg Salary =
AVERAGE('Sheet1'[MonthlyIncome])
```

---

# 🎨 Dashboard Design

## Theme
- Dark Professional Theme
- Corporate HR Analytics Layout

## Color Palette

| Purpose | Color |
|----------|--------|
| Background | Dark Navy |
| Attrition | Red |
| Salary Metrics | Green |
| Neutral Charts | Blue |
| Satisfaction | Purple |

---

# 🚀 Advanced Features

## ✅ Drill Through
Allows navigation from summary visuals to employee-level details.

## ✅ Custom Tooltips
Displays additional employee insights on hover.

## ✅ Dynamic Titles
Dashboard titles change automatically based on selected filters.

## ✅ AI Visuals
Used Power BI Key Influencers and Decomposition Tree visuals.

## ✅ Interactive Slicers
Filters available for:
- Department
- Gender
- Job Role
- Education Field
- Marital Status

---

# 📂 Project Structure

```text
HR-Analytics-Dashboard/
│
├── Dataset/
│   └── HR_Analytics_Dashboard_PBI.xlsx
│
├── PowerBI/
│   └── HR_Analytics_Dashboard.pbix
│
├── Screenshots/
│   └── Dashboard_Main.png
│
├── SQL/
│   └── hr_analytics_queries.sql
│
└── README.md
```

---

# 📌 Business Insights

The dashboard identified several important HR insights:

- Employees working overtime are more likely to leave.
- Lower salary employees show higher attrition.
- Employees aged 26–35 have the highest attrition.
- Research & Development department has maximum attrition.
- Low job satisfaction contributes to employee turnover.

---

# 📷 Dashboard Preview

Add your dashboard screenshot here.

```md
![Dashboard Preview](Screenshots/Dashboard_Main.png)
```

---

# 📈 Skills Demonstrated

- Data Cleaning
- Data Modeling
- DAX Calculations
- Dashboard Design
- Business Intelligence
- HR Analytics
- SQL Queries
- Data Visualization
- Power BI Advanced Features

---

# 🔗 GitHub Repository Setup

## Upload the following files:

- Power BI `.pbix` file
- Dataset `.xlsx`
- Dashboard screenshots
- SQL query file
- README.md

---

# 🎯 Project Outcome

This project demonstrates how HR analytics can help organizations:

- Reduce employee attrition
- Improve workforce planning
- Increase employee satisfaction
- Identify key attrition drivers
- Support data-driven HR decisions

---

# 👨‍💻 Author

Your Name  
Data Analyst | Power BI Developer | SQL Enthusiast

---

# ⭐ If You Like This Project

Please give this repository a ⭐ on GitHub.
