Objective:

In our project, we use Kaggle data to forecast possible future defaulters so that the consumer can be authorized for a loan offer. We used Python code to create our data visualizations. Furthermore, we evaluate multiple machine learning models, such as logistic regression, decision trees and KNN model to determine the best model that will assist the lender to predict customer behavior. 
Based on our predictive model, the lenders will decide which applicants will be approved and who will not be approved.

Data and Preprocess data:

In this dataset, we have 13 variables, which are Loan_ID, Credit_History, Self_Employed, Gender, Dependents, Married, Loan_Amount_Term, LoanAmount, and Loan_Status, with 981 instances. On Kaggle, we were provided with two datasets. Therefore, we concatenate both sets of data and sort them by Loan_ID. 

Solution Methodology using Machine Learning Models:

As previously stated, our primary goal is to assist lenders in determining whether a borrower is risky or not. We can accomplish this by developing and comparing multiple machine learning models and algorithms, then selecting the best model to assist the lender in predicting the borrower's behavior. Using these models and results, the lender can also approve or deny the loan early on.
A model for machine learning is a file that has been programmed to recognize specific patterns. We train a model using a set of data and provide it with an algorithm that it can use to reason about and learn from the data. Once the model has been trained, you can use it to reason over data that it hasn't seen before and make predictions about it. We used the following models for our project:
 
 Logistic Regression 

One of the machine learning technique used for classification issues is logistic regression. It is a predictive analysis algorithm, based on the concept of probability. Logistic regression is a statistical analysis method analyzes previous observations from a data set to predict the binary outcome, such as yes or no,0 or 1.

Decision Tree

A decision tree is a flowchart-like structure in which each internal node represents a "test" on an attribute (e.g. whether a coin flip comes up heads or tails), each branch represents the outcome of the test, and each leaf node represents a class label (decision taken after computing all attributes). The paths from root to leaf represent classification rules. In decision analysis, a decision tree and the closely related influence diagram are used as a
visual and analytical decision support tool, where the expected values (or expected utility) of
competing alternatives are calculated. A decision tree consists of three types of nodes:
	Decision nodes – typically represented by squares
	Chance nodes – typically represented by circles
	End nodes – typically represented by triangles

K-nearest neighbors(KNN) 

The k-nearest neighbors algorithm (k-NN) is a non-parametric classification method. It is used 
for classification and regression.
	In k-NN classification, the output is a class membership. An object is classified by a 
plurality vote of its neighbors, with the object being assigned to the class most common 
among its k nearest neighbors (k is a positive integer, typically small). If k = 1, then the 
object is simply assigned to the class of that single nearest neighbor.
	In k-NN regression, the output is the property value for the object. This value is the 
average of the values of k nearest neighbors.

NEURAL NETWORK MODEL:

Neural networks are comprised of a node layers, containing an input layer, one or more hidden layers, and an output layer. Each node, or artificial neuron, connects to another and has an associated weight and threshold. If the output of any individual node is above the specified threshold value, that node is activated, sending data to the next layer of the network. Otherwise, no data is passed along to the next layer of the network.

Comparison among different models:

Logistic Regression	Decision Tree	KNN	Neural Network
Accuracy	 0.592	 0.572	 0.572	0.842 
Precision Score	 0.516	 0.494	 0.494	 0.863
Recall	 0.572	 0.512	 0.512	 0.926
F1- Score	 0.542	 0.528	 0.502	 0.894
ROC_AUC_score	 0.646	 0.619	0.592 	 0.803

By considering all the metrics from the above for  the evaluation and found out that the Neural Network
has the highest metrics over all the other models. So we have chosen Neural Network as 
our best model for predicting our objective. 


