---
title: "Multivariate Stock Price Prediction Model (BUET, earlier work)"
excerpt: "RNN with LSTM model on DSE data"
collection: projects
---
It was part of final year ML course project. This project have two sub-systems: <br />
*Data Collection:* Mined stock related trade information since January, 2012 to June, 2018 from [Dhaka Stock Exchange](https://www.dsebd.org) website. We later installed an auto update feature to it to continuously monitor price changes within a day. <br />
*Prediction Model:* Designed and deployed a RNN with LSTM model for predicting stock price trends. Although as a learning project it were successful, we would highly discourage anyone to invest following any such ML based prediction. <br />
*We are also skeptical about any large scale accurate stock price predictor as the stock market resembles an type 2 chaotic system that reacts to the prediction itself.*

*Applied Technologies:*
* Tensorflow & Keras: For model Development
* Selenium (Java) & JSoup: For automated data capture, parsing & building dataset.
