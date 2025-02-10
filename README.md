# AirQuality-Prediction
## Overview
The air quality prediction analysis focuses on developing a machine learning regression model to predict carbon monoxide (CO) concentrations using data from a gas multisensor device. By accurately forecasting CO levels, we can contribute to better public health measures and environmental management, as air pollution significantly impacts human health and ecosystems.
## Workflow
The following steps outline the process followed in the analysis:
- #### Data Collection:
 - Collected the dataset "AirQualityUCI.csv" with hourly air quality readings collected from a gas sensor array.
- #### Data Preprocessing:
  - Handled missing values 
  - Outliers were detected and managed using IQR methos.
- #### Exploratory Data Analysis (EDA):
 - Conducted visualizations to explore the data distribution and identify trends or anomalies.
 - Generated a correlation matrix heatmap to assess relationships between different features and the target variable.
- #### Feature Selection:
 - Employed SelectKBest with the F-test to identify the most relevant features affecting CO predictions, reducing dimensionality.
 - #### Model Training and Evaluation:
  - Split the dataset into training (80%) and testing (20%) sets.
  - Scaled features using StandardScaler to ensure uniformity.
  - Trained various regression models:
    - Linear Regression
    - Random Forest Regressor
    - Gradient Boosting Regressor
    - Support Vector Regressor (SVR)
    - Multi-Layer Perceptron (MLP) Regressor
  - Evaluated model performance using metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R² Score.
- #### Hyperparameter Tuning:
  - Utilized GridSearchCV to optimize hyperparameters for the Random Forest Regressor, enhancing its predictive performance.
- #### Model Deployment:
  - Created a robust pipeline that combines preprocessing and model predictions using joblib for future applications.
- #### Prediction:
  - The final model was tested on unseen data to assess its efficacy in real-world applications.
#### Results
- Model Performance:
The Random Forest Regressor outperformed other models, achieving the highest R² score and lowest RMSE among the evaluated algorithms.
Metrics indicate that the model can accurately predict CO levels within acceptable tolerances, providing reliable forecasts for applications in air quality management.
- Feature Importance:
The analysis revealed critical features influencing CO concentrations, guiding future investigations and policymaking efforts.
### Conclusion
The analysis successfully developed a machine learning regression model capable of accurately predicting carbon monoxide concentrations using multisensor data. The project addressed key challenges related to data quality, feature selection, and model optimization. As a result, the trained model can be utilized for real-time air quality predictions, contributing to improved public health initiatives and environmental monitoring.
