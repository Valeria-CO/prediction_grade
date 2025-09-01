Predicting Student Grades from Socio-Demographic Data.


Purpose:  The goal of this project is to investigate whether it is possible to predict students’ final school grades using only socio-demographic and background features, without relying on direct academic performance indicators.

Data:   The dataset comes from https://archive.ics.uci.edu/dataset/320/student+performance?utm_source=chatgpt.com
This data approach student achievement in secondary education of two Portuguese schools. The data attributes include student grades, demographic, social and school related features) and it was collected by using school reports and questionnaires.

File (https://github.com/Valeria-CO/prediction_grade/blob/master/features_analysis.ipynb) contains exploratory analysis and preprocessing of data.


Methods:   The following models were used: Linear regression, RandomForestRegressor, XGBRegressor
           Evaluation metrics: MAE, MSE, R²
in detail https://github.com/Valeria-CO/prediction_grade/blob/master/models.ipynb

Key Results:
Best model - XGBRegressor (MAE = 2.18, MSE = 9.85, R² = 0.29)
Overfitting problems have always been observed, which can be seen in the learning curve.
Socio-demographic characteristics are weak predictors of grades; at most, they can capture general trends, but not exact values.

Conclusion:
Socio-demographic features alone provide only limited predictive power for student grades. While models like Random Forest and XGBoost outperform linear regression, they still suffer from overfitting and achieve modest accuracy. 
The results suggest that to make reliable grade predictions, additional academic or behavioral data would be necessary.
