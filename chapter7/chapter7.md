# Questions
1. Yes, there is a chance that combining them together into a voting ensemble will produce a more accurate model. It is better if all of the models are different from each other, and even better if they are trained on different types of data.
2. Hard voting classifiers simply use the class that has received the most votes of each classifier. Soft voting takes an average estimated class probability for aech class and picks the class with the highest probability. Hence, it gives high-confidence classifications more weight. 
3. Yes, it is possible to train multiple classifiers for a bagging ensemble in parallel as each predictor is independent from each other. The same is true for pasting ensembles and random forests for the same reason. The same cannot be said for gradient boosting as each predictor is trained on the previous predictor's weights or residual errors depending on the type. Hence, sequential training ios required for these. Stacking ensembles can be trained in parallel however the predictors in one layer can only be trained after the predctors in the previous layer have been trained. 
4. Out of bag evaluation removes the need for a validation set as each predictor in a bagging ensemble will be evaluated on data it has not been trained on. Hence, each bag shares data between each other for training and validation in a manner that is unbiased much like having a training and validation set. The benefit of this is that you have more data to train with rather than setting aside a large portion for simply validating the model.
5. When you are training a tree in a random forest, we randomise the feature selected for each split and we then search for the best possible thresholds for that feature. With Extra Trees we also randomise the threshold value so it is in a sense, more random. It will be quicker as a result of not having to compute the best possible threshold for each tree. Due to this increased randomness, if a standard random forest is overfitting, the extra trees implementation may perform (generalise) better. 
6. If Adaboost underfits then you can try increasing the number of estimators or try reducing regularisation hyperparameters of the base estimator. You can also try incrasing the learning rate slightly. 
7. If Gradient boost ensemble is overfitting we should decrease the learning rate as we multiply each predictor's weight by this value and thus, a higher predictor weight means stronger fit to the training data.