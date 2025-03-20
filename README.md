Credit Risk Classification Analysis
Overview
This project provides an assessment of credit risk classification data. The analysis compares the performance of two different machine learning models: Receiver Operating Characteristic (ROC) and Decision Tree (DT). The goal was to evaluate how well these models classify data into two distinct groups (0 and 1).

Approach
Dataset Examination:

The loan_status column exhibited the most noticeable difference between group 0 and group 1.

Initial analysis revealed a significant imbalance: over 96% of the data belonged to group 0, while only a small fraction belonged to group 1. This imbalance posed challenges for accurate predictions of group 1.

Data Preprocessing:

Data cleaning and normalization were performed using a standard scaler to address the disparity between the lowest and highest values.

Model Implementation:

Logistic Regression with ROC Curve:

A ROC curve evaluates the model’s ability to distinguish between groups. The test/train split was implemented to assess this metric.

Decision Tree Classifier:

A DT was utilized to compare results with the ROC model.

Results
Decision Tree Model Performance:

Precision (0.89): 89% of the predicted "1s" were correct.

Recall (0.83): Successfully captured 83% of actual "1s."

F1-Score (0.85): Balanced precision and recall for improved accuracy.

Key Insights:
While the DT model performed adequately, predicting group 1 proved more critical since group 0 was treated as a test environment.

The results highlight the importance of addressing class imbalance and focusing on accuracy for group 1 predictions.

Conclusion
The analysis demonstrates that while the Decision Tree model performs well, further improvements are necessary, particularly in capturing group 1 accurately. Refining preprocessing steps or exploring alternative algorithms could further enhance model performance.
