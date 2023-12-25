## Smoking Detection w/Online Learning (River)

(kaggle link -> https://www.kaggle.com/code/banddaniel/smoking-detection-w-online-learning-river )

First of all, I am very keen on trying new methods. This is why I tried an Online/Incremental Learning [1] method in this project for image classification. 

In this method, our model learns from one sample of each training loop. Actually, this type of learning is very handy in the streaming data. In this project, I assumed that smoking detection could be done with a low frame rate camera.


<img width="1135" alt="download (31)" src="https://github.com/john-fante/my-incremental-learning-projects/assets/50263592/080638af-566c-424d-aecb-b22395813cf3">




* I used **River** library for online/incremental learning[2], 
* I used a mirrored strategy (using 2 T4 GPU at the same time),
* I used a customized ViT model [3],
* Used <b>tf.data</b> for input pipeline,
* I used a Linear Regression model for classification (from River),




## References
1. https://en.wikipedia.org/wiki/Incremental_learning
2. https://riverml.xyz/dev/
3. https://github.com/faustomorales/vit-keras
