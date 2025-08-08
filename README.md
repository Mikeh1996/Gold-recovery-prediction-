# Gold Recovery Prediction

## Inspiration
This project was driven by my curiosity to understand why different machine learning models perform differently and how to select the most effective one for a specific task. I was excited to dive deeper into model evaluation and learn how preprocessing and metrics influence results. This also aligned with my broader interest in developing better intuition for model selection, especially in contexts where precision and business impact matter.

## Problem Statement
The task involves predicting the final gold recovery rate at a mining plant. The dataset includes process parameters and output concentrations at various stages: raw feed, rougher concentrate, and final concentrate. The challenge is to accurately model the recovery process by training robust regression models that can predict two key targets:

- `rougher.output.recovery`
- `final.output.recovery`

The evaluation metric is **sMAPE** (Symmetric Mean Absolute Percentage Error), with a weighted average formula used to reflect the importance of both target variables.

## Project Goals
- Analyze and clean the raw industrial data
- Investigate how metal concentrations and particle sizes evolve during processing
- Handle missing values and outliers
- Compare multiple regression models using cross-validation
- Calculate sMAPE and select the best-performing model
- Interpret and communicate the results clearly

## Key Questions Explored
- How does the particle size distribution differ between training and test sets?
- Are there abnormal concentrations of metals that should be removed?
- Which model (e.g., Linear Regression, Random Forest, etc.) performs best with this dataset?
- How does data scaling impact model performance?
- How can cross-validation (e.g., KFold) improve model evaluation?
- What does sMAPE tell us about predictive performance compared to standard error metrics?

## What I Learned from This Project
This project was my first hands-on experience comparing multiple regression models and evaluating them using a custom metric (sMAPE). I gained key insights into:

- Why comparing models is exciting and essential for learning how different algorithms behave
- How **standard scaling** affects model training
- How to use **KFold cross-validation** for more reliable performance estimation
- How to identify and handle **anomalies** in real-world industrial data
- The unique value of using **custom evaluation metrics** like sMAPE over traditional ones

## How to Run the Project Locally

1. Clone the repository:
```bash
git clone https://github.com/YOUR-USERNAME/gold-recovery-prediction.git
cd gold-recovery-prediction
