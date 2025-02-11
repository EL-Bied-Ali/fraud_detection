# Credit Card Fraud Detection

**Project Overview**  
This repository demonstrates a complete end-to-end solution for detecting fraudulent credit card transactions. We work with a highly imbalanced dataset (0.17% fraud) and implement techniques such as SMOTE for data resampling, Logistic Regression as a baseline, and XGBoost for a more advanced approach. 

**Key Steps & Highlights**  
1. **Data Exploration**:  
   - Analyzed transaction distribution and identified outliers using boxplots.  
   - Investigated feature correlations and found most features weakly correlated, implying the need for multiple features in detection.

2. **Handling Imbalance**:  
   - Oversampled the minority class (fraud) using SMOTE, significantly improving the model’s ability to detect fraud.

3. **Models & Performance**:  
   - **Logistic Regression**: 99.28% accuracy, 93% recall for fraud.  
   - **XGBoost**: ~99.96% accuracy, near-100% precision and recall for fraud.  
   - Hyperparameter tuning with GridSearchCV further validated the best parameters for XGBoost.

4. **Feature Importance & Selection**:  
   - Used XGBoost’s feature_importances_ to remove low-importance features, improving efficiency.

**How to Use**  
1. Clone the repository:
   ```bash
   git clone https://github.com/EL-Bied-Ali/fraud_detection.git
