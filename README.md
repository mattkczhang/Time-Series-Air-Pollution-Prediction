# Time Series Air Pollution Prediction

The Time Series Air Pollution project is a in-class group project at the University of Chicago Time Series Analysis and Forecasting course in 2022 Spring.

![air_pollution](https://user-images.githubusercontent.com/94136772/178402378-b60ef5b7-2637-4660-93a8-87f172740f26.jpeg)

## Description

The annual average concentration of fine particulate matter (PM2.5) across China was 57 micrograms per meter cubed in 2017, nearly six times what the World Health Organization deems to be acceptable limits. Poor outdoor air quality results in over 1 million deaths across China each year.

The causes of Beijing's widespread air pollution can be attributed to several factors: an enormous economic boom, a surge in the number of motorized vehicles, population growth, output from manufacturing, and natural reasons which include the city's surrounding topography and seasonal weather. 

The project intends to predict the future 3 months air quality based on 4 years air pollution data like PM2.5, PM10, S02, MO2, CO using Exponential Smoothing, ARIMA, Naïve, Regression, and Regression with ARMA errors. We first check the missing values and features correlation and then conduct data transformation based on the time series plot and stationarity tets. After exploring different possible models, we utilize cross validation with MSE and AICc as evaluation metrics to further confirm the model performance. 

Our final model is the Arima model with 2 PM10 and CO as the external (exogenous) variables because it has the lowest MSE. In this case, we view model complexity measured by AICc to be less important compared to model accuracy measured by MSE as our model is mainly designed for governments or big enterprises. The residual doesn’t have obvious autocorrelation, which is supported by the Ljung-box test with significant p-value. We also find out that all parameters are significantly different from zero. 

## Authors

Kaichong (Matt) Zhang: University of Chicago Student

Flora Huang: University of Chicago Student

Qiansheng Zhou: University of Chicago Student

Zhangchi Liu: University of Chicago Student

Michael Wu: University of Chicago Student
