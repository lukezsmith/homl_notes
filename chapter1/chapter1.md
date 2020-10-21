- Notes

  - Sample data super important
  - Sample size problems:
    - Sampling noise: where sample size is too small
    - Sampling boas: where sample size is too large
  - Overfitting: when your model is too specific to the training data it is supplied and therefore has trouble generalising to other data
  - Underfitting: when your model is too simple to learn the underlying structure of the data
  - ML project roadmap:
    - Gather data into a training set
    - Feed training set to a learning algorithm
      - If the learning algorithm is model-based it will tune some parameters to fit the model to the training set: finds the correct parameters such that the model makes good predictions on the training set itself and thus hopefully on new cases it sees
      - Alternatively, if the learning algorithm is instance-based it will learn the training set examples by heart and then extrapolates to new instances by comparing similarity to original training data

- Exercises:
  1. Machine learning concerns building systems that can learn from data, where the definition of learning is to get better at some task.
  2. Problems with no algorithmic solutions, replace long, manually completed tasks, problems that exist in fluctuating environments and problems that help humans learn.
  3. A labelled training set is one that contains the desired solution (label) for each instance
  4. Regression & classification
  5. Clustering, visualisation, dimensionality reduction and association rule learning
  6. Reinforcement learning
  7. Clustering algorithm
  8. Supervised
  9. Online learning systems can learn incrementally rather than all at once as in Batch learning. The benefit of this is that it can adapt quickly to changing data as well as large quantities of data.
  10. Out-of-core algorithms can handle very large quantities of data that cannot fit in a computer's main memory. To solve this, the algorithm splits the data into mini-batches and uses online learning on each one.
  11. Instance-based learning
  12. A model parameter determines the the prediction based on a new instance. A learning algorithm optimises these values so that the model generalises well to new instances. A hyperparameter is a parameter of the learning algorithm itself, not of the model.
  13. Model-based learning algorithms search for an optimal value for the model parameters such that the model generalises well to new instances. This is usually achieved by minimising a cost function that measures how bad the system is at making predictions on the training data. To make predictions, the new instance's features are passed into the model's prediction function along with the parameter values found by the learning algorithm
  14. Lack of data, poor data quality, models that are too simple or too complex.
  15. If the model performs well with training data but poorly on new instances it is likely overfitting the training data. Three potential solutions to models that are overfitting is: getting more data, simplifying the model, or reducing the noise in the training data.
  16. A test set is used to estimate the generalisation error that a model will mkake on new instances before the model is launched in production
  17. A validation set is used to compare models.
