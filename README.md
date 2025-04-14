```markdown
# 🧬 Disease Classification Dashboard: TF-IDF vs One-Hot Encoding

This project presents an interactive **Streamlit** application that compares **TF-IDF** and **One-Hot Encoding** for disease classification based on medical text data. It integrates feature extraction, dimensionality reduction, model evaluation, and real-time prediction capabilities.

---

## 📚 Overview

- **Vectorization Methods:** TF-IDF and One-Hot Encoding
- **Dimensionality Reduction:** PCA & Truncated SVD
- **Classification Models:** K-Nearest Neighbors (KNN) and Logistic Regression
- **Evaluation:** Cross-validation, performance metrics, visual analytics
- **Interactive Features:** User input-based disease prediction, encoding & model selection

---

## 🚀 Features

### 📊 Task 1: TF-IDF Feature Extraction
- Converts stringified medical features (`Symptoms`, `Signs`, `Risk Factors`) into text format
- Applies TF-IDF vectorization to each feature group
- Combines TF-IDF matrices and compares with One-Hot encoding in terms of shape and sparsity

### 📉 Task 2: Dimensionality Reduction
- Applies **PCA** and **Truncated SVD** to both encoding types
- Plots 2D clusters categorized by disease group (e.g., Cardiovascular, Neurological)
- Displays explained variance ratios

### 🤖 Task 3: Model Evaluation
- Supports **KNN** (with configurable `k` and distance metrics) and **Logistic Regression**
- Performs **Stratified K-Fold Cross-Validation** (user-selectable folds)
- Metrics: Accuracy, Precision, Recall, F1-Score
- Full performance comparison heatmap and top 5 models ranking

### 🧪 Real-Time Prediction
- Accepts user input for symptoms, signs, and risk factors
- Uses TF-IDF with Logistic Regression to predict disease from new input

---

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/M-Sarim/disease-classification-nlp.git
cd disease-classification-nlp

# (Optional) Create a virtual environment
python -m venv env
source env/bin/activate  # For Windows: .\env\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

---

## 💻 Run the App

Make sure the required CSV files (`disease_features.csv` and `encoded_output2.csv`) are present in the root directory.

```bash
streamlit run app.py
```

---

## 🗂️ Project Structure

```
.
├── app.py                    # Streamlit application
├── disease_features.csv      # Feature dataset
├── encoded_output2.csv       # One-hot encoded labels
├── requirements.txt          # Python dependencies
├── disease_prediction.ipynb  # ipynb file
└── README.md                 
```

---

## 🧠 Disease Categories

The app categorizes diseases into:

- Cardiovascular
- Endocrine
- Neurological
- Respiratory
- Infectious
- Gastrointestinal

Each is color-coded in visualizations for better interpretability.

---

## 🧪 Supported Models & Metrics

- **KNN** (with adjustable `k` and distance metrics: Euclidean, Manhattan, Cosine)
- **Logistic Regression**
- Performance metrics include:
  - Accuracy
  - Precision
  - Recall
  - F1-score

---

## 🧠 Predictive Inference

You can simulate predictions by inputting symptoms, signs, and risk factors. The model will output the predicted disease using the trained logistic regression classifier.

---

## 🧾 License

This project is licensed under the [MIT License](LICENSE).

---

## ✍️ Author

- [Muhammad Sarim](https://www.linkedin.com/in/imuhammadsarim/)

Feel free to reach out for feedback or collaboration opportunities!

---

> “Combining interpretability, interactivity, and machine learning to uncover patterns in medical data.”
