# Module_17_Challenge

### In this project, I am using imbalanced-learn and schikit-learn libraries to build and evaluate models using resampling. I am specific assessing credit risk, using data from LendingClub. For each sampling technique, I am looking for 3 data points: Accuracy Score, Precision, and Sensitivity. Balanced Accuracy is defined as the average of recall obtained on each class. It is measured on a scale of 0 (the worst) and 1 (the best). Precision answers the question, "What proportion of positive identifications was actually correct?" A model that produces no false positives has a score of 1. Sensitivity (or Recall) answers the question, "What proportion of actual positives was identified correctly?" A model that produces no false negaticves as a sensitivity of 1. The best technique will have all 3 values as close to 1 as possible. 


### The resampling techniques and their descriptions are as follows: 

-- Oversampling data using random oversampler

Accuracy Score: .67
Precision for Low Risk: 1.00
Precision for High Risk: 0.01
Sensitivitiy for Low Risk: 0.61
Sensitivity for High Risk: 0.72

-- Oversampling data using SMOTE 

Accuracy Score: .66
Precision for Low Risk: 1.00
Precision for High Risk: 0.01
Sensitivitiy for Low Risk: 0.70
Sensitivity for High Risk: 0.62

-- Undersampling data using Cluster Centroids

Accuracy Score: .54
Precision for Low Risk: 1.00
Precision for High Risk: 0.01
Sensitivitiy for Low Risk: 0.42
Sensitivity for High Risk: 0.67

-- Undersampling data using Cluster Centroids
Accuracy Score: .54
Precision for Low Risk: 1.00
Precision for High Risk: 0.01
Sensitivitiy for Low Risk: 0.42
Sensitivity for High Risk: 0.67

-- Combination sampling with SMOTEENN

Accuracy Score: .65
Precision for Low Risk: 1.00
Precision for High Risk: 0.01
Sensitivitiy for Low Risk: 0.57
Sensitivity for High Risk: 0.72

## Analysis
Since it is very difficult to have both precision and sensitivity score 1, different scenarios will prefer one of the other measurement to score higher. In the case of credit risk, it is more important for the sensitivity to High Risk be high. This means that there is a large percentage of actual positives identified. Someone who assesses credit risk wants to make sure that all high risk loans are caught. It is not nearly as important for low risk loans to be identified correctly, as they inherently pose less of a threat. 
That being said, the random oversampler was the best technique to use. The accuracy score was the highest, and the Sensitive for High Risk Loans was the highest. 

