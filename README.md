
# Personal Health Charges Analysis Using Multiple Linear Regression

## Overview

This project analyzes personal health-related charges using a multiple linear regression model. The data includes factors like age, BMI, number of children, sex, region, and smoking status to predict medical charges. Additionally, interaction terms between key variables (e.g., smoking and BMI, smoking and age) were introduced to explore how lifestyle factors affect charges.

## Project Objectives

1. **Predicting Charges**: Build a linear regression model to predict medical charges based on demographic and health factors.
2. **Interaction Effects**: Investigate how interactions between variables (e.g., smoking and BMI) influence medical charges.
3. **Model Evaluation**: Assess the performance of the model using R-squared, adjusted R-squared, and significance levels (p-values).
4. **Diagnostic Analysis**: Validate model assumptions and diagnose issues through residual analysis.

## Dataset

The dataset contains the following features:
- **Age**: Age of the individual.
- **BMI**: Body mass index (a health indicator based on weight and height).
- **Children**: Number of children covered by the health insurance.
- **Sex**: Gender of the individual (Male/Female).
- **Region**: Geographic region (Northwest, Southeast, Southwest).
- **Smoker**: Whether the individual is a smoker.
- **Charges**: Total medical charges billed to the individual.

## Methodology

The project utilizes **Ordinary Least Squares (OLS) regression** to predict the `charges` variable. Interaction terms between variables such as **Age*Smoker** and **BMI*Smoker** were included to explore how these factors interact to influence charges.

Key metrics used to evaluate the model:
- **R-squared**: Proportion of variance in charges explained by the model.
- **Adjusted R-squared**: Adjusted for the number of predictors in the model.
- **P-values**: To determine the statistical significance of predictors.
- **Standard Errors**: To assess the precision of the estimated coefficients.

## Results

### Key Findings
- **Significant Predictors**:
   - **Age**: Older individuals tend to incur higher medical charges.
   - **Number of children**: The more children an individual has, the higher the medical charges.
   - **Smoking**: Smokers face significantly higher medical charges compared to non-smokers.
   - **Region**: Living in Southeast and Southwest regions is associated with lower medical charges.

### Interaction Effects:
- **Age * Smoker**: The positive impact of age on charges decreases for smokers.
- **BMI * Smoker**: The impact of BMI on charges increases for smokers, implying a synergistic effect between smoking and BMI.

### Model Performance:
- **R-squared**: 0.820, indicating that 82% of the variance in charges is explained by the model.
- **Adjusted R-squared**: 0.819, suggesting strong model fit.
  
### Diagnostics:
- The model passed the Durbin-Watson test, indicating no significant autocorrelation in residuals.
- Residuals show significant skewness and kurtosis, as indicated by the Omnibus and Jarque-Bera tests, suggesting potential non-normality.


## Research Support

### Smoking and Medical Costs:
- Studies consistently show that smokers incur significantly higher healthcare costs due to smoking-related illnesses. For example, research by **Lightwood and Glantz (1997)** highlights that smoking is associated with increased healthcare costs, particularly for chronic conditions like heart disease and cancer. This aligns with our findings, where smoking was a significant predictor of higher medical charges.

   - Lightwood, J., & Glantz, S. A. (1997). Short-term economic and health benefits of smoking cessation: Myocardial infarction and stroke. *Circulation*, 96(4), 1089-1096. [Link](https://pubmed.ncbi.nlm.nih.gov/)

### Age and Healthcare Costs:
- Research also supports the notion that healthcare costs increase with age. **Yang et al. (2003)** demonstrated that older individuals tend to have higher medical costs due to a greater prevalence of chronic diseases.

   - Yang, Z., Norton, E. C., & Stearns, S. C. (2003). Longevity and health care expenditures: The real reasons older people spend more. *The Journals of Gerontology Series B: Psychological Sciences and Social Sciences*, 58(1), S2-S10. [Link](https://academic.oup.com/)

### BMI and Healthcare Costs:
- The correlation between higher BMI and increased medical costs is well-documented. **Andreyeva et al. (2004)** found that higher BMI is associated with elevated healthcare expenditures, particularly in individuals with obesity-related conditions such as diabetes and cardiovascular disease.

   - Andreyeva, T., Sturm, R., & Ringel, J. S. (2004). Moderate and severe obesity have large differences in health care costs. *Obesity Research*, 12(12), 1936-1943. [Link](https://onlinelibrary.wiley.com/)

## Conclusion

This project explores how demographic and lifestyle factors impact healthcare costs using linear regression. Smoking status, age, and BMI were found to be significant predictors of charges, with interactions between smoking and BMI revealing important insights. Residual analysis suggested the need for potential model improvements, such as addressing non-normality in residuals.

By understanding the key factors driving medical costs, this analysis can aid policymakers and insurers in better predicting healthcare expenses and tailoring interventions to reduce costs for high-risk individuals.
