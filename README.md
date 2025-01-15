
# Rajarshi_Guchhait_PM_Accelerator_Data_Scientist

Rajarshi Guchhait's Technical Assessment for the role of Data Scientist at PM Accelerator

## Mission of PM Accelerator

By making industry-leading tools and education available to individuals from all backgrounds, we level the playing field for future PM leaders.
We grant aspiring and experienced PMs what they need most – Access. 
We introduce you to industry leaders, surround you with the right PM ecosystem, and discover the new world of AI product management skills.



## About the project
This project is a part of technical assessment for the position of data scientist at PM Accelerator. This project involves analysis of Time-series data of the World Weather Repository. The parameters of interest are Temperature and Precipitation. This project evaluates multiple models and compares their performance.

## Dataset
World Weather Repository: https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository/code

No. of Columns: 41  
No. of Entries (Rows): 46577  
Parameters of interest: Temperature, Precipitation  
Columns chosen for time series analysis:
‘temperature_fahrenheit’,
‘precip_mm’


## Programming Environment
Programming language: Python 3.12  
IDE: Jupyter Notebook

## Dependencies 
* numpy
* pandas
* math
* matplotlib -> pyplot
* seaborn
* plotly -> express, graph_objects, subplots
* sklearn.preprocessing -> MinMaxScaler
* sklearn.metrics -> mean_absolute_error, mean_squared_error, r2_score
* sklearn.ensemble -> IsolationForest, GradientBoostingRegressor, RandomForestRegressor
* Prophet -> Prophet
* sklearn.model_selection -> train_test_split
* statsmodels.tsa.stattools -> adfuller
* statsmodels.tsa.arima.model -> ARIMA
* statsmodels.graphics.tsaplots -> plot_acf, plot_pacf

## Steps of Data Analysis
* **Step 1**: Import dataset 
* **Step 2**: Check for missing values
* **Step 3**: Check for outliers. This step consists of detecting outliers visually by Box plots.
* **Step 4**: Find outliers. This stage consists of two methods to find outliers:
    - Statistically using Inter-Quartile Range.
    - Anomaly detection using IsolationForest
* **Step 5**: Cap the outliers such that the values lie within the lower and upper limits.
* **Step 6**: Normalize the data --> Min-Max Scaling
* **Step 7**: Exploratory Data Analysis:
    - Correlation Visualization
    - Temperature and precipitation trends
    - Temperature, precipitation and humidity trends of three example countries: India, China and USA
    - Continent-wise Avg. Temperature, Humidity, and Wind speed and direction:
        - Asia
        - Europe
        - America
        - Africa
* **Step 8**: Time Series Modelling and Forecasting. 
    * Models: 
        - ARIMA
        - Gradient Boosting Regressor
        - Random Forest Regressor
        - Prophet
    * Performance Metrics:
        - Mean Absolute Error
        - Root Mean Squared Error
        - R2 Score
* **Step 9**: Model Comparison:
    - ARIMA and Prophet are not suitable for time series modelling of this dataset
    - Gradient Boosting Regressor and Random Forest Regressor give best performance stats
    - Overall, Random Forest Regressor gives lowest errors and highest R2 score but concerns remain about overfitting 





