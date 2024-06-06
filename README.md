# Netflix customer forecasting.
![netflix-symbol-black](https://github.com/Kamuthuj/Netflix-customer-forecasting/assets/121629618/0016c78e-5650-4fdf-88f4-6bcc716574b3)

The aim of this project is to accurately predict the number of new subscribers in a given period to better understand the growth potential of the business.The dataset contains subscription counts of Netflix at the start of each quarter from 2013 to 2023. The data was clean and did not have null values. I converted the date to its right data type before analysis. I created a new column to check on the quarterly growth rate by calculating the percentage change of the subscribers,labelling green as positive growth rate and red as negative.

![Quarterly subs](https://github.com/Kamuthuj/Netflix-customer-forecasting/assets/121629618/9a1970bd-e6ea-4b9a-a823-e12943ca5327)

I performed the same operation to check on the yearly subscription rate.
![Yearly growth](https://github.com/Kamuthuj/Netflix-customer-forecasting/assets/121629618/6750e9e7-3429-4b64-8d14-d4c869a1d5f2)

I utilized time series forecasting using ARIMA to forecast the number of subscriptions. I converted the original data frame into a time series fomart where the time period became the index and subscribers as the data. I plotted the ACF and PACF of the differenced time series to provide insights into the potential order of the AR and MA components in the time series.

![AR](https://github.com/Kamuthuj/Netflix-customer-forecasting/assets/121629618/bacdf252-a3b5-49dd-9120-92fe9c0e3cfa)
Based on the plots, we find that p=1 and q=1. The ACF plot cuts off at lag 1, indicating q=1, and the PACF plot also cuts off at lag 1, indicating p=1. As there is a linear trend in the subscription growth rate, we can set the value of d as 1 to remove the linear trend, making the time series stationary.

I forecasted for the next 5 quarters and plotted the visualization which showed an upward trend of new subscribers over time.
![Screenshot (90)](https://github.com/Kamuthuj/Netflix-customer-forecasting/assets/121629618/9ab82e0a-9022-4527-888f-e3e4cc96dd6e) 

Using techniques like time series forecasting, Netflix can estimate the expected number of new subscribers in a given time period and better understand the growth potential of their business. It enhances operational efficiency, financial planning, and content strategy, ultimately contributing to their success and growth in the highly competitive streaming industry.





