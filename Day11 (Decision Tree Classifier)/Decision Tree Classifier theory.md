#Decision Tree Classifier

**What is a Decision Tress?**
  A Decision Tree is a supervised machine learning algorithm used for classification and regression tasks. It splits the data into subsets based on feature values to create a tree-like model of decisions.

  **How it works:**
  1. Root Node: The dataset starts at the root node.
  2. Splitting: At each node, the algorithm selects a feature and a threshold to split the data in a way that best separates the classes.
  3. Leaf Node: A terminal node that makes a final prediction (class label or value).

**Split Criteria (Mathematical Intuition)**
The algorithm tries to maximize the "purity" of nodes using:
- Gini Impurity (default in sklearn)
  <img width="346" height="103" alt="image" src="https://github.com/user-attachments/assets/ac0786fb-f0fd-4170-ae74-dacd23621efd" />
where pi is the probability of class i at that node.

- Entropy (Information Gain):
  <img width="800" height="194" alt="image" src="https://github.com/user-attachments/assets/8e2079fc-44ec-4f7d-934f-e21cacf65339" />

**Recursive Splitting**
- The tree recursively splits the data until:
- All the records are pure (belong to one class), or
- A stopping condition (like max depth or min samples) is reached.

** Parameters in sklearn's DecisionTreeClassifier**
- criterion='gini' or 'entropy' - the function to measure quality of split
- max_depth - limits the depth of tree to prevent overfitting
- min_samples_split - minimum samples required to split a node
- min_samples_leaf - minimum samples required at a lead node

**Pros:**
- Easy to understand and visualize
- No need for feature scaling
- Works with both numerical and categorical data

**Cons**
- Prone to overfitting (especilly deep tree)
- Unstable to small variations in data
- Greedy splits may not always be optimal

**Example Use Case**
Classifying whether a tumor is benign or malignant based on features like radius, texture, etc.,
