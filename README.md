# SMS Spam Classification – Text Vectorization Project

This project demonstrates **text preprocessing and vectorization techniques** for building a **Spam Classification model** using the SMS Spam Collection dataset.  
It covers **Bag of Words (BoW)** and **TF-IDF** vectorization, model training with **Naive Bayes** and **Logistic Regression**, and evaluation with accuracy, precision, recall, and confusion matrix.

---

## Dataset
We use the [SMS Spam Collection Dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection) with:
- **label**: 'ham' (not spam) or 'spam'
- **message**: the SMS text

---

## Workflow
1. **Data Loading** → Load dataset into Pandas DataFrame  
2. **Exploration** → Null values, unique labels, statistics  
3. **Text Preprocessing**  
   - Lowercasing text  
   - Removing punctuation  
   - Removing stopwords  
   - Tokenization using NLTK  
4. **Feature Extraction**  
   - Bag of Words (BoW) with `CountVectorizer`  
   - TF-IDF with `TfidfVectorizer`  
5. **Comparison** between frequency (BoW) and importance (TF-IDF) for selected words  
6. **Train/Test Split**  
7. **Model Training**  
   - Naive Bayes  
   - Logistic Regression  
8. **Evaluation Metrics**  
   - Accuracy  
   - Precision  
   - Recall  
9. **Confusion Matrix** visualization  
10. **Top 10 TF-IDF Spam Words** visualization

---

## 📈 Results
| Metric     | Naive Bayes | Logistic Regression |
|------------|-------------|---------------------|
| Accuracy   | ~97%        | ~96–97%             |
| Precision  | ~95–96%     | ~95%                |
| Recall     | ~93%        | ~92–93%             |

The model achieves **high precision** and **recall**, making it effective at catching spam without marking many genuine messages as spam.

---

## 📊 Example Visualizations
- **Confusion Matrix** showing TP, TN, FP, FN  
- **Bar Chart** of top 10 spam-indicative words (highest TF-IDF scores)

---

## 🛠 Installation
```bash
https://github.com/<your-username>/spam-classification.git
cd spam-classification
pip install -r requirements.txt
