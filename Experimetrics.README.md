# 🎯 Gender and Fairness in the Ultimatum Game: An Experimetrics Analysis

## 📊 Project Overview
A comprehensive econometric analysis of gender differences in fairness preferences using experimental data from the Ultimatum Game. This project applies Maximum Likelihood Estimation, bootstrap resampling, and model comparison tests to understand how gender influences economic decision-making.

## 🎯 Research Questions
1. **Hypothesis 1:** Do fairness preferences differ by gender in economic bargaining?
2. **Hypothesis 2:** What are the gender-specific parameter estimates for fairness preferences?
3. **Hypothesis 3:** Is behavior better explained by fairness concerns or negative reciprocity?

## 📈 Experimental Design
- **Game:** Ultimatum Game (Proposer-Responder framework)
- **Sample:** Simulated experimental data with gender identifiers
- **Variables:**
  - Payoff allocations (`top_1`, `top_2`, `bottom_1`, `bottom_2`)
  - Binary choice variable (`d`): 1 = bottom allocation chosen, 0 = top allocation chosen
  - Gender indicator (`male`): 1 = male, 0 = female

## 🔬 Methodology

### **1. Econometric Framework**
- **Fehr-Schmidt Model:** Quantifies inequity aversion with parameters:
  - α (alpha): Sensitivity to disadvantageous inequality
  - β (beta): Sensitivity to advantageous inequality  
  - λ (lambda): Responsiveness to utility differences

### **2. Statistical Techniques**
- **Maximum Likelihood Estimation (MLE):** Parameter estimation with log-transformed positivity constraints
- **Bootstrap Resampling:** 100 iterations for robust standard errors (reduced for computational efficiency)
- **Regularized Hessian:** Numerical stabilization for variance-covariance matrices
- **Model Comparison:**
  - Vuong Test for non-nested models
  - Clarke Test for paired likelihood comparisons

### **3. Gender-Specific Analysis**
- Separate models for male and female proposers
- Direct parameter comparison with hypothesis testing
- Visualization of gender differences in fairness preferences

## 🛠️ Technical Implementation

### **Core R Packages**
```r
library(boot)        # Bootstrap resampling
library(DescTools)   # Clarke test
library(MASS)        # Multivariate normal sampling  
library(numDeriv)    # Numerical Hessian approximation
library(ggplot2)     # Data visualization
