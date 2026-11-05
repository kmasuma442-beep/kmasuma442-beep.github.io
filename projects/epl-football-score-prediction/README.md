# Beyond Win, Draw and Loss: A Comparative Study of Count Regression Models for English Premier League Football Score Prediction

## Project Overview

Football score prediction is an important application of statistical modelling in sports analytics. Since goals are discrete count variables, count regression models provide a suitable framework for analysing and predicting football scores.

This project investigates and compares three statistical approaches for predicting English Premier League (EPL) football scores:

- Poisson Regression
- Negative Binomial Regression
- Bivariate Poisson Regression

Unlike approaches that directly predict match outcomes such as Win, Draw, or Loss, this study first predicts the actual goal counts of home and away teams. The final match outcome is then determined by comparing the predicted scores.

## Research Objectives

- Apply Poisson Regression and Negative Binomial Regression separately for home and away goal prediction.
- Apply Bivariate Poisson Regression to jointly model home and away team goal counts.
- Compare the predictive performance of the three regression models.
- Identify important match-related factors influencing goal-scoring performance.
- Evaluate the models using statistical and classification-based performance measures.

## Dataset Description

The study uses historical English Premier League match data covering **10 complete seasons**, consisting of **3,770 matches**.

**Data Sources:**
- [FBref – Premier League Statistics](https://fbref.com/en/comps/9/Premier-League-Stats)
- [Transfermarkt](https://www.transfermarkt.co.in/)

### Key Variables

The dataset includes match-related variables such as:

- Season and Match Date
- Home Team and Away Team
- Full-Time Home Goals and Away Goals
- Half-Time Home Goals and Away Goals
- Home Shots and Away Shots
- Shots on Target
- Corners
- Fouls
- Yellow Cards and Red Cards
- Average Team Age
- VAR Usage

Exploratory analysis indicated the presence of overdispersion in the goal-scoring variables, as their variances exceeded their corresponding means.

## Methodology

The project follows a structured statistical modelling workflow:

1. **Data Collection:** Historical EPL match data were collected from FBref and Transfermarkt.
2. **Data Preprocessing:** Raw match records were cleaned and standardized.
3. **Exploratory Data Analysis:** Match outcomes, goal distributions, and descriptive statistics were examined.
4. **Feature Selection and Engineering:** Match performance variables and additional features were used for modelling.
5. **Model Development:** Poisson, Negative Binomial, and Bivariate Poisson regression models were implemented.
6. **Prediction:** Home and away goal counts were predicted, and match outcomes were determined from the predicted scores.
7. **Model Evaluation:** The predictive performance of the models was compared using evaluation metrics.

## Statistical Models

### 1. Poisson Regression

Poisson Regression was used as the baseline model for predicting home and away goal counts separately.

It assumes that the mean and variance of the response variable are equal.

### 2. Negative Binomial Regression

Negative Binomial Regression extends the Poisson model by introducing an additional dispersion parameter.

It is suitable for overdispersed count data, where the variance exceeds the mean.

### 3. Bivariate Poisson Regression

Bivariate Poisson Regression jointly models home and away goal counts within a single framework.

It helps incorporate the dependence between the scoring processes of both teams.

## Feature Engineering

Additional match-related features were incorporated into the Bivariate Poisson modelling framework:

- **Shot Difference:** Difference in total shots between the two teams.
- **Target Difference:** Difference in shots on target between the teams.
- **Pressure Ratio:** A measure representing relative pressing intensity.
- **Card Difference:** Difference in disciplinary cards between the teams.

## Model Evaluation Metrics

The models were evaluated using the following measures:

- Accuracy
- Precision
- Recall
- F1-Score
- Mean Squared Error (MSE)

A comparative evaluation was conducted to identify the model with the strongest predictive performance.

## Results and Model Comparison

The comparative results obtained in the dissertation are:

| Evaluation Metric | Poisson Regression | Negative Binomial Regression | Bivariate Poisson Regression |
|---|---:|---:|---:|
| Accuracy | 69.99% | **78.73%** | 75.33% |
| Precision | 0.68 | **0.79** | 0.75 |
| Recall | 0.70 | **0.79** | 0.75 |
| F1-Score | 0.68 | **0.78** | 0.74 |

### Key Findings

- Negative Binomial Regression achieved the highest prediction accuracy of **78.73%**.
- The presence of overdispersion affected the performance of the standard Poisson model.
- Negative Binomial Regression provided better predictive performance by accounting for overdispersion.
- Bivariate Poisson Regression captured the joint nature of home and away goal counts.
- Shots on target emerged as an important predictor of football goal-scoring performance.

## Conclusion

The comparative analysis indicates that Negative Binomial Regression provided the best overall predictive performance among the three models considered.

Its ability to accommodate overdispersion made it more suitable for the EPL goal-scoring data used in this study.

The findings highlight the importance of selecting appropriate count regression models for football score prediction and sports analytics.

## Future Scope

Future research may explore:

- Incorporating player injuries, team formations, and weather conditions.
- Applying machine learning and deep learning approaches.
- Developing hybrid statistical and machine learning models.
- Extending the analysis to other football leagues and competitions.

## Tools and Technologies

- Python
- Statistical Modelling
- Data Preprocessing
- Exploratory Data Analysis
- Feature Engineering
- Data Visualization

## Project Information

**Author:** Masuma Khatun  
**Degree:** M.Sc. Tech in Statistics and Data Science  
**University:** Adamas University  
**Project Type:** Academic Dissertation  
**Year:** 2026

**Project Focus:** Football Analytics | Count Regression | Statistical Modelling | Predictive Analytics
