## 🌧️ Rainfall Prediction using Machine Learning

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Flask-Web%20App-black?style=for-the-badge&logo=flask&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-ML-orange?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Accuracy-83.86%25-brightgreen?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge"/>
</p>

<p align="center">
  <b>A full-stack Machine Learning web application that predicts whether tomorrow will be a Rainy Day ☔ or Sunny Day ☀️</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/M.Sc.-Computer%20Science-purple?style=flat-square"/>
  <img src="https://img.shields.io/badge/University-Adikavi%20Nannaya%20University-red?style=flat-square"/>
  <img src="https://img.shields.io/badge/Year-2023--2025-blue?style=flat-square"/>
</p>

---

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [Demo](#-demo)
- [Features](#-features)
- [Dataset](#-dataset)
- [ML Algorithms Used](#-ml-algorithms-used)
- [Model Comparison](#-model-comparison)
- [System Architecture](#-system-architecture)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Installation & Setup](#-installation--setup)
- [How to Use](#-how-to-use)
- [Results](#-results)
- [Future Work](#-future-work)
- [Author](#-author)
- [Acknowledgements](#-acknowledgements)

---

## 🌟 About the Project

Rainfall prediction is one of the most challenging problems in meteorology, with huge real-world impact on:

- 🌾 **Agriculture** — Crop planning and irrigation management
- 💧 **Water Resource Management** — Reservoir and dam operations
- 🌊 **Flood Control** — Early warning systems
- 🚨 **Disaster Management** — Evacuation planning
- 🏙️ **Urban Planning** — Drainage and infrastructure

This project builds a **supervised machine learning model** trained on historical weather data to predict whether it will rain the next day. It includes a **Flask web application** with an interactive predictor interface, deployed locally using Python.


---

## 🎬 Demo

| Home Page | Prediction Form | Rainy Day Output | Sunny Day Output |
|:---------:|:---------------:|:----------------:|:----------------:|
| <img width="1898" height="857" alt="Screenshot 2025-06-19 231944" src="https://github.com/user-attachments/assets/3b0a2b17-ae33-44bc-b05c-a329d52f1b5e" /> |  <img width="1310" height="586" alt="Screenshot 2025-06-19 134449" src="https://github.com/user-attachments/assets/886e789d-d48f-446a-8eaa-3329608abd5e" /> | <img width="1395" height="841" alt="Screenshot 2026-05-01 210040" src="https://github.com/user-attachments/assets/c2b74293-409e-4489-8a40-3228679277d1" /> | <img width="1426" height="850" alt="Screenshot 2026-05-01 205856" src="https://github.com/user-attachments/assets/c4eec612-fdcc-40ee-948e-218291666dfc" /> |

---

## ✨ Features

- ✅ Predicts next-day rainfall as **Rainy** or **Sunny**
- ✅ Interactive web form to input 23 weather parameters
- ✅ Compares **3 ML algorithms** (Random Forest, KNN, Gaussian Naïve Bayes)
- ✅ **Random Forest** selected as best model with **83.86% accuracy**
- ✅ Trained on a large dataset of **9,15,355 weather records**
- ✅ Full ML pipeline: Data Preprocessing → Feature Selection → Training → Evaluation → Deployment
- ✅ Clean, responsive UI built with Bootstrap 5

---

## 📊 Dataset

| Property | Details |
|----------|---------|
| **Source** | [Kaggle – Rain in Australia](https://www.kaggle.com/) |
| **Records** | 9,15,355 rows |
| **Features** | 23 columns |
| **Target Variable** | `RainTomorrow` (0 = Sunny, 1 = Rainy) |
| **Train Split** | 80% |
| **Test Split** | 20% |

### 📋 Dataset Attributes

| # | Feature | Type |
|---|---------|------|
| 1 | Date | Nominal |
| 2 | Location | Nominal |
| 3 | MinTemp | Continuous |
| 4 | MaxTemp | Continuous |
| 5 | Rainfall | Continuous |
| 6 | Evaporation | Continuous |
| 7 | Sunshine | Continuous |
| 8 | WindGustDir | Nominal |
| 9 | WindGustSpeed | Continuous |
| 10 | WindDir9am | Nominal |
| 11 | WindDir3pm | Nominal |
| 12 | WindSpeed9am | Continuous |
| 13 | WindSpeed3pm | Continuous |
| 14 | Humidity9am | Continuous |
| 15 | Humidity3pm | Continuous |
| 16 | Pressure9am | Continuous |
| 17 | Pressure3pm | Continuous |
| 18 | Cloud9am | Continuous |
| 19 | Cloud3pm | Continuous |
| 20 | Temp9am | Continuous |
| 21 | Temp3pm | Continuous |
| 22 | RainToday | Nominal |
| 23 | **RainTomorrow** | **Target** |

---

## 🤖 ML Algorithms Used

### 1. 🌲 Random Forest
An ensemble learning method that builds multiple decision trees on random subsets of the data and takes a majority vote for prediction.

**Why Random Forest?**
- Handles large datasets efficiently
- Resistant to overfitting (averages multiple trees)
- Works for both classification and regression
- High accuracy on tabular weather data

**How it works:**
```
1. Select random samples from the dataset
2. Build a decision tree for each sample
3. Collect predictions from all trees
4. Take majority vote → Final prediction
```

---

### 2. 📐 K-Nearest Neighbor (KNN)
Classifies a new data point based on the majority class of its K nearest neighbors using Euclidean distance.

```
d(x, y) = √ Σ(xᵢ - yᵢ)²
```

**Advantages:** Simple to implement, robust to noisy data, effective on large datasets.

---

### 3. 📊 Gaussian Naïve Bayes (GNB)
A probabilistic classifier based on Bayes' theorem that assumes features follow a Gaussian (Normal) distribution.

```
P(C|X) = [P(X|C) × P(C)] / P(X)
```

**Advantages:** Fast, works well with multi-class problems, ideal for continuous data.

---

## 📈 Model Comparison

| Model | Accuracy |
|-------|----------|
| 🥇 **Random Forest** | **83.86%** |
| 🥈 K-Nearest Neighbor (KNN) | 74.78% |
| 🥉 Gaussian Naïve Bayes | 74.48% |

```
Accuracy (%)
│
85 ┤  ████████████
83 ┤  ████████████   
75 ┤  ████████████  ██████████  ██████████
70 ┤  ████████████  ██████████  ██████████
   └─────────────────────────────────────
      Random Forest    KNN         GNB
```

> ✅ **Random Forest** was selected as the final deployed model due to its superior accuracy.

---

## 🏗️ System Architecture

```
Real Dataset (Kaggle)
        │
        ▼
  Data Pre-processing
  (Handle nulls, encode, scale)
        │
        ▼
  Feature Selection
        │
        ├──────────────────┐
        ▼                  ▼
  Training Set (80%)  Testing Set (20%)
        │                  │
        └──────────┬───────┘
                   ▼
        Model Training & Evaluation
        (RF / KNN / GNB)
                   │
                   ▼
          Rainfall Prediction
          (Rainy ☔ / Sunny ☀️)
```

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|-----------|
| **Language** | Python 3.x |
| **Web Framework** | Flask |
| **ML Library** | Scikit-learn |
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Frontend** | HTML5, CSS3, Bootstrap 5 |
| **IDE** | Jupyter Notebook / PyCharm |
| **Environment** | Anaconda Navigator |
| **Model Format** | Pickle (.pkl) |

---

## 📁 Project Structure

```
Rainfall-Prediction-using-Machine-Learning/
│
├── app.py                      # Flask main application
├── xg_random.pkl               # Trained Random Forest model (pickle)
│
├── template/
│   ├── index.html              # Home page
│   ├── Predictor.html          # Prediction form page
│   ├── after_rainy.html        # Rainy day result page
│   └── after_sunny.html        # Sunny day result page
│
├── static/
│   ├── style1.css              # Home page styles
│   └── Predictor.css           # Predictor form styles
│
├── dataset/
│   └── rainfall_data.csv       # Kaggle weather dataset
│
├── notebooks/
│   └── Rainfall_Prediction.ipynb  # Model training notebook
│
├── screenshots/                # App screenshots (add your own)
│
├── requirements.txt            # Python dependencies
└── README.md                   # This file
```

---

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.x
- pip / Anaconda

### Step 1: Clone the Repository
```bash
git clone https://github.com/Devikalahari03/Rainfall-Prediction-using-Machine-Learning.git
cd Rainfall-Prediction-using-Machine-Learning
```

### Step 2: Create Virtual Environment (Recommended)
```bash
python -m venv venv
source venv/bin/activate        # On Linux/Mac
venv\Scripts\activate           # On Windows
```

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

Or install manually:
```bash
pip install flask flask-cors pandas numpy scikit-learn matplotlib seaborn xgboost pickle5
```

### Step 4: Run the Application
```bash
python app.py
```

### Step 5: Open in Browser
```
http://127.0.0.1:5000/
```

---

## 🖥️ How to Use

1. Open the app in your browser at `http://127.0.0.1:5000/`
2. Click on **"Predictor"** in the navigation bar
3. Fill in the weather parameters:
   - Date, Location
   - Min/Max Temperature
   - Rainfall, Evaporation, Sunshine
   - Wind Gust Speed & Direction
   - Wind Speed (9am / 3pm)
   - Humidity (9am / 3pm)
   - Pressure (9am / 3pm)
   - Cloud Cover (9am / 3pm)
   - Temperature (9am / 3pm)
   - Rain Today
4. Click **"Predict"**
5. View your result: ☔ **RAINY DAY** or ☀️ **SUNNY DAY**

---

## 📉 Data Preprocessing Steps

```python
# 1. Load Dataset
df = pd.read_csv('rainfall_data.csv')

# 2. Handle Missing Values
from sklearn.impute import SimpleImputer
imputer = SimpleImputer(strategy='mean')

# 3. Encode Categorical Variables
from sklearn.preprocessing import LabelEncoder

# 4. Split Dataset
from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test = train_test_split(
    x, y, test_size=0.2, random_state=20
)

# 5. Train Random Forest
from sklearn.ensemble import RandomForestClassifier
model = RandomForestClassifier()
model.fit(x_train, y_train)
```

---

## 📊 Results

### Sample Predictions

| Date | Location | Min Temp | Max Temp | Humidity | Result |
|------|----------|----------|----------|----------|--------|
| 01-12-2008 | Albury | 13.4 | 22.9 | 71 | ☀️ Sunny |
| 11-01-2009 | BadgerysCreek | 12.6 | 30.2 | 61 | ☔ Rainy |
| 02-01-2009 | Cobar | 18.4 | 28.9 | 30 | ☀️ Sunny |
| 02-01-2009 | CoffsHarbour | 22.8 | 24.7 | 66 | ☔ Rainy |

### Model Accuracy Summary

```
Random Forest  ████████████████████████████████ 83.86%
KNN            ████████████████████████████     74.78%
Gaussian NB    ████████████████████████████     74.48%
```

---

## 🔮 Future Work

- [ ] Extend model to predict **exact rainfall amount** (mm), not just binary classification
- [ ] Apply **Ensemble Learning** techniques (Voting, Stacking) for improved accuracy
- [ ] Train on **unlabeled data** using semi-supervised learning
- [ ] Add **real-time weather API integration** (e.g., OpenWeatherMap)
- [ ] Deploy on **Heroku / AWS / Render** for public access
- [ ] Add **date-wise comparative analysis** of rainfall patterns
- [ ] Extend dataset to include **more Indian states** beyond Andhra Pradesh

---
## 👩‍💻 Author
Devika Lahari

🎓 M.Sc. Computer Science 
🏛️ Adikavi Nannaya University, Rajamahendravaram (2023–2025)
🔗 GitHub

---

## 🙏 Acknowledgements

University: Adikavi Nannaya University, Rajamahendravaram
Dataset: Kaggle – Rain in Australia
Libraries: Scikit-learn, Flask, Pandas, NumPy, Matplotlib, Seaborn

---

<p align="center">
  ⭐ <b>If you found this project helpful, please give it a star!</b> ⭐
  <br><br>
  Made with ❤️ by <b>Bandi Devika Lahari</b>
</p>



-

































































































































