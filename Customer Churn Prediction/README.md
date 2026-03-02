#  Customer Churn Prediction 

## 📌 Project Overview
This project implements an **end-to-end machine learning pipeline** to analyze customer behavior and predict churn using the Telco Customer Churn dataset.

The workflow includes **Exploratory Data Analysis (EDA), data cleaning, feature engineering, handling class imbalance, model building, evaluation and model serialization**.

---

## Dataset Information
- **Dataset**: Telco Customer Churn
- **Total Records**: 7,043
- **Total Features**: 21
- **Target Variable**: `Churn` (Yes / No)

The dataset contains customer demographic details, service subscriptions, billing information and contract details.

---

## Technologies & Libraries Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Imbalanced-learn (SMOTEENN)

---

## Exploratory Data Analysis (EDA)
Key EDA steps:
- Verified data types and structure
- Converted `TotalCharges` from object to numeric
- Removed records with missing values (<0.2%)
- Created tenure-based customer groups
- Analyzed churn distribution (imbalanced: 73% No, 27% Yes)
- Visualized churn patterns across contracts, services, tenure, and charges

### Key Insights
- High churn observed for:
  - Month-to-month contracts
  - Customers with high monthly charges
  - Fiber optic internet users
  - Customers without online security or tech support
- Low churn observed for:
  - Long-term contracts
  - Customers with tenure above 5 years
  - Customers without internet service
- Gender and phone service showed minimal impact on churn

---

##  Data Preprocessing & Feature Engineering
- Converted target variable: `Yes → 1`, `No → 0`
- One-hot encoded categorical variables
- Dropped irrelevant columns (`customerID`, `tenure`)
- Saved the processed dataset as `tel_churn.csv`

---

## Model Building
### Models Implemented
- Decision Tree Classifier
- Random Forest Classifier

### Handling Class Imbalance
- Applied **SMOTEENN** (SMOTE + Edited Nearest Neighbors) to balance the dataset
- Improved recall and F1-score for churned customers

---

##  Model Performance

###  Before SMOTEENN
| Model | Accuracy | Recall (Churn) |
|------|----------|----------------|
| Decision Tree | ~78% | ~49% |
| Random Forest | ~80% | ~45% |

### After SMOTEENN (Final Model)
**Random Forest + SMOTEENN**
- **Accuracy**: 94%
- **Precision (Churn)**: 94%
- **Recall (Churn)**: 96%
- **F1-Score (Churn)**: 95%

