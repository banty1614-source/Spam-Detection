# 📧 Spam Detection System

A Machine Learning project built using **Python** and **Scikit-learn** to classify SMS messages as **Spam** or **Ham (Not Spam)**.

---

## 📌 Project Overview

This project uses the **Multinomial Naive Bayes** algorithm to automatically detect whether an SMS message is spam based on the words present in the message.

The project demonstrates how text data can be transformed into numerical features using **CountVectorizer** and then used to train a machine learning model for classification.

---

## 🎯 Problem Statement

Spam messages are unwanted messages that often contain advertisements, scams, or misleading information.

The goal of this project is to build a model that can classify SMS messages into:

* **Spam**
* **Ham (Not Spam)**

---

## 📂 Dataset

The project uses the **SMS Spam Collection Dataset**.

Each message in the dataset is labeled as:

* `ham` → Legitimate message
* `spam` → Unwanted message

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

---

## 🧠 Machine Learning Concepts Used

* Text Classification
* Features and Labels
* Train-Test Split
* Count Vectorization
* Naive Bayes Classification
* Model Evaluation

---

## ⚙️ Data Preprocessing

### 1. Removed Unnecessary Columns

The original dataset contained extra empty columns, which were removed.

### 2. Renamed Columns

| Original | New     |
| -------- | ------- |
| v1       | label   |
| v2       | message |

### 3. Label Encoding

```text
ham  → 0
spam → 1
```

---

## 🔢 Text Vectorization

Machine learning models cannot understand raw text directly.

Therefore, the SMS messages were converted into numerical features using **CountVectorizer**.

### Example

Message:

```text
FREE FREE WINNER
```

Vectorized Form:

| Word   | Count |
| ------ | ----- |
| FREE   | 2     |
| WINNER | 1     |

---

## 🤖 Algorithm Used

### Multinomial Naive Bayes

Naive Bayes is a probability-based classification algorithm.

It predicts whether a message is spam by estimating the probability of each class and selecting the class with the highest probability.

---

## 🚀 Project Workflow

```text
Load Dataset
      ↓
Data Cleaning
      ↓
Label Encoding
      ↓
Train-Test Split
      ↓
CountVectorizer
      ↓
Train Naive Bayes Model
      ↓
Make Predictions
      ↓
Evaluate Accuracy
```

---

## 📊 Results

The model achieved an accuracy of approximately:

```text
98.39%
```

on the test dataset.

---

## 💬 Example Predictions

### Example 1

Message:

```text
Congratulations! You have won ₹50,000. Click here to claim your prize.
```

Prediction:

```text
Spam
```

---

### Example 2

Message:

```text
Tomorrow's meeting starts at 9 AM. Please bring the project report.
```

Prediction:

```text
Ham
```

---

## 📚 What I Learned

Through this project, I learned:

* How machine learning works with text data
* The importance of converting text into numerical representations
* How CountVectorizer transforms text into features
* The intuition behind Naive Bayes classification
* How to build a complete text classification pipeline using Scikit-learn

---

## 🔮 Future Improvements

* Use TF-IDF Vectorization
* Evaluate the model using Precision and Recall
* Build a simple web application using Streamlit
* Compare Naive Bayes with other classification algorithms

---

## 📁 Project Structure

```text
spam-detection-system/
│
├── Spam_Detection_System.ipynb
├── spam.csv
├── README.md
└── requirements.txt
```

---

## 👨‍💻 Author

**Banty Kumar**

Electrical Engineering Undergraduate at NIT Patna

Learning Machine Learning through practical projects and hands-on implementation.

---

⭐ If you found this project interesting, feel free to explore the code and provide feedback.

This project is part of my Machine Learning learning journey.
