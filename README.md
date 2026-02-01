# 🧠 Duplicate Question Detection Using NLP

A Machine Learning + NLP based web application that detects whether two input questions are **duplicates or not**.  
The project uses **Bag of Words (BoW)** along with handcrafted similarity features and fuzzy matching, deployed using **Streamlit**.

---

## 🚀 Project Overview

Online platforms often receive semantically similar questions phrased differently.  
This project solves that problem by:

- Text preprocessing  
- NLP feature extraction  
- Bag of Words vectorization  
- Machine Learning classification  
- Streamlit web deployment  

Users can enter two questions and instantly see whether they are **Duplicate** or **Not Duplicate**.

---

## 🛠 Tech Stack

- Python  
- Natural Language Processing (NLP)  
- Machine Learning (Scikit-learn)  
- Streamlit  
- Matplotlib & Seaborn  

---

## 📂 Dataset

Quora Question Pairs Dataset

Columns:
- id  
- qid1  
- qid2  
- question1  
- question2  
- is_duplicate  

Total rows: ~404k  
Sampled 30k rows for training.

---

## 🔑 Features

### Text Preprocessing
- Lowercasing
- HTML removal
- De-contractions
- Special character cleaning

### Basic Features
- Question length
- Word count
- Common words
- Word share

### Advanced NLP Features
- Stopword ratios
- Token overlap
- First/last word match
- Length difference
- Longest common substring

### Fuzzy Matching
- QRatio
- Partial Ratio
- Token Sort Ratio
- Token Set Ratio

### Vectorization
- Bag of Words (CountVectorizer)

> TF-IDF is NOT used.

---

## 🤖 Model Pipeline

1. Preprocess questions  
2. Extract handcrafted features  
3. Apply Bag of Words  
4. Combine features  
5. Train ML classifier  
6. Save model + vectorizer  
7. Predict using Streamlit  

---

## 🖥 Web Application

Two inputs + Find button  
Displays:
- Duplicate  
- Not Duplicate  

---

## 📁 Project Structure

├── app.py  
├── helper.py  
├── model.pkl  
├── cv.pkl  
├── requirements.txt  
├── setup.sh  
├── Procfile  
├── notebooks  

---

## ▶️ Run Locally

### Install dependencies
pip install -r requirements.txt

### Download stopwords
python -c "import nltk; nltk.download('stopwords')"

### Run app
streamlit run app.py

---

## 📈 Visualizations

Performed using Matplotlib & Seaborn:
- Class distribution
- Length analysis
- Similarity metrics

---

## 💡 Future Improvements

- TF-IDF / embeddings
- Deep Learning (Siamese / BERT)
- Probability scores
- Better UI

---

## 👩‍💻 Author

Aashi Chahal  
CDAC Student | NLP & ML Enthusiast
