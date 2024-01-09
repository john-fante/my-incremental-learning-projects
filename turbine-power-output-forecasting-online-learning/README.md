## Turbine Power Output Forecasting w/Online Learning (River library)

(kaggle link -> https://www.kaggle.com/code/banddaniel/power-forecasting-w-online-learning-river)

First of all, I am very keen on trying new methods. This is why I tried an Online/Incremental Learning [1] method in this project for time series forecasting. 

In this method, our model learns from one sample of each training loop. Actually, this type of learning is very handy in the streaming data.

* I used **River** library for online/incremental learning[2],
* I created cyclical features at the feature engineering stage,
* I used a Linear Regression model for time series forecasting (from River),


## Proposed Pipeline

<img width="996" alt="download (45)" src="https://github.com/john-fante/my-incremental-learning-projects/assets/50263592/1a09528f-89f0-4320-9f34-aa2d7b4be39d">


## References
1. https://en.wikipedia.org/wiki/Incremental_learning
2. https://riverml.xyz/dev/
