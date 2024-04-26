# Final Project: Customer Churn Prediction for Comcast

### Overview
This project aims to predict customer churn within the telecom sector, using data from a telecommunications company. Customer churn, which occurs when customers discontinue their service, represents a significant challenge due to factors like poor service quality, better deals from competitors, and inadequate customer service.

### Data
The dataset used in this project comes from a fictional telecommunications company, tracking details like demographics, services used, and account details of 7043 customers. This data, sourced from an IBM community website, includes variables such as gender, age, services subscribed, and billing information.

### Methodology
#### Data Preprocessing
- Categorical data (InternetService, Contract, PaymentMethod) was encoded using one-hot encoding.
- Numerical features (tenure, MonthlyCharges, TotalCharges) were standardized.

#### Feature Engineering
- A new DataFrame `impactful_features` was created, combining both encoded categorical and standardized numerical features.
- Customer segmentation was performed using K-means clustering.

#### Model Development
Several machine learning models were applied:
- **Random Forest Classifier:** Achieved an accuracy of 0.78.
- **Support Vector Machine (SVM):** Also reached an accuracy of 0.78.
- **K-Nearest Neighbors (KNN):** Had an accuracy of 0.77.
- **LSTM Model:** Utilized for its ability to capture temporal dependencies, achieving the highest accuracy of 0.80.

### Results
The LSTM model demonstrated the best performance with a ROC-AUC score of 0.90, suggesting excellent predictive capability for customer churn. This model was found to be most suitable due to its high accuracy and effective handling of sequential data.

### Conclusion
The project illustrates the effectiveness of advanced machine learning techniques, particularly LSTM, in predicting customer churn in the telecom industry. By targeting specific customer segments and service features associated with higher churn rates, telecom companies can develop more effective retention strategies.
