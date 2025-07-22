#Evaluation Metrics in Classification#

**1. Confusion Matrix**
- TP (True Positive): Correctly predicted positives
- TN (True Negative): Correctly predicted negatives
- FP (False Positive): Incorrectly predicted positive (Type I error)
- FN (False Negative): Incorrectly predicted negative (Type II error)

**2. Accuracy**
- (TP + TN)/Total
- Good when classes are balanced

**3. Precision**
- TP/(TP + FP)
- How many predicted positives are actually positive?

**4. Recall (Sensitivity)**
- TP/(TP + FN)
- How many actual positive were caught?

**5. F1-Score**
- 2 * (Precision * Recall) / (Precision + Recall)
- Harmonic mean -> Balances Precision and Recall

**6. ROC Curve (Receiver Operating Characteristic)**
- Plots True Positive Rate (Recall) vs False Positive Rate
- Shows model's performance across thresholds

**7. AUC (Area Under Curve)**
- 0.5 = random, 1 = perfect.
- Higher AUC -> better model performance.

**8. Precision-Recall Curve**
- Plots Precision vs Recall for different thresholds.
- Useful when positive class is rare (e.g. fraud, cancer).

**Key Takeaway**
- Medical: High recall (catch al patients)
- Spam detection: High precision (don't block valid mails)
