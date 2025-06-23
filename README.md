# Amazon-Review-Sentiment-Analysis

This project is a sentiment analysis tool for Amazon product reviews. It allows users to input a sentence or upload a CSV file of reviews and returns whether the sentiment is Positive or Negative using a trained machine learning model. The tool features a clean web interface built with Streamlit and an API backend powered by Flask.

---

## Screenshots

### 🔹 Single Text Input Prediction  
![Single Text Prediction](screenshots/single_prediction.png)

### 🔹 Bulk CSV Upload and Download  
![Bulk Prediction](screenshots/bulk_prediction.png)

---

## Project Structure

.
├── main.py # Streamlit frontend
├── api.py # Flask backend API
├── Models/ # Trained model, scaler, and vectorizer
│ ├── model_xgb.pkl
│ ├── scaler.pkl
│ └── countVectorizer.pkl
├── templates/
│ └── landing.html # Optional landing page (Flask)
├── requirements.txt
└── README.md

---
# How to Run Locally

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/amazon-review-sentiment-analysis.git
cd amazon-review-sentiment-analysis '''

### 2. Create and Activate Virtual Environment (optional but recommended)

```bash
# macOS/Linux
python3 -m venv venv
source venv/bin/activate '''

```bash
# Windows
python -m venv venv
venv\Scripts\activate '''

### 3. Install Requirements

```bash
pip install -r requirements.txt'''

### 4. Run the API

```bash
python3 api.py '''

### 5. In a new terminal, run the Streamlit frontend

```bash
streamlit run main.py '''
