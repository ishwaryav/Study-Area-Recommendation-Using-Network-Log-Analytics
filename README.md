# Study-Area-Recommendation-Using-Network-Log-Analytics
The application recommends users of the San Jose State University's network, a place to perform work/entertainment activities by predicting the network usage of each access point for the next 4 hours and classifying them as being used for work/entertainment activities.

The application uses machine learning techniques to predict the availability of access points and categorize them into 2 classes – work and entertainment.

Classification Of Access Points Based On Browsing Data

Machine Learning Models used are:

1.  Random Forest 
2.  Gaussian Naive Bayes 
3.  XGBoost

Implementation: 

1.	Web scraper (a script implemented in Python) scrapes text from the URLs browsed by users of SJSU’s network
2.	Scraped text from URLs are manually classified into work/entertainment classes based on their content to aid the               classification algorithm in learning the data (also called as supervised learning).
3.	Efficiency of the algorithm is determined based on how well the algorithm is able learn and classify new uncategorized URL     texts
4.	The performance of the models are compared using a metric called F1-score
5.	Classification results are stored in a MySQL database for easy data retrieval


Prediction of Average Network Throughput of Access Points

Machine Learning Models used are:

1.  AutoRegressive Integrated Moving Average (ARIMA)
2.  Long Short-Term Memory (LSTM) 
3.  Facebook’s Prophet

Implementation:

1.  LSTM Model, one of recurrent neural networks is chosen to predict network usage in future and its performance is compared     with two baseline models ARIMA and Facebook Prophet
2.  Each model is trained using different sets of meta parameters, with network usage data from the past
3.  Models are evaluated using a metric called Mean Absolute Error (MAE) to determine the most efficient model

