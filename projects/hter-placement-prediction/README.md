# Student Placement Prediction Using HTER

## Project Overview
This academic internship project focuses on developing and evaluating a classification technique called **Hyperbolic Tangent Exponential Regression (HTER)** for predicting student placement outcomes.

The proposed model extends Logistic Regression by introducing two additional parameters: alpha (α), a scaling parameter, and gamma (γ), a damping parameter.

## Project Objectives
- Develop an HTER-based classification model for student placement prediction.
- Formulate parameter estimation and hypothesis testing procedures.
- Compare HTER with established classification algorithms.
- Evaluate model performance using statistical and classification metrics.

## Dataset
- **Source:** Aliah University placement data.
- **Original records:** 851 students.
- **Analysed records:** 749 students who participated in campus placement drives.
- **Target variable:** Placement Status (Placed / Not Placed).

### Key Features
- Academic performance (Class 10, Class 12 and B.Tech scores)
- Gender and academic stream
- Backlog history
- Placement training status
- Campus drives attended

## Methodology
1. Data cleaning and preprocessing.
2. Encoding categorical variables.
3. Standardisation of numerical features.
4. Implementation of the HTER classification model.
5. Parameter estimation using Maximum Likelihood Estimation (MLE).
6. Hypothesis testing and comparative model evaluation.

## Models Compared
- Hyperbolic Tangent Exponential Regression (HTER)
- Logistic Regression
- K-Nearest Neighbours (KNN)
- Linear Discriminant Analysis (LDA)
- Quadratic Discriminant Analysis (QDA)
- Decision Tree
- Support Vector Machine (SVM)

## Tools & Technologies
- Python
- Scikit-learn
- Statistical Modelling
- Numerical Optimisation
- Data Visualisation

## Evaluation Metrics
Accuracy, Precision, Recall, F1-score, ROC-AUC and McNemar's Test.

## Key Results
- HTER achieved **73.7% accuracy** in the comparative evaluation.
- Logistic Regression also achieved **73.7% accuracy**.
- SVM achieved the highest accuracy of **74.9%**.
- McNemar's test (p-value = 1.000) indicated no statistically significant difference between HTER and Logistic Regression predictions.

## Conclusion
The study showed that HTER achieved performance comparable to Logistic Regression on the placement dataset. Although it did not provide a significant improvement in this application, it offers additional theoretical flexibility for modelling nonlinear relationships.

## Author
**Masuma Khatun**  
M.Sc. Tech in Statistics and Data Science

