# Sentiment Analysis with Python

A simple Python project that analyzes the **sentiment of a sentence** (Positive, Negative, or Neutral) using the TextBlob library.

## 🚀 Features

* Takes user input
* Analyzes sentiment using Natural Language Processing
* Classifies text as:

  * Positive
  * Negative
  * Neutral
* Beginner-friendly Python project

## 🧠 How It Works

The program uses the **TextBlob** library to calculate the **polarity score** of a sentence.

Polarity ranges from **-1 to 1**:

* Positive → greater than 0
* Negative → less than 0
* Neutral → equal to 0

## 📦 Requirements

* Python 3
* TextBlob

Install dependencies:

pip install textblob

Download required corpora:

python -m textblob.download_corpora

## 💻 Code

```python
from textblob import TextBlob

def analyze_sentiment(text):
    blob = TextBlob(text)
    sentiment_score = blob.sentiment.polarity

    if sentiment_score > 0:
        return "Positive"
    elif sentiment_score < 0:
        return "Negative"
    else:
        return "Neutral"

post = input("Enter a sentence: ")
print("Sentiment:", analyze_sentiment(post))
```

## ▶️ How to Run

1. Save the file as `sentiment.py`
2. Open terminal
3. Run the program

python sentiment.py

## 📷 Example

Enter a sentence: I love programming
Sentiment: Positive

Enter a sentence: I hate bugs
Sentiment: Negative

## 📚 Technologies Used

* Python
* TextBlob
* Natural Language Processing (NLP)

## 👨‍💻 Author

Advik

## ⭐ Contribute

Feel free to fork this repository and improve the project!

If you like this project, give it a **star ⭐** on GitHub.
