# Predicting Clothing Item Fit
USF MSDS Machine Learning Lab - Group Project

#### Data: Rent The Runway Clothing Fit Feedback
Rent the Runway is a billion dollar clothing rental service that's trying to transform how women shop

![alt text](https://socialmediaweek.org/wp-content/blogs.dir/1/files/rtr-1.jpg)

Our dataset is from the publication:

Rishabh Misra, Mengting Wan, Julian McAuley "Decomposing Fit Semantics for Product Size Recommendation in Metric Spaces". RecSys, 2018. https://rishabhmisra.github.io/publications/


#### About this dataset:       
a> Number of customers: 105,508   
b> Number of products: 5,850    
c> Number of transactions: 192,544 

#### Contributors:

Esther Liu  
Arthur Qin  
Sakshi Singla

#### Goal:

In today's world where the fast fashion industry is the second biggest polluter on earth, how can we use data science to help reduce the carbon footprint this industry has created?

We look at Rent the Runway's dataset to see if we can predict whether the particular item on Rent the Runway will fit the customer or not based on past data collected for that item.

Our model hopes to help reduce the cost and carbon footprint of shipping, as well as reducing the barriers to entry for a platform like Rent the Runway.


#### Process - Feature Engineering:

1. Cleaning and extracting variables to convert them to numeric values
2. Frequency encoding for some variables
3. Label encoding the categorical variables
4. Balanced the dataset 

#### Data Modeling:

Pipeline 
1. Simple Imputer with strategy='median'
2. Standard Scaler - Applied to k-nearest neighbors (KNN) and Logistic Regression 
3. Models fitted - RandomForestClassifier, GaussianNB, KNeighborsClassifier, LogisticRegression
4. Hyperparameters tuning

#### Model Evaluation:

Compared various fitted model on basis on evaluation of validation set on metric: Accuracy and F1 score

#### Conclusion:

Random forest performs the best for modeling our data.
We could use size of the item, rating of the item, and a customer’s weight to provide item recommendation.

