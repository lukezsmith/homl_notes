# Questions
1. The fundamental idea behind an SVM is to fit the widest possible street between the classes such that there is a compromise between perfectly seperating the classes and having the widest margin. Another key point is using kernels when training on nonlinear datasets in order to speed training up.
2. After training an SVM, a support vector is any instance located on the 'street' or its border. The decision boundary is entirely determined by the support vectors.
3. Because SVM tries to fit the largest possible 'street' and so any features with small scales will be neglected in favour of larger ones.
4. An SVM classifier can output the distance between the test instance and the decision boundary which can be used as a confidence score. However, this cannot be converted to an estimation of class probability. Setting probability=True will instruct skl to perform logistic regression on svm's scores in order to give probabilities to the SVM. 
5. If you have a very large dataset, used primal. 
6. If an SVM classifier trainied with an RBF kernel is underfitting it means that there might be too much regularisation and more specifically, one of two things: gamma parameter is too low or c parameter is too low (or both)
7. 