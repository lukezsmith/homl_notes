# Questions
1. The depth of a well-balanced binary tree with m leaves is log2(m). As we have 1 million instances, m = 1 million and thus equals approximately log2(10^6) = 20. However, in reality there will be more depth than this as the tree will not be perfectly balanced. 
2. A node's gini impurity is generally lower than its parent's. This is because the cost function splits each node in such a way that each node's children have a minimised gini impurity. However, it is possible that a child has a higher impurity than its parent if it is the case that another child has a significantly lower gini impurity than that same parent. 
3. Yes, as reducing tree depth is a form of regularisation.
4. No, decision trees do not require feature scaling, modifying them will be a waste of time.
5. The computational complexity of training a decision tree is O(nxmxlog(m)) and thus, computing this means that training a dataset of 10million instances will take around 11.7 hours
6. Presorting dataset only yields a quicker training time if the number of instances is below a few thousand. Otherwise, it actually slows down training. 
7. 