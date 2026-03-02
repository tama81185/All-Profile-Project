# Amazon Alexa Reviews — Sentiment Analysis

## Project Overview
This project implements an end-to-end machine learning pipeline to analyze Amazon Alexa product reviews and predict customer feedback (positive or negative) based on review text.

The workflow includes Exploratory Data Analysis (EDA), data cleaning, text preprocessing, feature extraction using Bag-of-Words, model training, evaluation, hyperparameter tuning and model serialization.

---

## Dataset Information
- **Dataset:** Amazon Alexa Reviews (`amazon_alexa.tsv`)
- **Total Records:** 3,150 (3,149 after removing null values)
- **Total Features:** 5 original features + 1 engineered feature
- **Target Variable:** Feedback (0 = Negative, 1 = Positive)

### Features
- `rating` — Product rating (1–5)
- `date` — Review date
- `variation` — Product variation/type
- `verified_reviews` — Review text
- `feedback` — Sentiment label
- `length` — Length of review text (engineered feature)

---

## Technologies & Libraries Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- NLTK
- Scikit-learn
- XGBoost
- WordCloud
- Pickle

---

## Exploratory Data Analysis (EDA)

### Key EDA Steps
- Checked dataset structure, feature names and data types
- Removed one record with missing review text
- Created a new feature: review length
- Analyzed distributions of ratings, feedback and product variations
- Visualized:
  - Rating distribution
  - Feedback distribution
  - Variation distribution
  - Review length distribution
- Generated word clouds for:
  - All reviews
  - Negative reviews
  - Positive reviews

---

## Key Insights
- Most reviews are highly positive (over 90% positive feedback)
- Ratings of 1–2 correspond to negative feedback
- Ratings of 3–5 correspond to positive feedback
- Certain product variations received more reviews than others
- Positive reviews commonly contain words like:
  - good, amazing, best, great
- Negative reviews commonly contain words like:
  - garbage, poor, horrible, repair

---

## Data Preprocessing & Feature Engineering

### Text Processing Steps
- Removed non-alphabet characters
- Converted text to lowercase
- Removed English stopwords
- Applied stemming using Porter Stemmer
- Built a corpus of cleaned reviews

### Feature Extraction
- Used **CountVectorizer** (Bag-of-Words)
- Limited vocabulary to top 2,500 words
- Scaled features using **MinMaxScaler**

---

## Model Building

### Models Implemented
- Random Forest Classifier
- XGBoost Classifier
- Decision Tree Classifier

### Train-Test Split
- 70% Training
- 30% Testing

---

## Model Performance

### Random Forest
- Training Accuracy: **99.41%**
- Testing Accuracy: **94.18%**

### XGBoost
- Training Accuracy: **97.19%**
- Testing Accuracy: **93.76%**

### Decision Tree
- Training Accuracy: **99.41%**
- Testing Accuracy: **91.96%**

---

## Cross-Validation & Hyperparameter Tuning

### Random Forest Cross-Validation
- Mean Accuracy: **93.28%**
- Standard Deviation: **0.006**

### Best Parameters (Grid Search)
- bootstrap: True
- max_depth: 80
- min_samples_split: 8
- n_estimators: 100

---

## Model Saving
Saved components using Pickle:

- Count Vectorizer → `countVectorizer.pkl`
- Scaler → `scaler.pkl`
- XGBoost Model → `model_xgb.pkl`

Models are ready for reuse and deployment.

---

## Conclusion
Successfully built a machine learning system to classify Amazon Alexa reviews as positive or negative using text data.

The project demonstrates:

- Effective text preprocessing
- Feature extraction using Bag-of-Words
- Comparison of multiple classification algorithms
- Hyperparameter tuning for improved performance
- Deployment-ready saved models
