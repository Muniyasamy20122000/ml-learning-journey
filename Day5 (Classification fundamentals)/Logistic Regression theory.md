**Logistic Regression - Intuition**

Logistic Regression is used for classification tasks.

**How it works:**
Users a sigmoid function to convert linear combination of inputs into probabilities between 0 and 1.

**Mathematical Formula:**
 p= 1/
1+e 
−(mx+c)
 
​
- mx + c : linear combination of inputs
- e: Euler's number (~2.718)
- p: probability of class 1

If p > 0.5 -> class 1, else class 0

**Why sigmoid?**
Maps any real number to a bounded range (0,1) for probability interpretation.
