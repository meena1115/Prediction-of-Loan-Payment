# Prediction-of-Loan-Payment
# Data Analysis on predicting Loan Payment
CODE:
#Logistic Regression 
from sklearn.linear_model import LogisticRegression 
l1=LogisticRegression() 
l1.fit(xtrain,ytrain) 
yp1=l1.predict(xtest)
from sklearn.metrics import accuracy_score,precision_score,recall_score,f1_score 
from sklearn.metrics import classification_report,confusion_matrix 
from sklearn.metrics import roc_curve, roc_auc_score 
print(" accuracy is ",accuracy_score(ytest,yp1)) 
print(" precision score is ",precision_score(ytest,yp1)) 
print(" recall is ",recall_score(ytest,yp1)) 
print(" f1 score is ",f1_score(ytest,yp1)) 

************************      RESULTS    **********************************
accuracy 	 	0.5928753180661578 
precision score  	0.5163043478260869 
recall 			0.572289156626506 
f1 score 		0.5428571428571428
confusion matrix    	[[138 89] 
                      [ 71 95]] 
****************************************************************************
CODE:
#Descision Tree 
from sklearn.tree import DecisionTreeClassifier 
d1=DecisionTreeClassifier() 
d1.fit(xtrain,ytrain) 
yp2=d1.predict(xtest) 
************************      RESULTS    **********************************
accuracy	 	0.5725190839694656 
precision score 	0.49473684210526314 
recall  			0.5662650602409639 
f1 score 		0.5280898876404494 
confusion matrix 	[[131 96] 
                   [ 72 94]] 
****************************************************************************
CODE:
from sklearn.neighbors import KNeighborsClassifier 
#DEFAULT value is 5 number of neighbours to be used for k neigbour queries 
knn5 = KNeighborsClassifier(n_neighbors = 5) 
#Value changed and now only 1 neighbour to be used for k neigbour queries 
knn1 = KNeighborsClassifier(n_neighbors=1)
knn5.fit(xtrain,ytrain) 
yp3=knn5.predict(xtest) 
knn1.fit(xtrain,ytrain) 
yp4=knn1.predict(xtest) 

************************      RESULTS    **********************************
accuracy 		 0.5725190839694656 
precision score 	 0.4941860465116279 
recall 			 0.5120481927710844 
f1 score 		 0.5029585798816567 
confusion matrix 	  [[140 87] 
                    [ 81 85]]
                    
****************************************************************************
