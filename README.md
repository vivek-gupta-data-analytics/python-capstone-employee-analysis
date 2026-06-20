# python-capstone-employee-analysis
End-to-end data analysis project involving data cleaning, merging, transformation, and business analytics using Python.

# Employee Project Management Analysis

## Overview

This project is a Python-based data analysis solution developed using Pandas and NumPy. It focuses on managing employee, project, and seniority-level data while performing various data cleaning, transformation, and business-rule implementations.

The project demonstrates practical data manipulation techniques commonly used in real-world analytics and data engineering workflows.

---

## Objectives

The main objectives of this project are:

- Create and manage structured datasets using Pandas DataFrames.
- Handle missing values in project cost data.
- Clean and transform employee information.
- Merge multiple datasets into a unified view.
- Apply business rules for employee promotions and demotions.
- Calculate employee bonuses based on project performance.
- Analyze project costs at the employee level.
- Perform data filtering and reporting operations.

---

## Dataset Information

The project uses three datasets:

### Employee Dataset
Contains employee details such as:
- Employee ID
- Name
- Gender
- City
- Age

### Seniority Level Dataset
Contains:
- Designation Level
- Employee Designation Mapping

### Project Dataset
Contains:
- Project ID
- Employee ID
- Project Cost
- Project Status

---

## Project Workflow

### 1. DataFrame Creation
Created Employee, Seniority Level, and Project DataFrames and exported them as CSV files.

### 2. Missing Value Treatment
Handled missing values in the Project Cost column using the running average approach.

### 3. Data Cleaning
- Split employee names into First Name and Last Name.
- Removed the original Name column.

### 4. Data Integration
Merged all datasets into a single consolidated DataFrame for analysis.

### 5. Bonus Calculation
Calculated employee bonuses based on project completion status.

**Bonus Rule:**
- Employees receive 5% of the project cost as a bonus if the project status is "Finished".

### 6. Employee Demotion Logic
Implemented business rules to:
- Demote employees associated with failed projects.
- Remove employees whose designation levels exceed the allowed limits.

### 7. Data Transformation
- Added appropriate prefixes (Mr./Mrs.) to employee names.
- Removed the Gender column after transformation.

### 8. Employee Promotion Logic
Promoted employees above the specified age threshold by upgrading their designation level.

### 9. Project Cost Analysis
Generated a summary DataFrame containing:
- Employee ID
- Employee Name
- Total Project Cost

### 10. Data Filtering
Filtered employee records based on city names containing specific characters.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Jupyter Notebook

---

## Project Structure

```text
Employee-Project-Analysis/
│
├── Capstone_Project_Python.ipynb
├── README.md

```

---

## Installation

Clone the repository:

```bash
git clone <repository-url>
cd Employee-Project-Analysis
```

Install required libraries:

```bash
pip install -r requirements.txt
```

---

## Requirements

```text
pandas
numpy
```

---

## Learning Outcomes

Through this project, the following concepts are demonstrated:

- Data cleaning and preprocessing
- Handling missing values
- DataFrame manipulation
- Data merging and joining
- Business rule implementation
- Aggregation and analysis
- Data transformation using Pandas
- Real-world data processing workflows

---

## Conclusion

This project showcases the practical application of Python, Pandas, and NumPy for employee and project data management. It demonstrates how raw data can be transformed into meaningful insights through data cleaning, integration, analysis, and business-rule implementation.
