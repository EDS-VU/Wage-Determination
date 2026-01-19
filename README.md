# Wage Determinants Study

**Authors:** Imane el Bouzrouti, Máté Horgász, Simona Pavlovičová, Duy Phan  
**Date:** January 2025  
**Course:** Data Science Practical  

## Project Summary  
This project explores what truly drives wage differences and evaluates whether parental education is a major determinant of earnings. The goal is to quantify its impact and compare it with other factors such as individual education, cognitive ability, and work experience. We used multiple predictive models to understand which approach best captures wage variation.

## Problem Statement 
Economic theory suggests that parents’ education may influence a child’s future income, directly or indirectly through the child’s own education. However, it is unclear whether parental background remains important once individual characteristics are taken into account.

This project answers three core questions:
1. **Does parental education significantly explain wage differences?**
2. **Do individual factors (education, IQ, experience) matter more?**
3. **Which predictive method best models wage outcomes?**

## Approach  
1. **Data Preparation**  
   - Cleaned and prepared a dataset of 935 observations (wages, education, IQ, experience, demographics).
   - Applied a log‑transformation to wages to reduce skewness.  
   - Removed missing values and identified outliers.  
2. **Modeling Approaches**  
   - Built and compared three predictive models:
     - **Linear Regression (OLS)**
     - **K‑Nearest Neighbors (KNN)**
     - **Regression Trees**  
   - Conducted variable selection using correlation analysis and hypothesis testing.  
3. **Model Evaluation**  
   - Used train‑test split (80/20) and Mean Squared Error (MSE) to assess performance.
   - Performed statistical tests, including t‑tests, F‑tests, VIF, Breusch‑Pagan, and Jarque‑Bera, to validate model assumptions.  
   - Tested model assumptions: linearity, multicollinearity, homoskedasticity, and normality of residuals.  
4. **Simulation Study**  
   - Performed Monte Carlo simulations with heavy‑tailed residuals to test the robustness of OLS compared to KNN and regression trees.

## Results
- **Parental education matters, but its effect is modest:**: a one‑year increase in parental education corresponds to approximately **1.8% higher wages**.  
- Once individual education and IQ are included, parental influence decreases, indicating that personal characteristics explain more wage variation.  
- Other important predictors in the final model: individual education, IQ,  work experience, marital status, and urban residency.  
- **Linear Regression performed best**, achieving the lowest MSE(0.0908), outperforming KNN (0.123) and regression trees(0.117).  
- Simulation results show that OLS estimates remained **unbiased and consistent**, even when residuals are non‑normal.  

## Key Takeaways
- Parental background influences wages, but individual ability and education dominate.
- A simple linear model captures wage patterns better than more flexible non‑parametric methods.

## Skills:
- Data cleaning, statistical inference, model validation, and predictive modeling.
