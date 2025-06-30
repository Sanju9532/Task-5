Introduction:
        Importing the dataset, checking data types and null values, and performing some statistical analysis. This is a classification dataset, so we split the input and output variables 
and perform a train-test split. Next, I build a Decision Tree model, visualize the tree, and tune hyperparameters using GridSearchCV. After that,I build a Random Forest model and comparing 
the accuracy of the Decision Tree and Random Forest. Also examine feature importances and finally evaluate the models using cross-validation.

Decision Tree Model: 
        I split the dataset into x and y, and then performed a train-test split. Next, I built a Decision Tree classifier model and achieved good scores on both the training and testing sets,
but it was not perfect; the model was slightly overfitted, with a training recall score of 1.0 and a testing recall score of 0.97. I then visualized the tree and proceeded to tune some 
hyperparameters using GridSearchCV, reducing the tree depth from 9 to 5. However, this resulted in lower scores compared to the original Decision Tree, with a training recall of 0.95 and a 
testing recall of 0.90, followed by another visualization of the tree and I saved the model for future use.

Random Forest Model: 
        I built a Random Forest classifier model and used evaluation metrics such as accuracy, recall, precision, and F1-score. I achieved a perfect score of 1.0 for all metrics, indicating 
that it is an excellent model. I saved the model for future use. Then, I compared the accuracy of the Decision Tree and Random Forest models, finding that the Random Forest had a significantly 
better score. I interpreted feature importances by visualizing a bar plot, which showed that some features had a strong relationship with the target variable while others had a weak relationship.
Finally, I evaluated the model using cross-validation, where the Random Forest achieved a mean score of 0.997, compared to 0.993 for the Decision Tree.

Conclusion:
        The Random Forest model outperformed the Decision Tree model, achieving perfect evaluation metrics and a mean cross-validation score of 0.997. The analysis of feature importances 
revealed valuable insights into predictor relationships. Overall, the Random Forest proved to be an effective and reliable classification model, and it has been saved for future use.
