#Random Forests#

**Definition:**
- An ensemble of Decision Trees.
- Trains multiple trees on random subsets of data and features and takes majority vote (classification) or average (regression).

- **Why better than a single tree?**
- - Reduces overfitting by averaging multiple models -> higher generalisation.

  **Key parameters:**
  - n_estimators: number of trees.
  - max_depth: limits tree depth to avoid overfitting.
  - max_features: number of features to consider when looking for best split.
