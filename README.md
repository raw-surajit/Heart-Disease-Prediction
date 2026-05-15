# ❤️ Heart Disease Prediction Portal

An end-to-end Machine Learning web application that predicts the risk of heart disease based on clinical parameters. Built with Python, Scikit-Learn, and Streamlit.

## 🚀 Project Overview
This project focuses on identifying risk factors for heart disease using clinical data. After evaluating multiple classification algorithms including K-Nearest Neighbors (KNN), Support Vector Machines (SVM), and Decision Trees, **Logistic Regression** was selected as the final model due to its superior accuracy and reliability on this specific dataset.

The application allows users to input health metrics via a user-friendly interface and provides an instant risk assessment (High Risk vs. Low Risk).

## 🛠️ Tech Stack
* **Language:** Python 3.12
* **Modeling:** Scikit-Learn, Pandas, NumPy
* **Web Framework:** Streamlit
* **Environment Management:** Virtualenv (venv)
* **Development:** VS Code & Google Colab

## 📊 Features & Parameters
The model analyzes 11 core clinical features to predict the risk status:
* **Demographics:** Age, Sex
* **Chest Pain Type:** (Typical Angina, Atypical Angina, Non-Anginal, Asymptomatic)
* **Vitals:** Resting Blood Pressure, Cholesterol, Fasting Blood Sugar
* **Cardiac Tests:** Resting ECG (Normal, ST, LVH), Max Heart Rate, Exercise-Induced Angina
* **Advanced Metrics:** Oldpeak (ST Depression), ST Slope (Up, Flat, Down)

## 📁 Project Structure
```text
├── .venv/               # Virtual environment (Local only)
├── .gitignore           # Excludes .venv and temp files from GitHub
├── Heartdisease.ipynb   # Jupyter Notebook for EDA & Model Training
├── app.py               # Streamlit application frontend code
├── heart.csv            # Raw dataset used for training
├── requirements.txt     # List of Python dependencies
├── LogisticRegression_heart_model.pkl  # The trained "Brain" of the app
├── heart_scaler.pkl     # Pre-fitted StandardScaler for inputs
└── heart_columns.pkl    # Serialized list of expected model columns


## ⚙️ Installation & Usage

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/heart-disease-prediction.git
cd heart-disease-prediction
```

### 2️⃣ Create & Activate Virtual Environment

```bash
python -m venv .venv
```

#### Windows

```bash
.\.venv\Scripts\activate
```

#### Linux / macOS

```bash
source .venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Application

```bash
streamlit run app.py
```

## 📈 Model Performance

Based on the experimental phase documented in the notebook, the Logistic Regression model achieved:

* **Accuracy:** ~89%
* **Reliability:** High balance between Precision and Recall, making it suitable for educational diagnostic assistance.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

**Disclaimer:** This tool is for educational purposes and is not a substitute for professional medical advice, diagnosis, or treatment.