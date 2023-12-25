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


## My Another Projects
* [Mammals Classification w/Ensemble Deep Learning](https://www.kaggle.com/code/banddaniel/mammals-classification-w-ensemble-deep-learning)
* [Bladder Tissue Classification w/ViT (F1 Scr: 0.82)](https://www.kaggle.com/code/banddaniel/bladder-tissue-classification-w-vit-f1-scr-0-82)
* [Segment Medical Instrument, w/Custom DeepLabv3+(Dice: 0.86)](https://www.kaggle.com/code/banddaniel/segment-medical-instrument-deeplabv3-dice-0-86)
* [Jellyfish Detect (10CV Custom ConvMixer) (F1:0.87)](https://www.kaggle.com/code/banddaniel/jellyfish-detect-10cv-custom-convmixer-f1-0-87)


## References
1. https://en.wikipedia.org/wiki/Incremental_learning
2. https://riverml.xyz/dev/
3. https://github.com/faustomorales/vit-keras
