## Tesla Stock Price Prediction w/Online Learning

(kaggle link -> https://www.kaggle.com/code/banddaniel/tesla-stock-price-prediction-w-online-learning)

<i><span style="color:#e74c3c;"> Main Goal: </span> Predict <b>the close price</b> of a Tesla stock price using the Online Learning method with a Linear Regression model.</i>

First of all, I am very keen on trying new methods. This is why I tried an Online/Incremental Learning [1] method in this project for time series forecasting. 
In this method, our model learns from one sample of each training loop. Actually, this type of learning is very handy in the streaming data.


* I used **River** library for online/incremental learning [2],
* I created cyclical features at the feature engineering stage (1 row = 1 day, 5 rows = 1 week, 20 rows = 1 month),
* I have considered 5 rows of data as one week for cyclical features (stock price data is available only weekdays).
* I used a Linear Regression model for time series forecasting (from River),



## Proposed Pipeline

<img width="1212" alt="Screenshot 2024-03-13 at 12 49 07 AM" src="https://github.com/john-fante/my-incremental-learning-projects/assets/50263592/ea75303d-ac1d-4db0-9a25-18409164e7be">




## References
1. https://en.wikipedia.org/wiki/Incremental_learning
2. https://riverml.xyz/dev/
