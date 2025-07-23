# K-Nearest Neighbors (KNN)

**1. What is KNN?**
- A supervised learning algorithm used for classification and regression.
- Instance-based / lazy learning algorithm -> it stores training data and predicts labels based on proximity at runtime.

**2. How does it work?"**
- To classify a new data point:
  - Calculate disctance to all training data points (commonly Euclidean distance)
  - Select k nearest neighbors.
  - Assign class based on majority vote among k neighbors (classification) or average (regression).

**3. Mathematics - Eucllidean Distance**
For two points p = (p1,p2,...,pn) and (q1,q2, ..., qn):

d(p,q) = √(p1-q1)^2+ (p2-q2)^2 + ... + (pn - qn)^2

**4. Hyperparameter 'k'**
- k =  number of neighbors considered
- Low k -> sensitive to noise (overfitting).
- High k -> smoother decision boundary (uderfitting if too high)

**5. Pros**
- Simple, intuitive, no training phase.
- Works well with small to medium sized data.

**6. Cons:**
- Slow prediction time for large dataset (calculates distance to all points).
- Affected by irrelevant features / unscaled data -> Requires normalization.

**7. When to use?**
- Suitable for classification tasks with clearly clustered data.
- Example: Handwritten digit recognition, recommendation systems.
