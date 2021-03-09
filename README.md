# Building Machine Learning Models to Predict ETF Prices (Python)
Design and build a machine learning model that can accurately predict historical prices of ETFs using Python.

Website showcasing our findings: https://machine-learning-etfs.herokuapp.com/home.html

# Introduction
Our team was tasked with creating a Machine Learning model to incorporate into a final dashboard including visualizations from our findings from our models.
Considering the stock market's recent media popularity surrounding the $GME and r/WallStreetBets battle against hedge funds, we chose to construct various models to attempt to predict prices of a chosen ETF (^NTXD) when the model is given historical pricing data. 

We chose to use an Exchange Traded Fund (ETF) as opposed to a stock in order to encompass a prediction of an industry snapshot as opposed to a single company or commodity stock. The Nasdaq-100 Technology Sector Index is an equally rated index of companies listed as "Technology" on the Nasdaq-100 (Source: https://indexes.nasdaqomx.com/Index/Overview/NDXT?)


# Modeling
Three types of models were used for the machine learning models: ARIMA, CART, and Facebook Prophet. More information on how these models work can be found on our website, listed above. For stock price forecasting, time series modeling must be used, in to compensate for moving averages.  

For each model, hyperparameters were tuned in order for the models to produce the most accurate results possible. The Sci-kit Learn module used for modeling allowed the random splitting of train and test datasets to ensure for reproducibility. 

The results of the train and test model are mean squared error and r squared, respectively. The mean squared error is the average squared difference between the estimated values and the actual value. The smaller this number is, the more accurate the model.

A max_depth of 100 proved to be less accurate than a max_depth of 8. It is important to remember that these results are randomized. A higher max_depth is not necessarily a determinant of a more accurate model, finding the correct depth is more important than using a ridiculously high number (and therefore a great deal of computing power).

More details and information about the tuning process, prediction, and output can be found on our site.

# Results

In conclusion, producing reliable models to accurately and reliably predict securities pricing is difficult. While working with different <code>max_depth</code> values, our team was able to produce somewhat accurate predictions. However, unexpected dips in the market (such as in late 2018/early 2019) present a challenge to accurately predicting prices. 
  
# Sources
^NDXT Historical Pricing Data:
https://finance.yahoo.com/quote/%5ENDXT/history?p=%5ENDXT

^NDXT Overview:
https://indexes.nasdaqomx.com/Index/Overview/NDXT?


