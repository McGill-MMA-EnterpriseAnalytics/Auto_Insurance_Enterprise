The dataset is one of the sample datasets obtained from IBM. It contains the results of an auto insurance company's marketing campaign which offers customers with expiring policies one of four different renewal proposals to retain them. The data has 9134 customer records with 24 variables. The policies for all customers expire between Jan 1 to Feb 28, 2011.

The main objective of the analysis is to understand different customer segments of an auto insurance company and understand how consumers are responding to different renewal offers. To understand the data and different customer segments, data exploration analysis and clustering using (K-means) was performed. Additionally, to understand what customers to target, a regression model was built to predict the customer lifetime value. Also, a classfication model was built to determine if a customer will accept or reject the renewal offer. Feature selection was done to determine the insignificant predictors and different machine learning algorithms such as Random Forest, Gradient Boosting Tree, XG Boost, Light GBM etc was used to build the models. Since the renewal acceptance rate was low, causal inference was done to see if any potential causes can be determined that are causing people to reject these offers and to better understand what strategy the company should adopt to get more engagement in terms of acceptance to renewal offers. 

**Challenges**

Some of the challenges that were faced while doing the analysis included having a high recall for some of our classification models. To manage this problem various factors were checked including:
1. Potential Data Leakage Sources: All the features were checked to see if there was anything that could lead to data leakage. Customer Lifetime Value (CLV) was determined to be one of the factors that could lead to data leakage because it could increase or decrease depending on a person's response to offers. Several other features that showed high feature importance was tested to see if they made a difference to recall, which wasn't the case.
2. Another potential reason of recall could be due to having similar customer data. This wasn't possible for our dataset because this data contained information of unique customers. 
3. Third potential reason could be due to time series: As mentioned this dataset only included people whose policies were going to expire within a certain time period. It was concluded that this might not be the reason for high recall. 
4. No data dictionary: This dataset did not have a data dictionary and another sources was used to come up with data dictionary. It is very likely that our interpretation of features might be incorrect. 
5. Synthetic datatset: This is synthetic dataset by IBM. Hence, there is a high likelihood that the potentially high recall by some of the algorithms could be attributed to this. 

In the end, the goal of this project was to work on a business idea and do analysis to derive insights, which we wer able to achieve. After all the analysis, we were able to come up with the following insights for the auto insurance company:
1. Focus on people with high predicted CLV and who would respond yes to consumers 
2. Target retired people and promote offer 2 

Future steps: 
1. Understand the consumer base to determine the type of offers that should be made available to consumers 
2. Personalizing the offer types, which can lead to higher acceptance rate 
3. Understanding 'why' some of the offers ar enot working by talking to customers. 


Link to the dataset: https://www.kaggle.com/pankajjsh06/ibm-watson-marketing-customer-value-data

**Refer to the Final Files folder for all the modelling notebooks.
**__
