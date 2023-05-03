# KNN:

**Dataset**
The load_wine() dataset is a classic dataset in machine learning used for classification tasks. It contains the results of a chemical analysis of wines grown in a specific area of Italy, with the aim of identifying the cultivar. The dataset has 13 numeric attributes that describe the properties of the wine, such as alcohol content, color intensity, and hue. The dataset has 178 instances and is often used as a benchmark for classification algorithms.


**Algorithm Explanation**
The following code performs a wine classification task using the K-Nearest Neighbors (KNN) algorithm. The dataset used is the Wine dataset from the Scikit-Learn library. The aim of this task is to classify wines into three classes based on their chemical attributes.

**Step 1: Data Preparation**
The Wine dataset is loaded using the load_wine function from Scikit-Learn. The input features are stored in a Pandas DataFrame, X, and the target variable is stored in a Pandas Series, y. The dropna method is then used to remove any null values from the dataset. The median filter is then applied to remove any noise from the dataset. Any missing values are then imputed with the mean value of the corresponding column. Finally, the data is normalized using the StandardScaler function from Scikit-Learn.

**Step 2: Feature Extraction**
Principal Component Analysis (PCA) is used to extract the most important features from the data. Three different PCA feature sets are created, PCA1, PCA2, and PCA3, each containing 3, 5, and 7 features, respectively. These feature sets are stored in a list, pca_list.

**Step 3: Model Training and Evaluation**
The dataset is split into training and testing sets using the train_test_split function from Scikit-Learn. For each PCA feature set in pca_list, a KNN classifier is trained using the training set. The number of neighbors used in the KNN classifier is set to 5. The accuracy of the classifier is evaluated using the testing set, and the accuracy score is printed to the console. The first two principal components of each feature set are also plotted for visualization purposes.

The best feature set is selected based on the highest accuracy score. The accuracy score and best feature set are printed to the console. Finally, the classification report and confusion matrix are generated to evaluate the performance of the best KNN classifier on the testing set.
