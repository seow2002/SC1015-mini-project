<h1> Credit Card Churn </h1>

<h2> About </h2>
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence which focuses on credit card churn from <a href = "https://www.kaggle.com/sakshigoyal7/credit-card-customers?select=BankChurners.csv"> this Kaggle data set</a>. For detailed walkthrough, refer to the source code in order:

1. <a href = "https://github.com/silverarrows22/SC1015-mini-project/blob/main/Data%20Visualisation%20with%20EDA.ipynb">Data Visualisation with EDA</a>
2. <a href = "https://github.com/silverarrows22/SC1015-mini-project/blob/main/Logistic%20Regression%20(one-hot%20encoding).ipynb">Machine Learning: Logistic Regression</a>
3. <a href = "https://github.com/silverarrows22/SC1015-mini-project/blob/main/Naive%20Bayes%20(one-hot%20encoding).ipynb">Machine Learning: Naive Bayes</a>
4. <a href = "https://github.com/silverarrows22/SC1015-mini-project/blob/main/Decision%20Tree%20(one-hot%20encoding).ipynb">Machine Learning: Decision Tree</a>
5. <a href = "https://github.com/silverarrows22/SC1015-mini-project/blob/main/Random%20Forest%20(one-hot%20encoding).ipynb">Machine Learning: Random Forest</a>

<h2> Contributors </h2>
Phoebe C - Machine Learning: Logistic Regression, Decision Tree, Naive Bayes, Random Forest <br>
Nagammai S - Exploratory Data Analysis, Decision Tree, Logistic Regression <br>
Melissa S - Data Preparation, Logistic Regression <br>

<h2> Problem Definition </h2>
Are we able to predict which customers are more likely to carry out credit card churning?

<h2> Models Used </h2>
<h4> Regression (Logistic, Decision Tree, Random Forest) </h4>
We used multiple machine learning models to find a solution for our problem: <br>

<b> Logistic regression </b> is a supervised learning technique. Attrition_Flag is defined as the customer activity (ie. attrited customers vs existing customers) which is a categorical variable. Since this categorical variable is our dependent variable, we chose to use logistic regression instead of simple regression. However, it must be noted that as logistic regression uses all the variables in the regression equation, it may result in lower accuracy. <br>

<b> Decision tree </b> also uses the supervised learning technique. The tree-like model allows the decisions to be represented in a clear and well-defined manner. Moreover, decision tree has a higher accuracy compared to logistic regression. Since the decision tree has high variance and requires complex calculations if there are many class variables, we used the random forest, which is made up of multiple decision trees. A random forest is more efficient with large datasets, and is also more accurate compared to decision tree. <br>

<h2> Learning Points </h2>
<ul>
  <li> Naive Bayes </li>
  <dd>Assuming that the predictors are independent and with lesser training data, Naive Bayes was used to predict the class of the data. Naive Bayes finds the probabilities of each variable and predicts the variable with the highest probability. The accuracy and speed of Naive Bayes classifier is high even for large datasets. </dd>
  <li> Resampling the data </li>
  <dd> To improve the accuracy and to balance out the classes, the data was resampled. Some of the variables from the minority classes were duplicated in order to balance the classes. </dd>
  <li> One-Hot Encoding </li>
  <dd> Prediction and accuracy are improved as one-hot encoding converts the categorical variables so that they can be used in the algorithms. Categorical variables are represented as binary vectors by mapping the categorical variables to integers. Except for the index, the other integer values are all zero. Moreover, one-hot encoding ensures that machine learning does not value higher numbers. </dd>
  <li> Calculating permutation importance </li>
  <dd> The change in the prediction error of the model can be measured by permutation importance. When each of the predictor variables are shuffled in a random manner, the accuracy of the model will be monitored. Permutation importance observed the changes in the accuracy of the model and would measure the importance of the variable directly. </dd>
</ul>

<h2> Conclusion </h2>
Total Transaction Count, Total revolving balance, total change in transaction count from Q4 to Q1 are the variables that are closely correlated to churn rate.
These variables can be used to predict which customers are more likely to potentially carry out credit card churning.
<br>
Decision Forest has the highest accuracy and therefore is the most optimal model for predicting churn rate.
Hence, we are able to predict which customers are more likely to carry out credit card churning

<h2> References </h2>
Feature importance in naive Bayes classifiers. InBlog. (n.d.). Retrieved April 24, 2022, from https://blog.ineuron.ai/Feature-Importance-in-Naive-Bayes-Classifiers-5qob5d5sFW#:~:text=Feature%20importance%20is%20the%20methodology,are%20in%20predicting%20target%20variable <br>
Goyal, S. (2020, November 19). Credit Card customers. Kaggle. Retrieved April 24, 2022, from https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers?select=BankChurners.csv <br>
Supervised learning. scikit. (n.d.). Retrieved April 24, 2022, from https://scikit-learn.org/stable/supervised_learning.html  <br>
