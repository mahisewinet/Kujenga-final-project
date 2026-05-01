# Bunna Bank HR Data — Final Project

**Student:** Mahlet Sewinet Admasu  
**Country:** Ethiopia  
**Course:** Kujenga  
**GitHub:** https://github.com/mahisewinet/Kujenga-final-project

---

## Research Question

What factors predict the current monthly salary of Bunna Bank employees, and does gender play a significant role after controlling for other variables?

---

## About the Data

The dataset comes from Bunna Bank HR records and contains information on a random sample of employees. It includes the following variables:

| Variable | Description |
|---|---|
| `Sex` | Gender of the employee (male or female) |
| `YearsOfEducation` | Total years of formal education completed |
| `CurrentMonthlySalary` | Current monthly salary in ETB (target variable) |
| `StartingMonthlySalary` | Monthly salary at the time of hiring |
| `MonthsAtBunnaBank` | Length of service at Bunna Bank, in months |
| `PriorExperienceMonths` | Work experience before joining Bunna Bank, in months |

The data files are located in the `data/` folder.

---

## Project Structure

```
Mahlet Kujenga final project/
├── mahlet_ethiopia_final_project.ipynb   # Main analysis notebook
├── README.md                             # This file
└── data/
    ├── Bunna_bank_HR_data.csv            # Main dataset
    └── Bunna_bank_HR_data_dictionary.csv # Variable descriptions
```

---

## Analysis Overview

The notebook is organized into 8 sections:

1. **Data Loading & Inspection** — loading the dataset and understanding its structure
2. **Data Cleaning** — checking for missing values, duplicates, outliers, and encoding variables
3. **Exploratory Data Analysis** — visualizing salary distributions by gender
4. **T-Test** — testing whether the salary difference between male and female employees is statistically significant
5. **Correlation Analysis (Uni Variable)** — examining how each factor individually relates to current salary
6. **Linear Regression (Multi Variable)** — building a model that predicts salary using all factors together
7. **Discussion** — comparing findings across sections
8. **Conclusion** — summarizing the answers and limitations

---

## How to Run

1. Clone this repository
2. Make sure you have the required libraries installed:
   ```
   pip install pandas numpy matplotlib seaborn scipy statsmodels
   ```
3. Open `mahlet_ethiopia_final_project.ipynb` in Jupyter Notebook or JupyterLab
4. Run all cells from top to bottom

---

## Key Findings

- `StartingMonthlySalary` is by far the strongest predictor of current salary
- All five factors are statistically significant when combined in the regression model
- A statistically significant gender pay gap exists even after controlling for education, experience, and starting salary
