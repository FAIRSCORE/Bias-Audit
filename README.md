# COMPAS Fairness Audit

This repository contains a comprehensive **bias audit and mitigation study** using the **COMPAS two-year recidivism dataset**. The project evaluates disparities in algorithmic predictions across racial groups and implements fairness interventions.

## Project Overview

The project focuses on:

- Building a **baseline logistic regression model** to predict recidivism.
- Evaluating **fairness metrics** across protected groups (`race_cat`):  
  - Positive Rate (PR)  
  - True Positive Rate (TPR)  
  - False Positive Rate (FPR)
- Implementing **bias mitigation techniques**:  
  - **Post-processing** using Fairlearn’s `ThresholdOptimizer` (Equalized Odds).  
  - **Weighted logistic regression** (optional) to adjust for imbalanced group representation.
- Conducting **statistical tests** (chi-square, two-proportion z-tests) to validate disparities.
- Creating **visualizations** to compare fairness metrics across groups.
- Providing **ethical analysis and dataset improvement recommendations**.

## Technologies Used

- Python 3.x  
- Jupyter Notebook  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Fairlearn  
- AI Fairness 360 (AIF360)

## Installation

### Step 1: Using pip
Open your **Anaconda Prompt** or **Jupyter terminal** and run the following commands **line by line**:

```bash
pip install aif360==0.7.0
pip install fairlearn==0.9.1
