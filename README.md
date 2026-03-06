# AI Automation Risk Predictor

![Python](https://img.shields.io/badge/Python-3.14-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## Overview
This project explores the **AI-Powered Job Market Insights** dataset to predict the automation risk level of job roles in an AI-driven economy. Using a range of classification models, we analyze how factors such as industry, required skills, company size, salary, and AI adoption level contribute to whether a job is at **Low**, **Medium**, or **High** risk of automation.

> **Note:** The dataset used in this project is synthetic but realistic, designed to simulate modern job market dynamics.

## Research Questions
1. *Can we predict the automation risk level (Low / Medium / High) of a job role based on industry, company characteristics, required skills, and AI adoption level?*
2. *Which factor contributes the most to a job's automation risk?*

## Dataset
- **Name:** AI-Powered Job Market Insights
- **Source:** [Kaggle](https://www.kaggle.com/datasets/uom190346a/ai-powered-job-market-insights)
- **Size:** 500 job listings, 10 features
- **Target Variable:** `Automation_Risk` (Low / Medium / High)

## Project Pipeline
1. Data Loading
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Feature Engineering
5. Model Training & Evaluation
6. Interpretation & Conclusions

## Results

| Model | Accuracy | F1 Score |
|---|---|---|
| Logistic Regression | 0.32 | 0.29 |
| Decision Tree | 0.30 | 0.30 |
| **Random Forest** | **0.36** | **0.36** |

## Key Findings
- **Salary is the strongest predictor** of automation risk, followed by Industry and Required Skills
- Lower-paid jobs in routine-heavy industries are most at risk of automation
- Random Forest outperformed all other models on both Accuracy and F1-score
- Simple correlation analysis underestimated Salary's importance — highlighting the value of ML over statistical measures

## Project Structure
```
AI-Automation-Risk-Predictor/
│
├── data/
│   └── ai_job_market_insights.csv
├── notebooks/
│   └── ai_automation_risk.ipynb
├── requirements.txt
└── README.md
```

## Requirements
Install dependencies using:
pip install -r requirements.txt

## Dependencies
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Author
Made as a portfolio project for a BSc Computer Science degree.

## License
This project is licensed under the MIT License.
```

You'll also want to create a `requirements.txt` file in your project root with:
```
pandas
numpy
matplotlib
seaborn
scikit-learn