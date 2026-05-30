# 🐦 Twitter Sentiment Analysis

A Machine Learning project that classifies tweets as **Positive** or **Negative** using TF-IDF vectorization and Logistic Regression, trained on 1.6 million tweets from the Sentiment140 dataset.

---

## 📁 Project Structure
Twitter_Sentiment_Analysis/
├── main.ipynb        
├── README.md         
├── requirements.txt  
└── .gitignore        

---

## 📊 Dataset

| Property   | Details                              |
|------------|--------------------------------------|
| Name       | Sentiment140                         |
| Source     | [Kaggle](https://www.kaggle.com/datasets/kazanova/sentiment140) |
| Size       | 1.6 million tweets                   |
| Labels     | 0 = Negative, 1 = Positive           |
| Balance    | 800k Positive + 800k Negative        |

> ⚠️ Dataset is not included in this repo due to size.
> Download it directly from Kaggle using the notebook setup cell.

---

## 🚀 How to Run

**1. Open the notebook in Google Colab**
- Go to [colab.research.google.com](https://colab.research.google.com)
- Upload `main.ipynb` or open it directly from GitHub

**2. Set up your Kaggle token**
- Go to kaggle.com → Settings → API → Create New Token
- Add it to Colab Secrets (🔑 icon) with the name `KAGGLE_TOKEN`

**3. Run all cells in order**
- Runtime → Run All
- Training takes ~3–5 minutes on full data

---

## 🤖 Model

| Step  | Method                          |
|-------|---------------------------------|
| Clean | Regex + Stemming + Stopwords    |
| Transform | TF-IDF Vectorizer (50k features, bigrams) |
| Model | Logistic Regression (saga solver) |
| Split | 80% Train / 20% Test            |

**Simple explanation:**
- TF-IDF converts each tweet into numbers based on word importance
- Logistic Regression learns the pattern between those numbers and sentiment
- No deep learning needed — simple models work great on clean text data

---

## 📈 Results

| Metric    | Score  |
|-----------|--------|
| Accuracy  | 81.98% |
| F1-Score  | 0.82   |
| Precision | 0.82   |
| Recall    | 0.82   |

---



## 👤 Author

**Abdelrahman Mohamed Salah**  
AI Engineer | Machine Learning & NLP Developer

