# Create the README.md content based on the previous message
readme_content = """
# 📊 Palmoria Group – HR Analytics & Bonus Allocation (Power BI Capstone Project)

## 🔍 Project Overview

This project is part of the **DSA Data Analysis Capstone Project**, focused on identifying and addressing **gender-related issues**, **salary structures**, and **bonus allocations** at **Palmoria Group**, a manufacturing company based in Nigeria.

The analysis was done using **Power BI**, drawing insights from HR data across departments and regions. The goal is to uncover gaps in gender pay equality, policy compliance, and performance-based bonus systems, and offer actionable recommendations for management.

---

## 🧾 Dataset Description

- **Employee Data** (`Palmoria Group emp-data.csv`)
  - Fields: `Employee ID`, `Gender`, `Salary`, `Region`, `Department`, `Performance Rating`, etc.
- **Bonus Rules Data** (`Palmoria Group Bonus Rules.xlsx`)
  - Contains performance-based bonus multipliers for each department.

---

## ⚙️ Data Cleaning Process

1. Handled missing gender by assigning them as `"Undisclosed"`.
2. Removed records with `NULL` departments.
3. Removed employees without salary (assumed exited).
4. Ensured `Salary` column was numeric.
5. Merged bonus rule data using `Department` and `Performance Rating`.

---

## 📊 Analysis Metrics & DAX Logic

### ✅ Gender Distribution
```dax
Employee Count = COUNTROWS(EmployeeData)
