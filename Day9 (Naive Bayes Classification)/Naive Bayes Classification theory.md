# Naive Bayes Classification

**What is Naive Bayes?**
- A probabilisitc supervised learning algorithm based on Bayes Theorem.
- Called naive because it assumes features are independent given the class.

**2. Bayes Theorem**
<img width="379" height="117" alt="image" src="https://github.com/user-attachments/assets/6ca0bde5-198d-4c2e-b7b1-879697771d61" />

Where:
- P(A|B): Probability of A given B (posterior).
- P(B|A): Probability of B given A (likelihood).
- P(A): Probability of A (prior).
- P(B): Probability of B (evidence).

**3. How Naive Bayes works?**
- For each class, calculate:
   <img width="647" height="83" alt="image" src="https://github.com/user-attachments/assets/c3a0ca3e-0ec8-4b14-8ce5-a914ad36044f" />
- Pick class with highest posterior probability.

**4. Types of Naive Bayes:**
| Type            | Used for                                   | Distribution assumption |
| --------------- | ------------------------------------------ | ----------------------- |
| **Gaussian**    | Continuous data                            | Normal distribution     |
| **Multinomial** | Discrete counts (e.g. word counts in text) | Multinomial             |
| **Bernoulli**   | Binary features                            | Bernoulli               |

**5. Pros:**
- Very fast and efficient even with large data.
- Works well for text clasification (spam detection, sentiment analysis).

**6. Cons:**
- The "naive" independence assumption rarely holds in real data.
- Performs poorly if features are highly correlated.

