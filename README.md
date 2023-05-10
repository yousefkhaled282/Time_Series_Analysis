# Project Title:  Time Series Analysis & Forecasting on Airline Passengers Dataset

## Introduction:
In this project, we perform time series analysis on the airline passengers dataset to predict future passenger numbers for the airline industry. 
Time series analysis is a statistical technique that is used to analyze time series data and extract meaningful insights. 
In this project, we use various time series techniques such as 
 - naive forecasting 
 - simple average
 - weighted moving average 
 - simple linear regression
 - classical decomposition
 - STL decomposition
 - ARIMA 
 - S-ARIMA 
 - Exponential Smoothing 
 - Facebook Prophet 
 - XGBoost 
 
to make predictions on future passenger numbers.

## Dataset:
The dataset used in this project is the **airline passengers** dataset which contains the number of passengers who traveled by airline per month from 1949 to 1960.
The dataset has 144 observations and two columns: Month and the number of passengers. 

Methodology:
First, we import the necessary libraries such as numpy, pandas, sklearn, warnings, and matplotlib. 
Then, we read the dataset using the pandas read_csv function and convert the Month column to a datetime data type. 
We then set the Month column as the index and plot the data to visualize the trend and seasonality in the data. 
We find that the data has a positive trend with seasonality and there is a peak in passenger numbers every year between July and August.

Next, we split the data into training and testing sets using various techniques such as 
  - fixed partition 
  - roll-forward
  - cross-validation
  

We then use naive forecasting, simple average, weighted moving average, simple linear regression, classical decomposition, 
  STL decomposition, ARIMA, S-ARIMA, Exponential Smoothing, Facebook Prophet, and XGBoost to make predictions on future passenger numbers.

We evaluate the models using various metrics such as **RMSE** and compare the performance of each model using fixed partition, roll-forward, and cross-validation techniques. We find that the roll-forward technique gives the best results for most models and that the simple linear regression model performs well when combined with classical decomposition.

## Results:

<table>
  <tr>
    <th>Technique</th>
    <th>Fixed</th>
    <th>Roll</th>
    <th>Cross</th>
  </tr>
  <tr>
    <td>Simple Moving Average</td>
    <td>113.8</td>
    <td>55.38</td>
    <td>139.6</td>
  </tr>
  <tr>
    <td>Naïve forecast</td>
    <td>137.3</td>
    <td>44.2</td>
    <td>142.6</td>
  </tr>
  <tr>
    <td>Weighted Moving Average</td>
    <td>84.6</td>
    <td>52.4</td>
    <td>183</td>
  </tr>
  <tr>
    <td>Linear Regression Average</td>
    <td>74.7</td>
    <td>55.4</td>
    <td>80</td>
  </tr>
  <tr>
    <td>Classical Decomposition</td>
    <td>60</td>
    <td>54.7</td>
    <td>84.1</td>
  </tr>
  <tr>
    <td>STL Decomposition</td>
    <td>68.7</td>
    <td>66.2</td>
    <td>80.7</td>
  </tr>
  <tr>
    <td>ARIMA</td>
    <td>126.1</td>
    <td>39.72</td>
    <td>141.83</td>
  </tr>
  <tr>
    <td>S-ARIMA</td>
    <td>39.9</td>
    <td>11.5</td>
    <td>55.1</td>
  </tr>
  <tr>
    <td>Exponential Smoothing Single</td>
    <td>139.7</td>
    <td>47.1</td>
    <td>140.3</td>
  </tr>
  <tr>
    <td>Exponential Smoothing Double Additive</td>
    <td>118.3</td>
    <td>44</td>
    <td>93.7</td>
  </tr>
  <tr>
    <td>Exponential Smoothing Double Multiplicative</td>
    <td>107.6</td>
    <td>43.7</td>
    <td>104.9</td>
  </tr>
  <tr>
    <td>Exponential Smoothing Triple Additive</td>
    <td>35.7</td>
    <td>12.3</td>
    <td>57.4</td>
  </tr>
  <tr>
    <td>Exponential Smoothing Triple Multiplicative</td>
    <td>13.8</td>
    <td><strong>10.3</strong></td>
    <td>40.1</td>
  </tr>
  <tr>
    <td>FB Prophet</td>
    <td>40.3</td>
    <td>31.5</td>
    <td>45.4</td>
  </tr>
  <tr>
    <td>XGBOOST Regressor</td>
    <td>53.1</td>
    <td> - </td>
    <td>104.2</td>
  </tr> 
  </table>




## Conclusion:
In conclusion, we have analyzed the airline passengers dataset using various time series techniques and found that 
the Exponential Smothing Triple Multiplicative model gives the best results overall when predicting future passenger numbers.
This project demonstrates the usefulness of time series analysis in making predictions for future trends in various industries, especially in the airline industry.
