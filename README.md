<div align="center">

# 🌧️ Rainfall Prediction using Machine Learning 🚀

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-orange.svg)](https://pandas.pydata.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-1.7%2B-lightblue.svg)](https://xgboost.readthedocs.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)


![Demo GIF](screenshots/demo.gif)
### Predicting Rain Today, Planning Better Tomorrow ☁️📊

</div>

## 🚀 Project Overview

This project focuses on predicting rainfall using historical weather data and machine learning models.
It demonstrates a complete ML pipeline — from **data preprocessing** to **model building** and **prediction system deployment**.

---

## 🎯 Key Features

* 📊 Data preprocessing and feature selection
* 🤖 Multiple machine learning models implemented
* 📈 Model comparison and evaluation
* 🌐 Simple prediction system (using trained model)
* 📉 Data visualization for better insights

---

# 🔍 What I did:

• Built and compared ML models including Random Forest, KNN, and Gaussian Naive Bayes

• Achieved 83.8% accuracy, improving prediction reliability

• Performed data cleaning, preprocessing, and exploratory data analysis on multi-year datasets

• Applied feature engineering to enhance model performance


# 💡 Going beyond modeling:

• Designed system architecture using UML diagrams (Use Case, Class, Sequence, Activity) for structured development and knowledge sharing

• Developed a Flask-based web interface to generate real-time rainfall predictions

• Created detailed research documentation for academic and reporting purposes

---

## 📂 Project Structure

```bash
Rainfall-Prediction/
│
├── Data Preprocessing.ipynb
├── dt.pkl
├── GaussianNB Model.ipynb
├── Feature Selection.ipynb
├── Logistic Regression Model.ipynb
├── LogisticRegression.pkl
├── Decision Tree model.ipynb
├── Random Forest model.ipynb
├── SVC Model.ipynb
├── svc.pkl
├── KNeighbors Classifier Model.ipynb
├── GaussianNB Model.ipynb
├── gnb.pkl
├── Xgboost model.ipynb
├── xg_random
├── Catboost model.ipynb
├── cat.pkl
│
├── app.py                     # Prediction system
├── requirements.txt          # Dependencies
├── weatherAUS.csv            # Dataset (optional)
│
├── templates/                # HTML files (if UI exists)
├── static/                   # CSS/JS files
│
└── README.md
```

---


## 📊 Dataset
- **Source**: https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package
- **Features**: 15 columns including Location, MinTemp, MaxTemp, RainfallAmount, Evaporation, Sunshine, WindGustSpeed, Humidity, Pressure, Cloud, WindDir, RainToday.
- **Size**: 50k+ samples, preprocessed for missing values (imputation) and outliers.
- **Target**: Continuous rainfall (mm)—regression problem.

## 🛠️ Tech Stack
| Category     | Tools                          |
|--------------|--------------------------------|
| Language    | Python 3.8+                   |
| ML Framework| Scikit-learn, XGBoost         |
| Data        | Pandas, NumPy, Matplotlib     |
| Viz         | Seaborn, Plotly               |
| Environment | Jupyter Notebook, Conda       |

## 💻 Environment Setup
1. Clone the repo:
   ```bash
   git clone https://github.com/Devikalahari03/Rainfall-Prediction-using-Machine-Learning.git
   cd Rainfall-Prediction-using-Machine-Learning
   ```
2. Create virtual env:
   ```bash
   conda create -n rainfall python=3.8
   conda activate rainfall
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
## ▶️ How to Run the Project

### 📌 Run Notebooks

1. Open project in **VS Code**
2. Install Python & Jupyter extensions
3. Run notebooks step-by-step:

   * Data Preprocessing
   * Feature Selection
   * Model Building

---

### 🌐 Run Web App (if app.py exists)

```bash
python app.py
```

Then open in browser:

```
http://127.0.0.1:5000/
```

---


## 📈 Results

* Compared multiple ML models for rainfall prediction
* Identified best-performing model based on accuracy
* Generated insights from weather features

# Output screens

# <img width="1898" height="857" alt="Screenshot 2025-06-19 231944" src="https://github.com/user-attachments/assets/3b0a2b17-ae33-44bc-b05c-a329d52f1b5e" />
# <img width="1310" height="586" alt="Screenshot 2025-06-19 134449" src="https://github.com/user-attachments/assets/886e789d-d48f-446a-8eaa-3329608abd5e" />
# <img width="1303" height="562" alt="Screenshot 2025-06-19 134948" src="https://github.com/user-attachments/assets/d46c6f7f-be0f-478e-b506-635102b76ca8" />
# <img width="1395" height="841" alt="Screenshot 2026-05-01 210040" src="https://github.com/user-attachments/assets/c2b74293-409e-4489-8a40-3228679277d1" />
# <img width="1426" height="850" alt="Screenshot 2026-05-01 205856" src="https://github.com/user-attachments/assets/c4eec612-fdcc-40ee-948e-218291666dfc" />

---

## 💡 Key Learnings

* Importance of data cleaning and preprocessing
* Feature selection improves model performance
* Model comparison helps choose best algorithm
* End-to-end ML workflow implementation

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!

---

## 👩‍💻 Author

**Devika Lahari**































































































































