# 🧠 Social Media Sentiment Analysis

This project is a simple yet powerful machine learning pipeline that performs sentiment analysis on tweets. It classifies text into **Positive**, **Negative**, or **Neutral** sentiment using logistic regression and TF-IDF vectorization.

---

## 📌 Project Features

- Preprocesses raw tweet text (removes links, mentions, stopwords, punctuation).
- Converts tweets into numeric features using TF-IDF.
- Trains a Logistic Regression model on 30,000+ tweets.
- Evaluates model performance with accuracy and classification report.
- Predicts sentiment of new, custom text inputs.
- Visualizes sentiment distribution in the dataset.

---

## 📂 Dataset Used

The project uses the [Sentiment140 Dataset](https://www.kaggle.com/datasets/kazanova/sentiment140), which contains over 1.6 million labeled tweets.

- **Label 0** → Negative  
- **Label 2** → Neutral  
- **Label 4** → Positive  

Only the `label` and `tweet` columns are used.

---

## 🛠 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/social-media-sentiment-analysis.git
cd social-media-sentiment-analysis
```

### 2. Install Dependencies
It’s recommended to use a virtual environment.

```bash
pip install -r requirements.txt
```

### 3. Download the Dataset
Get the dataset from [Kaggle](https://www.kagglecom) and extract it. Place the file:
```bash
training.1600000.processed.noemoticon.csv
```

### 4. Run the Script
```bash
python social_media_sentiment_analysis.py
```

## 🔍 Predicting Custom Text
At the end of the script, there’s a function:
```python
predict_sentiment("I love the new update on Instagram!")
```
You can modify this with any sentence to test the model’s prediction in real-time.

## 📌 Notes
- Only a sample of 30,000 tweets is used for faster training.
- For better accuracy, use the full dataset or fine-tune with additional data.
- You can integrate this model into a web app using Streamlit or Flask.
