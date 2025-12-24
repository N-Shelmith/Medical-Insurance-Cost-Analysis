# Medical Insurance Cost Prediction (Linear Regression)

## Overview
This project applies a linear regression model to predict individual medical insurance charges using demographic and health-related features. The goal is to identify key cost drivers and assess how well a simple, interpretable model can explain variation in insurance costs.

The analysis prioritizes clarity, interpretability and business relevance over model complexity.

---

## Dataset
The dataset contains 1,338 records with the following variables:

- **age** – age of the beneficiary  
- **sex** – gender of the beneficiary  
- **bmi** – body mass index  
- **children** – number of dependents covered  
- **smoker** – smoking status  
- **region** – residential region in the US  
- **charges** – medical insurance cost (target variable)  

---

## Approach
1. Conducted quick exploratory data analysis to understand distributions and relationships  
2. Encoded categorical variables using one-hot encoding  
3. Split the data into training (80%) and testing (20%) sets  
4. Trained a baseline **Linear Regression** model  
5. Evaluated performance using **MAE**, **RMSE**, and **R²**  
6. Interpreted model coefficients to identify key cost drivers  

---

## Key Results

- **MAE:** ~$4,181  
- **RMSE:** ~$5,796  
- **R²:** ~0.78  

### Insights
- Smoking status is the strongest predictor, increasing expected insurance charges by over **$23,000** on average  
- Age and BMI have moderate positive effects on costs  
- Number of children has a smaller positive impact  
- Sex and region show minimal influence after controlling for other factors  
- Higher prediction errors for high-cost individuals reflect the skewed nature of medical insurance charges  

---

## Limitations
- Insurance charges are highly right-skewed, which inflates RMSE  
- Linear regression assumes linear and additive relationships  
- The model is intended for cost understanding rather than actuarial pricing or deployment  

---

## Conclusion
A simple linear regression model explains a substantial portion of the variation in medical insurance costs while remaining highly interpretable. The results highlight smoking status as the dominant cost driver and demonstrate the trade-off between model simplicity and performance on extreme cases.
