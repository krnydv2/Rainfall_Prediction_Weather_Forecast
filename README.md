# Rainfall_Prediction_Weather_Forecast

![Rainfall](https://user-images.githubusercontent.com/96686904/181911450-4af7f711-0409-4a53-8cb6-9c8072361936.jpg)

# Problem Definition
Weather forecasting is the application of science and technology to predict the conditions of the atmosphere for a given location and time. Weather forecasts are made by collecting quantitative data about the current state of the atmosphere at a given place and using meteorology to project how the atmosphere will change.

Rain Dataset is to predict whether or not it will rain tomorrow. The Dataset contains about 10 years of daily weather observations of different locations in Australia.

Here, we are trying to Build Machine Learning Model to predict Two things:


## The Objectives:
1. Whether or not it will rain Tomorrow - A classification problem
2. Prediction of amount of rainfall - A regression problem

### Data Directory
- Date - The date of observation
- Location -The common name of the location of the weather station
- MinTemp -The minimum temperature in degrees celsius
- MaxTemp -The maximum temperature in degrees celsius
- Rainfall -The amount of rainfall recorded for the day in mm
- Evaporation -The so-called Class A pan evaporation (mm) in the 24 hours to 9am
- Sunshine -The number of hours of bright sunshine in the day.
- WindGustDir- The direction of the strongest wind gust in the 24 hours to midnight
- WindGustSpeed -The speed (km/h) of the strongest wind gust in the 24 hours to midnight
- WindDir9am -Direction of the wind at 9am
- WindDir3pm -Direction of the wind at 3pm
- WindSpeed9am -Wind speed (km/hr) averaged over 10 minutes prior to 9am
- WindSpeed3pm -Wind speed (km/hr) averaged over 10 minutes prior to 3pm
- Humidity9am -Humidity (percent) at 9am
- Humidity3pm -Humidity (percent) at 3pm
- Pressure9am -Atmospheric pressure (hpa) reduced to mean sea level at 9am
- Pressure3pm -Atmospheric pressure (hpa) reduced to mean sea level at 3pm
- Cloud9am - Fraction of sky obscured by cloud at 9am
- Cloud3pm -Fraction of sky obscured by cloud at 3pm
- Temp9am-Temperature (degrees C) at 9am
- Temp3pm -Temperature (degrees C) at 3pm
- RainToday -Boolean: 1 if precipitation (mm) in the 24 hours to 9am exceeds 1mm, otherwise 0
- RainTomorrow -The amount of next day rain in mm. Used to create response variable . A kind of measure of the "risk".


### Steps Included in the Project:
- Importing Libraries
![1](https://user-images.githubusercontent.com/96686904/181914205-91dd13b8-3536-4608-bef3-2800c37e006e.png)

- Loading Data
![2](https://user-images.githubusercontent.com/96686904/181914216-0af06ced-12d7-4a9c-8299-274a891ec2af.png)

- Understanding Data
![6](https://user-images.githubusercontent.com/96686904/181914252-7ba1a709-13eb-41a6-ae73-f16bb5065543.png)

- Missing Values
- Exploring Variables(Data Anylasis)
![3](https://user-images.githubusercontent.com/96686904/181914235-14cd31f4-f2e1-458e-9850-b82290d11a18.png)

- Univarite, Bivariate and Multi Variate Analysis
![4](https://user-images.githubusercontent.com/96686904/181914242-ef92ed1a-19ba-4dc1-bafb-4982b31c05fb.png)
![9](https://user-images.githubusercontent.com/96686904/181914284-a4eab474-be86-48f2-abc6-3096fae015e3.png)


- Data Processing like Checking Skewness, Checking Outliers, Checking Corr
![7](https://user-images.githubusercontent.com/96686904/181914262-fbf82137-6a5a-4dc6-9401-d572ee39edc2.png)
![8](https://user-images.githubusercontent.com/96686904/181914276-669605ab-ae32-48c6-a62b-4a84f885f6c7.png)
![10](https://user-images.githubusercontent.com/96686904/181914297-cb74b5cc-59f4-4868-8fd4-e34a217ab577.png)



- Checked Multicollinearity using VIF
- Applying different models for Both Classification and Regression Target Variable.
![11](https://user-images.githubusercontent.com/96686904/181914303-905f70f1-8a46-458a-aaa5-bd6f5f362c9b.png)

- Choosing right model
![12](https://user-images.githubusercontent.com/96686904/181914313-773f9806-d519-4ebe-8102-afe523dff4e1.png)
![13](https://user-images.githubusercontent.com/96686904/181914320-087b953c-ee5f-4e99-93d3-61dba1d54561.png)

- Performing Parameter Tuning
![14](https://user-images.githubusercontent.com/96686904/181914326-182335d8-f72f-4140-8e4e-2688f1ff6a43.png)
![15](https://user-images.githubusercontent.com/96686904/181914330-db29e1a8-f82f-485f-b1e2-cf5467659071.png)

Again performed the same set of operation for second variable
![16](https://user-images.githubusercontent.com/96686904/181914343-97da5749-3176-4635-9f6b-5c6d5bb0f008.png)
![17](https://user-images.githubusercontent.com/96686904/181914354-645f51ad-c7ab-46ad-a605-654631dda0a4.png)

### Conclusion:
- RandomForest Regressor model has the best Accuracy i.e. 91%
- Performed Hyper Parameter Tuning using GridSearchCV, and Accuracy score was 88%, which is very good.
- Drawn Distribution Plot between Acutal and Predicted Test Data, Which has Normally Distribution and shows that our Model is working very well.

