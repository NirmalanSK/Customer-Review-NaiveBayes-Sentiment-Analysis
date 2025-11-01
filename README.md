#  Customer Review Sentiment Analysis using Naive Bayes

##  Overview
This project performs **Sentiment Analysis** on customer reviews using the **Naive Bayes** algorithm.  
The goal is to classify text reviews into **Positive** or **Negative** sentiments based on the words used.  

The model uses **text preprocessing**, **TF-IDF vectorization**, and **Multinomial Naive Bayes** to understand how words contribute to the sentiment of a review.

---

##   Libraries Used
- **Python**
- **pandas** – data loading and manipulation  
- **numpy** – numerical operations  
- **scikit-learn (sklearn)** – machine learning model, vectorization, metrics  
- **nltk** – natural language preprocessing  
- **tqdm** – progress tracking  
- **matplotlib** & **seaborn** – data visualization  
- **BeautifulSoup** & **re** – text cleaning (regex and HTML removal)

---

##  Project Workflow

### 1. Data Loading
- Load and inspect the dataset containing customer text reviews and sentiment labels.  

### 2. Data Preprocessing
- Removed URLs, HTML tags, numbers, and non-alphabetic characters  
- Converted all text to lowercase  
- Tokenized and removed stopwords  
- Lemmatized/stemmed words to their base form  

### 3. Feature Extraction
- Used **TF-IDF Vectorization** to convert text into numerical features that represent word importance.

### 4. Model Building
- Trained a **Multinomial Naive Bayes** classifier using `sklearn.naive_bayes.MultinomialNB`.  
- Optimized the smoothing parameter **alpha** using **GridSearchCV**.

### 5. Model Evaluation
- Evaluated performance using:
  - **Accuracy**
  - **Precision, Recall, F1-score**
  - **ROC Curve and AUC Score**
- Visualized top features contributing to **Positive** and **Negative** classes.

### 6. Results
- Displayed most informative features for each sentiment.  
- Plotted **Confusion Matrix**, **ROC Curve**, and **Word Importance** charts.  
- Model achieved high accuracy on unseen test data, demonstrating strong generalization.

---

##  How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/NirmalanSK/Customer-Review-NaiveBayes-SentimentAnalysis.git
