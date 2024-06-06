# Netflix customer forecasting.
![netflix-symbol-black](https://github.com/Kamuthuj/Netflix-customer-forecasting/assets/121629618/0016c78e-5650-4fdf-88f4-6bcc716574b3)

The aim of this project is to accurately predict the number of new subscribers in a given period to better understand the growth potential of the business.The dataset contains subscription counts of Netflix at the start of each quarter from 2013 to 2023. The data was clean and did not have null values. I converted the date to its right data type before analysis. I created a new column to check on the quarterly growth rate by calculating the percentage change of the subscribers,labelling green as positive growth rate and red as negative.

![Quarterly subs](https://github.com/Kamuthuj/Netflix-customer-forecasting/assets/121629618/9a1970bd-e6ea-4b9a-a823-e12943ca5327)

I performed the same operation to check on the yearly subscription rate.
![Yearly growth](https://github.com/Kamuthuj/Netflix-customer-forecasting/assets/121629618/6750e9e7-3429-4b64-8d14-d4c869a1d5f2)

I utilized time series forecasting using ARIMA to forecast the number of subscriptions. I converted the original data frame into a time series fomart where the time period became the index and subscribers as the data. I plotted the ACF and PACF of the differenced time series to provide insights into the potential order of the AR and MA components in the time series.



