# Cryptocurrency-Price-Predictor

> **Cryptocurrency** is a type of online payment that may be used to buy and sell products and services. Many businesses have created their own currencies, known as tokens, that can be exchanged for the goods or services that the business offers. Consider them to be arcade tokens or casino chips. To use the good or service, you'll need to convert actual money for cryptocurrency. is the technology that enables cryptocurrency to function. is a technology that handles and records transactions across numerous computers. The security of this technology is part of its attractiveness.
> 
> We'll look at three of the most well-known ones in this study. As a result, it aims to do the following by employing machine learning algorithms that can uncover hidden patterns in data, integrate them, and generate considerably more accurate predictions:
  * Providing a complete examination of the many existing techniques for predicting the prices of Bitcoin, Ethereum, and (BTC, ETH, and   LTC, respectively).
  * For prediction, a deep learning method called long short-term memory (LSTM) has been used.
The main goal is to develop a trustworthy prediction model based on historical values that investors can trust.

 ### **Dataset used in this Project**

We are training our pricing model, using public price data of cryptocurrencies reported from Jan 1st, 2018 to Dec 31, 2020 downloaded from Yahoo Finance. For testing our model, we use the price data of cryptocurrencies from Jan 1st 2021 to present date. We use the model to predict the crytocurrency prices for this period and compare it to the actual prices to check the efficiency of this model in predicting the prices.



### **Model have used for prediction**

We are using a multilayer RNN Long Term Short Term Memory (LSTM) model having 3 LSTM layers with each layer followed by a dropout layer (with 20% dropout frequency) and at last have used a Dense layer to produce the predicted price.

In RNN, the information goes through a cycle. When making a decision, it considers the current input and also what it has learned from the inputs it has received previously.

### **Problems with our approach**

The RNN-LSTM model that we have used to predict the prices of crypto currency is very accurate on the test data, however, it fails to predict the prices very accurately for the long term. We observed that the model can be used for predicting prices only for the next 5-7 days without significant loss in accuracy. That is why we have only used the model to predict the prices for the next 7 days.

### **Implementation**

The Implementation can be found in the model.ipynb file
