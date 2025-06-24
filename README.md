
# Sentiment Analysis of Movie Reviews 🎬

This project implements a sentiment analysis system that classifies movie reviews as **positive** or **negative** using multiple machine learning models. The dataset used is the [Polarity Dataset v2.0](http://www.cs.cornell.edu/people/pabo/movie-review-data) by Bo Pang and Lillian Lee.

---

## 📁 Dataset

The dataset is included in the file `review_polarity.tar.gz`.  
After extracting, the structure is:

```
review_polarity/
└── txt_sentoken/
    ├── pos/  # Positive reviews
    └── neg/  # Negative reviews
```

---

## 🧹 Preprocessing Steps

- Convert text to lowercase  
- Remove punctuation  
- Tokenize text  
- Remove stopwords and non-alphabetic tokens  
- Apply stemming and lemmatization  

---

## 🧠 Feature Extraction

Text is vectorized using **TF-IDF** with:

- N-gram range: (1, 2) → unigrams and bigrams  
- Min document frequency: 5  
- Max document frequency: 0.7  

---

## 🤖 Models Used

| Model                | Accuracy |
|---------------------|----------|
| XGBoost              | 83.8%    |
| SVM                  | 82.8%    |
| Logistic Regression  | 82.3%    |
| Neural Network (MLP) | 82.0%    |
| Gradient Boosting    | 82.0%    |
| Random Forest        | 79.8%    |
| Naive Bayes          | 71.5%    |
| KNN                  | 66.5%    |
| Decision Tree        | 64.5%    |

---

## 🛠️ Tools & Libraries

- Python
- scikit-learn
- NLTK
- XGBoost

---

## 🚀 How to Run

Install the required packages:

```bash
pip install nltk scikit-learn xgboost
```

Then run the notebook or Python file:

```bash
python sentiment_analysis.py
```
