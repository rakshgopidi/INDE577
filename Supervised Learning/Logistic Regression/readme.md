# Insurance Purchase Prediction using Logistic Regression
**Introduction**
The aim of this project is to use logistic regression to predict whether a person will purchase insurance or not based on their age. In this code, we will use scikit-learn library to build a logistic regression model on a dataset that contains two columns: age and bought_insurance.

**Dataset Description**
The dataset used in this code is an insurance dataset that contains two columns: age and bought_insurance. The age column contains the age of a person, and the bought_insurance column contains the information whether the person bought insurance or not. The dataset contains 27 rows.

**Algorithm**
Logistic regression is a statistical method that is used to analyze and model the relationship between a binary dependent variable (in this case, whether a person bought insurance or not) and one or more independent variables (in this case, age). The logistic regression model uses a sigmoid function to transform the linear regression output into a probability score between 0 and 1. If the probability score is greater than a certain threshold, the person is predicted to have bought insurance, otherwise not.

**Model Description**
The first step in building a logistic regression model is to split the dataset into training and testing sets. In this code, we use 80% of the dataset for training the model and 20% for testing the model. After splitting the dataset, we use scikit-learn's LogisticRegression() class to build the logistic regression model. The model is trained on the training set and tested on the testing set to predict the probability of a person buying insurance given their age.

**Performance Analysis**
The performance of the model is evaluated using the confusion matrix and classification report. The confusion matrix shows the number of true positives, false positives, true negatives, and false negatives. The classification report shows the precision, recall, f1-score, and support for each class (bought insurance and did not buy insurance). The model achieves a high accuracy score on the testing set, which suggests that age is a strong predictor of insurance purchase.

**Conclusion**
In conclusion, this code demonstrates how logistic regression can be used to predict whether a person will buy insurance or not based on their age. The logistic regression model achieves a high accuracy score on the testing set, indicating that age is a significant factor in determining insurance purchase. This code can be used as a starting point for analyzing larger insurance datasets or for building more sophisticated machine learning models.
