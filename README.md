# willy402-HOMOGENEOUS-ENSEMBLE-RANDOM-FOREST.-
    # HOMOGENEOUS-ENSEMBLE-RANDOM-FOREST.


Churn Modelling Random Forest Example
 The goal of this example is to predict whether a customer will churn (i.e., close their account) based on a number of features such as their credit score, age, and number of products.




To run this example, you will need Python 3 and the following Python packages:

    pandas
    numpy
    scikit-learn
    matplotlib

You can install these packages using pip:

pip install pandas numpy scikit-learn matplotlib

Once you have installed the necessary packages, you can run the example by executing the random_forest_churn.py script in this repository:

python random_forest_churn.py

This will load the Churn Modelling dataset, preprocess the data, split it into training and testing sets, train a Random Forest classifier on the training data, and evaluate the classifier's performance on the testing data and the  accuracy score of the classifier will be printed to the console.


Results got from churning

When running this example, the accuracy score of the Random Forest classifier on the testing data was 0.865. This means that the classifier correctly predicted whether a customer would churn or not 86.5% of the time.

We also calculated the feature importances of the classifier to see which features were the most important for predicting churn. The features ae as follows

    Age (0.239)
    NumOfProducts (0.146)
    CreditScore (0.141)
    Balance (0.138)
    EstimatedSalary (0.136)
    Tenure (0.086)
    HasCrCard (0.021)
    Geography_Germany (0.020)
    IsActiveMember (0.018)
    Geography_France (0.012)
    Gender_Female (0.011)
    Gender_Male (0.011)
    Geography_Spain (0.010)

This suggests that a customer's age, the number of products they have, their credit score, and their balance are the most important factors in predicting whether they will churn.

Visualizing the Decision Trees

I have  used the plot_tree() function to visualize the first decision tree in the Random Forest and this has helped  me  understand how the classifier is making its predictions.

Random Forest Decision Tree

As we can see, the tree consists of a series of decision nodes that split the data based on certain features. Each leaf node represents a prediction of whether a customer will churn or not. By following the path from the root node to a leaf node, we can see how the classifier is making its prediction for a given customer.


    
