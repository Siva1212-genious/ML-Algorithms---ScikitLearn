1. model.coef_

2. model.intercept_

3. model.feature_names_in_ — feature names

4. model.classes_ — classes learned by a classifier

5. model.n_features_in_ — number of input features

6. model.n_iter_ — number of iterations

7. model.get_params() — parameters YOU gave the model

8. model.score() — model score

9. model.predict() — predictions

10. model.predict_proba() — probabilities

11. model.feature_importances_

12. model.tree_ — underlying tree structure

13. model.n_estimators_ / model.estimators_


1. Things the model LEARNED

Usually have _ at the end:

model.coef_
model.intercept_
model.classes_
model.feature_names_in_
model.n_features_in_
model.feature_importances_
model.n_iter_




2. Things YOU SET — hyperparameters

Usually don't have _:

model.max_depth
model.min_samples_split
model.min_samples_leaf
model.criterion
model.n_estimators
model.learning_rate
model.C
model.max_iter


3.Things you ASK the model to do

Methods:

model.fit()
model.predict()
model.predict_proba()
model.score()
model.get_params()





A simple cheat sheet

Item	                     Meaning	                            Common models
coef_	Learned           feature weights	                    Linear/Logistic Regression
intercept_	          Learned bias/intercept	              Linear/Logistic Regression
feature_names_in_	    Feature names used during training	     Many sklearn models
n_features_in_	      Number of input features	               Many sklearn models
classes_	                Classes learned	                        Classifiers
feature_importances_	 Importance of features	               Decision Tree/Random Forest
n_iter_	                Training iterations	                   Logistic/SGD etc.
tree_	Internal            tree structure	                      Decision Tree
estimators_	             Individual trees	                       Random Forest
max_depth	            Maximum allowed tree depth	           Decision Tree/Random Forest
min_samples_split	   Minimum samples needed to split	       Decision Tree/Random Forest
min_samples_leaf	   Minimum samples in a leaf	             Decision Tree/Random Forest
n_estimators	          Number of trees	                           Random Forest
criterion	            How split quality is measured	                Tree/Forest
get_params()	          Shows model configuration	            Most sklearn models
predict()	               Makes predictions	                      Most models
predict_proba()	        Gives class probabilities	              Many classifiers
score()	                    Returns estimator-specific score	      Most models
