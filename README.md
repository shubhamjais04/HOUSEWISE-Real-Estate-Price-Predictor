# 🏠 HOUSEWISE — Real Estate Price Predictor

A machine learning system that predicts residential property prices instantly — built on 21,613 real house transactions from King County, Seattle. Enter 5 property details, get an instant data-driven price estimate through an interactive web interface.

---

## 🌐 Web Interface

**Input Form — Enter property details:**
![HOUSEWISE Input Interface](screenshots/interface_without_result.jpg)

**Prediction Output — Instant price estimate:**
![HOUSEWISE Prediction Result](screenshots/interface_with_result.jpg)

---

## 📌 Project Overview

Traditional property valuation relies on agent expertise and manual comparisons — inconsistent, time-consuming, and prone to human bias. HOUSEWISE replaces guesswork with a data-driven ML pipeline that covers the full lifecycle: raw data → EDA → feature engineering → model training → evaluation → deployed web application.

---

## 🏆 Model Performance

| Metric | Linear Regression | Random Forest |
|--------|------------------|---------------|
| R² Score (Test) | 0.49 | **0.53** |
| RMSE | ~$272,080 | **~$266,541** |
| MAE | ~$175,000 | **~$160,103** |
| MAPE | ~33% | **~31.38%** |
| **Selected** | ❌ | ✅ **Final Model** |

> Random Forest Regressor selected as the final model — outperformed Linear Regression across all four metrics.

---

## ✨ What's Covered

- 📥 Data loading and inspection — 21,613 rows, 21 columns
- 📊 Exploratory Data Analysis — price distribution, correlation heatmap, scatter plots
- ⚙️ Feature engineering — 5 key features selected from 21 available columns
- 📐 Data preparation — 80/20 train-test split, StandardScaler normalization
- 🤖 Model training — Linear Regression (baseline) vs Random Forest (final)
- 📈 Model evaluation — R², RMSE, MAE, MAPE comparison
- 💾 Model persistence — saved with Pickle for reuse without retraining
- 🌐 Web deployment — interactive Gradio interface for non-technical users

---

## 🔍 Key Insights

| Finding | Detail |
|---------|--------|
| Strongest predictor | `sqft_living` — highest correlation with price |
| Bathrooms > Bedrooms | Bathrooms have stronger price impact than bedroom count |
| Price distribution | Right-skewed — most houses priced between $200K–$800K |
| Mean price | $540,088 |
| Median price | $450,000 |

---

## 💡 Sample Predictions

| Bedrooms | Bathrooms | Living Area | Lot Size | Floors | Predicted Price |
|----------|-----------|-------------|----------|--------|----------------|
| 3 | 2 | 2,000 sqft | 5,000 sqft | 1 | $625,777 |
| 5 | 3.5 | 3,500 sqft | 8,000 sqft | 2.5 | $1,110,857 |
| 8 | 4 | 6,000 sqft | 10,000 sqft | 5 | $1,800,413 |

---

## 📊 Dataset

- **Source:** King County House Sales Dataset — Kaggle
- **Records:** 21,613 residential property transactions
- **Region:** Seattle, Washington, USA
- **Features:** 21 columns — property attributes, sale prices, location details
- **Target Variable:** `price` (house sale price in USD)

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4B8BBE?style=for-the-badge&logo=python&logoColor=white)
![Gradio](https://img.shields.io/badge/Gradio-FF7C00?style=for-the-badge&logo=gradio&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 📁 Project Structure

```
HOUSEWISE/
├── data/                              # King County house sales dataset
├── images/                            # EDA plots and visualizations
├── models/                            # Saved model and scaler (pickle)
├── screenshots/
│   ├── interface_without_result.jpg   # Gradio input form
│   └── interface_with_result.jpg      # Gradio prediction output
├── Housewise.ipynb                    # Main ML notebook
└── README.md                          # Project documentation
```


---

## 🚀 How to Run

**1. Clone the repository**
```bash
git clone https://github.com/shubhamjais04/HOUSEWISE.git
cd HOUSEWISE
```

**2. Install dependencies**
```bash
pip install pandas numpy scikit-learn matplotlib seaborn gradio jupyter
```

**3. Open the notebook**
```bash
jupyter notebook Housewise.ipynb
```

**4. Run all cells in order**

**5. Launch the Gradio web interface**

The last cell in the notebook launches the interactive web app — open the local URL in your browser and start predicting prices instantly.

---

## 👨‍💻 Author

**Shubham Jaiswal**   
*ML engineer | Building data-driven tools that bring transparency to real-world decisions*

---

## 📬 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/shubhjais04)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/shubhamjais04)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shubhjais.in@gmail.com)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/shubhamjaiswal04)






