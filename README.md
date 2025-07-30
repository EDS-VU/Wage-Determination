# Wage Determinants Study

**Authors:** Imane el Bouzrouti, Máté Horgász, Simona Pavlovičová, Duy Phan  
**Date:** January 2025  
**Course:** Data Science Practical  

## Overview  
This project investigates the factors that explain differences in wages, with a focus on **parental education** as a potential key determinant. Using a dataset of 935 individuals, we analyze whether parental education alone drives wage differences or if other variables (such as individual education, IQ, work experience, and personal background) play a larger role.

## Methodology  
1. **Data Preparation**  
   - Collected wage, education, IQ, work experience, demographic, and family background variables.  
   - Transformed wages using the natural log (`lwage`) to correct skewness.  
   - Removed missing values and identified outliers.  
2. **Modeling Approaches**  
   - Built and compared three predictive methods:
     - **Linear Regression (OLS)**
     - **K‑Nearest Neighbors (KNN)**
     - **Regression Trees**  
   - Conducted variable selection using correlation analysis and hypothesis testing.  
3. **Model Evaluation**  
   - Used train‑test split (80/20) and Mean Squared Error (MSE) to assess performance.  
   - Tested model assumptions: linearity, multicollinearity, homoskedasticity, and normality of residuals.  
4. **Simulation Study**  
   - Performed Monte Carlo simulations with heavy‑tailed residuals to test the robustness of OLS compared to KNN and regression trees.

## Key Findings  
- **Parental education has a significant impact**: a one‑year increase in parental education is associated with approximately **1.8% higher wages**.  
- Its effect, however, **diminishes when individual education and IQ are included** in the model.  
- Other important predictors: work experience, marital status, and urban residency.  
- **Linear Regression outperformed KNN and regression trees**, achieving the lowest MSE (0.0908).  
- OLS estimates remained **unbiased and consistent**, even when residuals were non‑normal.  


