# Best Model Summary

**Date:** 2025-08-24 14:32:42

Among all the models trained, **Random Forest** performed the best.

- **Test Accuracy:** 1.0000  
- **Test Precision:** 1.0000  
- **Test Recall:** 1.0000  
- **Test F1-score:** 1.0000  
- **Test AUC-ROC:** 1.0000  
- **Best cross-validated score (ROC-AUC):** 0.8022  
- **Best hyperparameters:** `{'clf__max_depth': None, 'clf__min_samples_leaf': 4, 'clf__min_samples_split': 2, 'clf__n_estimators': 200}`

**Why this model is best:**  
Random Forest achieved the strongest overall performance on the test set and showed solid cross-validated AUC, indicating good generalization. As an ensemble of decision trees, it reduces overfitting risk and captures non-linear feature interactions better than Logistic Regression, a single Decision Tree, or KNN.

**Note:** Perfect or near-perfect test scores can occur with small test sets. Results should be interpreted with care and validated on additional data or via repeated cross-validation.


**Precision across models (baseline):**

| Model               |   Precision |
|:--------------------|------------:|
| Random Forest       |    1        |
| Decision Tree       |    0.25     |
| KNN                 |    0.166667 |
| Logistic Regression |    0.125    |

