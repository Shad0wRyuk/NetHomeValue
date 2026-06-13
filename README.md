<div align="center">

# 🏠 HomeNetValue
### Real Estate Market Analyzer — Predicting House Prices with Machine Learning

<br/>

![Python](https://img.shields.io/badge/Python-3.10-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Scientific-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-2ea44f?style=for-the-badge)

<br/>

> *"Predicting the Future of Real Estate with Machine Learning."*

<br/>

[📊 Explore the Notebook](#-project-structure) · [🤖 Model Details](#-machine-learning-pipeline) · [🔮 Try a Prediction](#-sample-prediction) · [🚀 Future Plans](#-future-improvements)

</div>

---

## 📌 Overview

**HomeNetValue** is an end-to-end Machine Learning project that predicts **house prices per unit area** using real estate attributes. It walks through the complete ML lifecycle — from raw data to a saved, reusable model — making it a great reference for aspiring data scientists.

<br/>

| Stage | What's Covered |
|-------|---------------|
| 📊 Data | Collection, exploration, and analysis |
| 🧹 Preprocessing | Cleaning, scaling, train-test split |
| 🔍 Analysis | Correlation heatmaps, outlier detection |
| 📈 Visualization | Matplotlib & Seaborn plots |
| ⚙️ Engineering | Feature pipelines |
| 🤖 Modeling | Random Forest Regressor |
| 🎯 Tuning | GridSearchCV hyperparameter optimization |
| 💾 Deployment | Model serialization with Joblib |

---

## 📂 Dataset

**Real Estate Valuation Dataset** — 414 records, 8 columns

| Feature | Name | Description |
|---------|------|-------------|
| `X1` | Transaction Date | Year of the transaction |
| `X2` | House Age | Age of the house (years) |
| `X3` | Distance to MRT | Distance to nearest MRT station (meters) |
| `X4` | Convenience Stores | Number of nearby convenience stores |
| `X5` | Latitude | Geographic latitude |
| `X6` | Longitude | Geographic longitude |
| `Y` ⭐ | **House Price** | Price per unit area *(Target Variable)* |

---

## 🛠️ Tech Stack

<div align="center">

| Category | Tools |
|----------|-------|
| Language | Python 3.10 |
| Data Wrangling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-Learn |
| Model Persistence | Joblib |
| Environment | Google Colab |

</div>

---

## 🤖 Machine Learning Pipeline

```
Raw Data ──► Preprocessing ──► Feature Engineering ──► Model Training ──► Tuning ──► Prediction
```

### Preprocessing Steps
- ✅ Missing value handling
- ✅ Feature scaling (StandardScaler)
- ✅ Train-test split (80/20)
- ✅ Full Scikit-Learn Pipeline

### Model
> **Random Forest Regressor** — an ensemble of decision trees that reduces overfitting and handles non-linear relationships well.

### Hyperparameter Tuning
Optimized via **GridSearchCV** with cross-validation:

```python
Best Parameters Found:
{
    'n_estimators':    300,
    'max_depth':       10,
    'min_samples_split': 5
}
```

---

## 📈 Model Performance

<div align="center">

| Metric | Score |
|--------|-------|
| 🎯 R² Score | **0.8161** |
| 📉 RMSE | **5.5538** |

</div>

> An R² of **0.82** means the model explains ~82% of the variance in house prices — solid performance for a 414-row real-world dataset.

---

## 🔮 Sample Prediction

**Input Features:**
```python
{
    "Transaction Date":      2013.5,
    "House Age":             15,
    "Distance to MRT":       300,     # meters
    "Convenience Stores":    5,
    "Latitude":              24.97,
    "Longitude":             121.54
}
```

**Predicted Output:**
```
🏷️  House Price per Unit Area = 46.79
```

---

## 📁 Project Structure

```
HomeNetValue/
│
├── 📓 HomeNetValue.ipynb                     ← Main Jupyter Notebook
├── 🤖 house_price_model.pkl                  ← Saved ML Model
├── 📊 Real estate valuation data set.xlsx    ← Dataset
├── 📄 README.md                              ← You're here!
└── 📦 requirements.txt                       ← Dependencies
```

---

## ⚡ Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/Shad0wRyuk/HomeNetValue.git
cd HomeNetValue

# 2. Install dependencies
pip install -r requirements.txt

# 3. Open the notebook
jupyter notebook HomeNetValue.ipynb
```

Or open directly in **Google Colab** — no local setup needed.

---

## 🚀 Future Improvements

- [ ] 🌐 Deploy as a **Streamlit Web App**
- [ ] 📊 Add an **interactive dashboard** (Plotly / Dash)
- [ ] 🚀 Experiment with **XGBoost / LightGBM** for better accuracy
- [ ] 🔄 Integrate **real-time real estate data** via APIs
- [ ] ☁️ Deploy on **AWS / GCP / Render**
- [ ] 🧪 Add unit tests and CI/CD pipeline

---

## 👨‍💻 Author

<div align="center">

<img src="https://github.com/Shad0wRyuk.png" width="100" style="border-radius:50%"/>

### Kartik Sharma
*Machine Learning Enthusiast · Python Developer · Data Analytics*

[![GitHub](https://img.shields.io/badge/GitHub-Shad0wRyuk-181717?style=for-the-badge&logo=github)](https://github.com/Shad0wRyuk)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Kartik%20Sharma-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/kartiksharma2005)
[![Gmail](https://img.shields.io/badge/Gmail-k4rtik.09@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:k4rtik.09@gmail.com)

</div>

---

<div align="center">

**If this project helped you, please consider giving it a ⭐ — it means a lot!**

*Made with Python & Machine Learning*

</div>
