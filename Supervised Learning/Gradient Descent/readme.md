# Comparing Adam and Mini-batch Gradient Descent for Binary Classification
This code compares two popular optimization algorithms, Adam and Mini-batch Gradient Descent, for binary classification on a breast cancer dataset. The goal is to predict whether a tumor is malignant (cancerous) or benign (non-cancerous) based on various features.

**Dataset**
The dataset used in this code is the Breast Cancer Wisconsin (Diagnostic) Data Set from the UCI Machine Learning Repository. The dataset consists of 569 instances, with 30 features for each instance. The target variable is the diagnosis of the tumor, which is either M (malignant) or B (benign).

**Preprocessing**
Before training the models, the following preprocessing steps are performed on the data:

Dropping unnecessary columns (id and Unnamed: 32)
Converting the diagnosis labels to binary values (M = 1, B = 0)
Splitting the data into training and testing sets (80% for training, 20% for testing)
Standardizing the features using StandardScaler
Adding an intercept term to the feature matrix
Adam Optimization
Adam is a popular optimization algorithm for training deep neural networks. It combines the ideas of Momentum and RMSprop to achieve faster convergence. The hyperparameters for Adam used in this code are:

Learning rate (learning_rate) = 0.0001
Number of iterations (iterations) = 500
Exponential decay rates for the first and second moment estimates (beta1 and beta2) = 0.9 and 0.999, respectively
Small constant (epsilon) to prevent division by zero
The Adam algorithm is implemented using a loop that iteratively computes gradients and updates the parameters. The sigmoid function is used as the activation function, and the binary cross-entropy loss function is used to evaluate the cost.

The accuracy of the model on the test set is reported at the end of the loop.

**Mini-batch Gradient Descent**
Mini-batch Gradient Descent is another popular optimization algorithm for training machine learning models. Unlike Adam, which updates the parameters after every iteration, Mini-batch Gradient Descent updates the parameters after processing a small batch of examples at a time. This can speed up the convergence and reduce memory usage.

The hyperparameters for Mini-batch Gradient Descent used in this code are:

Learning rate (learning_rate) = 0.0001
Number of iterations (iterations) = 500
Batch size (batch_size) = 32
The Mini-batch Gradient Descent algorithm is implemented using a loop that iteratively processes mini-batches of examples and updates the parameters. The sigmoid function is used as the activation function, and the binary cross-entropy loss function is used to evaluate the cost.

The weights, bias, and cost history of the model are returned at the end of the loop. The accuracy of the model on the test set is computed using the weights and bias.

**Conclusion**
This code demonstrates how to implement two popular optimization algorithms, Adam and Mini-batch Gradient Descent, for binary classification. The accuracy of both algorithms can be compared to determine which one works best for a given dataset and problem.
