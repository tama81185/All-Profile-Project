# Sentiment Analysis

##  Project Overview
This project performs **sentiment analysis**  using machine learning techniques.  
The goal is to predict whether a review is **positive (feedback = 1) or negative (feedback = 0)** based on the textual content of the verified reviews.

The workflow includes **Exploratory Data Analysis (EDA), text preprocessing, feature extraction, model building (Random Forest, XGBoost, Decision Tree), evaluatio
---

## 📊 Dataset Information
- **Dataset**: Amazon Alexa Reviews
- **Total Records**: 3,149 (after removing nulls)
- **Total Features**: 5
  - `rating` – rating given by user (1–5)
  - `date` – review date
  - `variation` – product variation
  - `verified_reviews` – textual review
  - `feedback` – target variable (0 = negative, 1 = positive)
- **Target Variable**: `feedback`  

**Class Distribution**:  
- Positive reviews: 91.87%  
- Negative reviews: 8.13%

---

## 🛠️ Technologies & Libraries Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn, WordCloud  
- NLTK (stopwords, PorterStemmer)  
- Scikit-learn (RandomForestClassifier, DecisionTreeClassifier, MinMaxScaler, CountVectorizer, cross_val_score, GridSearchCV)  
- XGBoost (XGBClassifier)  
- Pickle (model serialization)

---

## 🔍 Exploratory Data Analysis (EDA)
Key steps performed:
- Checked for null values and dropped 1 record with missing `verified_reviews`
- Created `length` column to store the length of each review
- Analyzed `rating` column:
  - Most reviews are 5-star (72.59%)
  - Ratings 1–2 correlate with negative feedback; 3–5 with positive feedback
- Analyzed `variation` column to understand product types
- Created bar plots, pie charts, and histograms for ratings, feedback, review lengths, and variations
- Generated **WordClouds** for all reviews, positive reviews, and negative reviews
  - Negative words: garbage, pointless, poor, horrible, repair
  - Positive words: good, enjoying, amazing, best, great

---

## 📝 Text Preprocessing
Steps applied to `verified_reviews`:
1. Remove non-alphabet characters
2. Convert to lowercase
3. Tokenize and remove stopwords
4. Apply **Porter Stemming**
5. Combine processed words into cleaned corpus

Used **CountVectorizer** to create Bag-of-Words features (max 2500 features)  
Saved CountVectorizer for deployment as `Models/countVectorizer.pkl`.

---

## ⚙️ Data Preparation
- Target variable: `feedback`
- Split dataset into train (70%) and test (30%) sets
- Applied **MinMaxScaler** to scale features between 0 and 1
- Saved scaler for deployment as `Models/scaler.pkl`

---

## 🤖 Model Building

### Random Forest Classifier
- Trained on scaled training data
- Achieved high accuracy on train and test sets
- Performed **K-Fold Cross Validation** (cv = 10)
- Applied **GridSearchCV** for hyperparameter tuning
- Confusion Matrix visualized

### XGBoost Classifier
- Trained on scaled training data
- High accuracy on train and test sets
- Confusion matrix visualized
- Saved model as `Models/model_xgb.pkl`

### Decision Tree Classifier
- Trained on scaled training data
- Moderate performance compared to Random Forest and XGBoost
- Confusion matrix visualized

---

## 📈 Model Performance

| Model             | Training Accuracy | Testing Accuracy |
|------------------|-----------------|----------------|
| Random Forest     | High (~>90%)    | High (~>90%)   |
| XGBoost           | High (~>90%)    | High (~>90%)   |
| Decision Tree     | Moderate        | Moderate       |

**Observations:**
- Random Forest and XGBoost outperform Decision Tree
- Text preprocessing and feature extraction critical for model performance
- Positive feedback dominates dataset; class imbalance should be considered for deployment

---

## 💾 Model Saving
- **CountVectorizer** → `Models/countVectorizer.pkl`
- **Scaler** → `Models/scaler.pkl`
- **XGBoost model** → `Models/model_xgb.pkl`

---

## ✅ Conclusion
- Successfully implemented **sentiment analysis** for Amazon Alexa reviews
- Performed **EDA**, **text preprocessing**, **feature extraction**, and **model building**
- **XGBoost** selected as final model for deployment due to high accuracy
- Visualized key insights via bar plots, pie charts, histograms, and word clouds

---

## 🚀 Future Enhancements
- Apply **SMOTE or class balancing** to improve negative review detection
- Implement **TF-IDF** or **word embeddings** for better feature representation
- Deploy model using **Flask / FastAPI** for real-time prediction
- Build **interactive dashboards** for insights visualization, and model serialization**.

---


---

## 📊 Dataset Information
- **Dataset**: Amazon Alexa Reviews
- **Total Records**: 3,149 (after removing nulls)
- **Total Features**: 5
  - `rating` – rating given by user (1–5)
  - `date` – review date
  - `variation` – product variation
  - `verified_reviews` – textual review
  - `feedback` – target variable (0 = negative, 1 = positive)
- **Target Variable**: `feedback`  

**Class Distribution**:  
- Positive reviews: 91.87%  
- Negative reviews: 8.13%

---

## 🛠️ Technologies & Libraries Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn, WordCloud  
- NLTK (stopwords, PorterStemmer)  
- Scikit-learn (RandomForestClassifier, DecisionTreeClassifier, MinMaxScaler, CountVectorizer, cross_val_score, GridSearchCV)  
- XGBoost (XGBClassifier)  
- Pickle (model serialization)

---

## 🔍 Exploratory Data Analysis (EDA)
Key steps performed:
- Checked for null values and dropped 1 record with missing `verified_reviews`
- Created `length` column to store the length of each review
- Analyzed `rating` column:
  - Most reviews are 5-star (72.59%)
  - Ratings 1–2 correlate with negative feedback; 3–5 with positive feedback
- Analyzed `variation` column to understand product types
- Created bar plots, pie charts, and histograms for ratings, feedback, review lengths, and variations
- Generated **WordClouds** for all reviews, positive reviews, and negative reviews
  - Negative words: garbage, pointless, poor, horrible, repair
  - Positive words: good, enjoying, amazing, best, great

---

## 📝 Text Preprocessing
Steps applied to `verified_reviews`:
1. Remove non-alphabet characters
2. Convert to lowercase
3. Tokenize and remove stopwords
4. Apply **Porter Stemming**
5. Combine processed words into cleaned corpus

Used **CountVectorizer** to create Bag-of-Words features (max 2500 features)  
Saved CountVectorizer for deployment as `Models/countVectorizer.pkl`.

---

## ⚙️ Data Preparation
- Target variable: `feedback`
- Split dataset into train (70%) and test (30%) sets
- Applied **MinMaxScaler** to scale features between 0 and 1
- Saved scaler for deployment as `Models/scaler.pkl`

---

## 🤖 Model Building

### Random Forest Classifier
- Trained on scaled training data
- Achieved high accuracy on train and test sets
- Performed **K-Fold Cross Validation** (cv = 10)
- Applied **GridSearchCV** for hyperparameter tuning
- Confusion Matrix visualized

### XGBoost Classifier
- Trained on scaled training data
- High accuracy on train and test sets
- Confusion matrix visualized
- Saved model as `Models/model_xgb.pkl`

### Decision Tree Classifier
- Trained on scaled training data
- Moderate performance compared to Random Forest and XGBoost
- Confusion matrix visualized

---

## 📈 Model Performance

| Model             | Training Accuracy | Testing Accuracy |
|------------------|-----------------|----------------|
| Random Forest     | High (~>90%)    | High (~>90%)   |
| XGBoost           | High (~>90%)    | High (~>90%)   |
| Decision Tree     | Moderate        | Moderate       |

**Observations:**
- Random Forest and XGBoost outperform Decision Tree
- Text preprocessing and feature extraction critical for model performance
- Positive feedback dominates dataset; class imbalance should be considered for deployment

---

## 💾 Model Saving
- **CountVectorizer** → `Models/countVectorizer.pkl`
- **Scaler** → `Models/scaler.pkl`
- **XGBoost model** → `Models/model_xgb.pkl`

---

## ✅ Conclusion
- Successfully implemented **sentiment analysis** for Amazon Alexa reviews
- Performed **EDA**, **text preprocessing**, **feature extraction**, and **model building**
- **XGBoost** selected as final model for deployment due to high accuracy
- Visualized key insights via bar plots, pie charts, histograms, and word clouds

---

## 🚀 Future Enhancements
- Apply **SMOTE or class balancing** to improve negative review detection
- Implement **TF-IDF** or **word embeddings** for better feature representation
- Deploy model using **Flask / FastAPI** for real-time prediction
- Build **interactive dashboards** for insights visualization
