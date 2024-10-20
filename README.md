# IBM-Z-DATATHON-QUANTUM-CODERS
# Models Overview
This project employs several time series forecasting models to predict energy consumption. Below are detailed descriptions of each model used in this project.
## 1. ARIMA (AutoRegressive Integrated Moving Average)
## Overview: 
ARIMA is a widely used statistical method for time series forecasting. It combines autoregressive and moving average components along with differencing to make the time series stationary.
## Key Features:
1) Effective for univariate time series data.
2) Identifies patterns and relationships based on past values.
3) Parameters: 𝑝(AR terms), 𝑑(differencing), 𝑞(MA terms).
## Usage:
Used as a baseline model to evaluate performance against more complex models.
**PROGRAM :**
![image](https://github.com/user-attachments/assets/cf5f44ba-3973-49fd-87d8-794b157257a0)
![image](https://github.com/user-attachments/assets/a4afcea5-0ae3-4f22-9f13-239643241ae9)
![image](https://github.com/user-attachments/assets/f4214347-2aee-40a0-bba3-ff598cfc4a99)
![image](https://github.com/user-attachments/assets/2a45b98c-6416-4a96-9d01-b02cecd5bca2)
![image](https://github.com/user-attachments/assets/3b8b9070-08d3-423a-aa76-42b251617df9)
![image](https://github.com/user-attachments/assets/dd542eb8-caa1-42f1-80aa-9e646929ec09)
![image](https://github.com/user-attachments/assets/771e3a0d-6a23-4e83-9d2c-5f39b267ccb4)
![image](https://github.com/user-attachments/assets/02307091-1ceb-43ca-a835-a00babf5a257)
## 2. SARIMA (Seasonal AutoRegressive Integrated Moving Average)
## Overview: 
SARIMA extends ARIMA to handle seasonal data. It incorporates seasonal autoregressive and moving average components to better capture seasonality in time series.
## Key Features:
1) Accounts for both non-seasonal and seasonal factors.
2) Parameters: 𝑃,𝐷,𝑄,𝑆 represent seasonal AR terms, differencing, MA terms, and the seasonality length.
## Usage:
Utilized for datasets with clear seasonal patterns, enhancing forecast accuracy.
**PROGRAM:**
![image](https://github.com/user-attachments/assets/71124edf-10ef-4e03-8d6e-183bf5c1dcfa)
![image](https://github.com/user-attachments/assets/0ce8e363-2e8b-48bd-847d-fe960f6ec648)
![image](https://github.com/user-attachments/assets/24abeaa5-ff6b-4b56-8ac9-7212d0f4a54f)
![image](https://github.com/user-attachments/assets/b8a5f1e5-c7b4-433c-834d-7de8c85faeb8)
![image](https://github.com/user-attachments/assets/dc6d1591-d7eb-49b7-b743-0638f465039e)
## 3. LSTM (Long Short-Term Memory)
## Overview: 
LSTM is a type of recurrent neural network (RNN) designed to learn long-term dependencies in sequential data. It is well-suited for time series forecasting due to its ability to capture complex relationships.
## Key Features:
1) Handles large datasets and long sequences.
2) Can learn nonlinear patterns and relationships in data.
3) Employs a gating mechanism to retain relevant information over time.
## Usage:
Applied to capture intricate relationships and dynamics in the energy consumption data.
**PROGRAM:**
![image](https://github.com/user-attachments/assets/1711e9b7-1753-4b3b-8301-e06c2337bc73)
![image](https://github.com/user-attachments/assets/8ed16665-b299-42a2-a649-bcfad73769af)
![image](https://github.com/user-attachments/assets/e7abb23c-d008-49a0-845b-835d364101df)
![image](https://github.com/user-attachments/assets/65eb8dec-2fd6-481c-9cb4-947d4f9b503b)
![image](https://github.com/user-attachments/assets/b4732997-1315-4218-a25a-91b06369b33f)
## 4. Enhanced SARIMA (E_SARIMA)
## Overview: 
The enhanced SARIMA model incorporates advanced techniques to improve forecasting accuracy. This includes optimizing hyperparameters, implementing cross-validation, and integrating external factors such as weather conditions.
## Key Features:
1) Improved parameter tuning for better model fit.
2) Incorporation of additional exogenous variables to enhance prediction accuracy.
3) Continuous model evaluation and updates based on feedback loops.
## Usage:
Used as the primary model for accurate energy consumption forecasts, leveraging its enhanced capabilities to adapt to changing patterns in the data.
**PROGRAM:**
![image](https://github.com/user-attachments/assets/bef4aec8-7bdb-4edb-8f85-25bb044a3424)
![image](https://github.com/user-attachments/assets/7e34cef8-d9de-47b5-8427-1dee340ac094)
![image](https://github.com/user-attachments/assets/1863ba9d-ef8b-4891-b6df-4c71ad139c9e)
![image](https://github.com/user-attachments/assets/769b2455-e16d-430c-b29e-7e547b87bf00)
![image](https://github.com/user-attachments/assets/a0b4f862-a4f0-4c8e-9184-3127e0d83e6e)
![image](https://github.com/user-attachments/assets/aa9080bc-dcfd-464c-b35c-9b7994983caa)

## How to Use the Models
**1) Dataset Preparation**: Ensure your dataset (pre_data.csv) is in the project directory and formatted correctly.
**2) Installation**: Make sure to install all required libraries
```
pip install numpy pandas matplotlib statsmodels scikit-learn tensorflow
```
**3) Run the Models**:
1) You can run each model by executing the respective Python scripts.
2) The main script integrates all models and compares their performance.
   
**4) Evaluate the Results**: Metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and Mean Absolute Percentage Error (MAPE) are calculated for each model.Evaluate the Results: Metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and Mean Absolute Percentage Error (MAPE) are calculated for each model.
## CONCLUSION : 
This project showcases the implementation of various forecasting techniques to address the challenge of energy consumption prediction. Each model's performance is evaluated, providing insights into the effectiveness of traditional and modern approaches.

