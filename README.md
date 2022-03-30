# hotel_recommendation

## Hotel Recommendation System

**Introduction**

A hotel recommendation system typically works on collaborative filtering that makes recommendations based on ratings given by other customers in the same category as the user looking for a product.

**Objective**

Analyze the dataset and identify the most relevant parameters that recommends users for a hotel booking or reservations as per the user personalization. In this context, study the customer data and predict the feasibility or probability whether user will stay at different group of hotels. It is therefore also our approach to build a recommendation system based on customer reviews and ratings. So, use the ratings and reviews given by customers who belong to the same category as the user and build a hotel recommendation system.

**Dataset**

The dataset, ***Hotel_Reviews.csv***, is taken from Kaggle. This dataset contains data about reviews of some thousands of customers mentioning *Hotel Address*, *Review Date*, *Average Score*, *Hotel Name*, *Total Number of Reviews*, *Positive Reviews* etc. There are nearly 15 features in this dataset.

**Perform the following tasks:**
1) Write a Data Science Proposal for achieving the objective mentioned
2) Perform exploratory data analysis on the data and describe your understanding of the data
3) Perform data wrangling/pre-processing, e.g., missing data, normalization, discretization, etc.
4) Apply any two feature selection engineering techniques
5) Compare the two selected feature engineering techniques
6) Plot top 5, 6, and 8 features
7) Provide a high-level description of Machine Learning models – Logistic regression and Decision tree to predict
8) Compare the performance of the two classifiers – Logistic regression and Decision tree to predict
9) Present the conclusions

## Inferences

**Overview**
 - *Objective:* Recommends users for a hotel booking or reservations as per the user personalization. Approach is to build a recommendation system based on customer reviews and ratings
- *Methodology:* Use the ratings and reviews given by customers who belong to the same category as the user and build a hotel recommendation system for the UK and Netherlands

**Dataset**
 - *How many features* – 16 feature variables and a target variable
 - *Size of the dataset* – 1699 rows and 17 columns
 - *Multiple files* – No
 - *What kind of data* – Nominal, Ordinal and Numeric data. Target variable is numeric
 - *Balanced or imbalanced* – Data seems to be mostly balanced
 - *Distribution of training set, validation set, testing set* – 80% (train set), 20% (test set)
 - *Missing data and Preprocessing challenges* – No missing data

**Feature Engineering Techniques**
 - Feature Removal
 - Feature Creation
 - Feature Ranking
 - Class Imbalance Treatment
 - Other <br/>
	 Performed Standard Scalar transformation across all input variables so that the model is more balanced while predicting and is not biased towards variables with larger values

**Methodology**
 - The 3 classifiers used
 - Ensemble pipeline
 - Other models considered
 - Hyper-parameter tuning<br/>
     ```
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, shuffle=True)
     dt_model = DecisionTreeClassifier()
     dt_model.fit(X_train, y_train)
     lr_model = LogisticRegression()
     lr_model.fit(X_train, y_train)
     ```
