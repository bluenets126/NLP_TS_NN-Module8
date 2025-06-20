# NLP_TS_NN-Module8
Final Summative Lab


Created three seperate files.  One for each section.  

NLP is for Natural language processing

TSF is for Time Searies Forecasting

NN is for Neural Networks


NLP
In the NLP i used Random Search instead of Grid search.  Grid search was taking too long to run with the parameters so I switched to random search to find the best model and used that for the predictions.  
Preprocessing - I cleaned up the text by removing numbers, punctuations, and any HTML tags that might exist.  Then lemmentized the text
Tried fitting a model using Bag of words and TF-IDF, TF-IDF was the better one.  So for the random search i only used TF-IDF to save time.
Function created for prediction, and created 5 examples to test accuracy


TSF
For this I was messing around with the data in the beginning.  I ended up putting the data into a new DF called df.
I checked for seasonality and didn't find anything.  
Used a package found called pmdarima to find the best parameters for the ARIMA model.
Fitted a model on both the normal GSPC and log GSPC.  Foudn that the log was more accurate.  Lower MAE and RMSE.  


NN
Used different optimizers and activations.  When checking performance on them, the output varied from time to time.  The best outcome I came out with was to use Adam with Tanh activation.  98% Accurate
