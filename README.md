# Sarcasm Detection from Bengali Text

Sarcasm detection is the process of identifying whether a piece of text is sarcastic or not. Sarcasm is one of the main challenges for sentiment analysis systems. This is because a sarcastic sentence usually carries a negative implicit sentiment, while it is expressed using positive expressions. This contradiction between the surface sentiment and the intended one creates a complex challenge for sentiment analysis systems. Sarcasm detection received attention in other languages, but Bengali still lags behind. There is a broader business and educational interest in developing a Bengali AI tool to identify sarcastic content. In this regard, We, Department of Electronics and Telecommunication Engineering (ETE), CUET, is elated to present an NLP competition, as a part of ETE DecaHertz 2022.

Competetion link: https://www.kaggle.com/competitions/nlp-competition-cuet-ete-day-2022/overview

Leaderboard: https://www.kaggle.com/competitions/nlp-competition-cuet-ete-day-2022/leaderboard


## Train Dataset Visualization:

* ### Label Distribution

![alt text](https://github.com/sahasourav17/ML-Competition-CUET-ETE-Day-2022/blob/main/Label_Distribution.png?raw=true)

From label distribution, we can see that the dataset is imbalanced. As deep learning model can handle imbalanced dataset, we didn't need to use upsampling and downsampling technique.

#### Problems of Upsampling and Downsampling:
If we do downsampling , our model will lose vast amount of potential Data.
If we do upsampling, our model will lose it generalization ability.

* ### Data Statistics

![alt text](https://github.com/sahasourav17/ML-Competition-CUET-ETE-Day-2022/blob/main/Data_Statistics.png?raw=true)

* ### Frequency Length Distribution

![alt text](https://github.com/sahasourav17/ML-Competition-CUET-ETE-Day-2022/blob/main/Frequency_Length_Distribution.png?raw=true)

From frequency length distribution, we can find out the maximum,minimum and average length of our training data which will guide us during Tokenization and Model creation phase.

## Model Architecture:

Here, I've lately fused four model to build a Fusion model. No word embedding is used.
Models I've used:

* BiGRU (Bidirectional Gated Recurrent Unit)
* BiLSTM (Bidirectional Long Short Term Memory)
* BiGRU + CNN (Hybrid Model)
* BiLSTM + CNN (Hybrid Model)

![alt text](https://github.com/sahasourav17/ML-Competition-CUET-ETE-Day-2022/blob/main/Model_Architecture.png?raw=true)

## Model Evaluation:

* ### Accuracy Curve

![alt text](https://github.com/sahasourav17/ML-Competition-CUET-ETE-Day-2022/blob/main/Accuracy_Curve.png?raw=true)

* ### Loss Curve

![alt text](https://github.com/sahasourav17/ML-Competition-CUET-ETE-Day-2022/blob/main/Loss_Curve.png?raw=true)


## Accuracy: 86.308%
