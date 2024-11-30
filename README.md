# Shared Bike Demand Prediction  

## Project Overview  
This project aims to analyze and predict the demand for shared bikes using a multiple linear regression model. The analysis and predictions are based on data provided by **BoomBikes**, a US-based bike-sharing company. This study is conducted to help the company identify key factors driving bike demand and optimize its business strategies post-pandemic.  

---

## Problem Statement  
BoomBikes experienced a significant dip in revenue during the COVID-19 pandemic and is looking to rebound by understanding the factors influencing bike demand. The goal is to build a predictive model to determine the total number of daily rentals (`cnt`) and understand how various factors impact the demand.

---

## Dataset  
The dataset includes daily bike rental counts along with features such as weather conditions, season, temperature, humidity, and wind speed.  
### Key Features:
- **Temporal Variables**: `season`, `yr`, `mnth`, `weekday`, `workingday`, `holiday`.  
- **Weather Conditions**: `weathersit`, `temp`, `atemp`, `hum`, `windspeed`.  
- **Demand Indicators**: `casual`, `registered`, `cnt` (target variable).  

### Target Variable:
- **`cnt`**: Total number of bike rentals per day (sum of `casual` and `registered`).  

---

## Approach  
1. **Exploratory Data Analysis (EDA)**  
   - Performed univariate and bivariate analysis to understand feature distributions and relationships with `cnt`.  
   - Identified trends, seasonality, and weather impacts on bike demand.  

2. **Data Preparation**  
   - Converted categorical variables (`season`, `weathersit`) into meaningful labels.  
   - Checked for and handled multicollinearity among features.  
   - Normalized numerical variables where needed.  

3. **Model Building**  
   - Developed a multiple linear regression model using the `statsmodels` library.  
   - Evaluated the model's performance using metrics like R-squared, Adjusted R-squared, and residual analysis.  

4. **Insights and Recommendations**  
   - Identified key factors affecting demand, such as weather, season, and wind speed.  
   - Provided actionable insights for optimizing operational and marketing strategies.

---

## Model Performance  
- **R-squared**: 0.818  
- **Adjusted R-squared**: 0.815  
- **Key Findings**:  
  - **Positive Impact**: Warmer temperatures, September, and the year 2019.  
  - **Negative Impact**: High wind speeds, spring season, and poor weather conditions.  

