# 🤖 Machine Learning — From Basics to Advanced

Machine Learning AI ka sabse powerful branch hai jahan computers data se automatically seekhte hain bina explicit programming ke.

---

## 📂 Module Structure:

### Day 31: [`day31_ml_introduction.ipynb`](day31_ml_introduction.ipynb) — ML Foundations
- 🔵 **What is Machine Learning?** — Core definitions (Arthur Samuel & Tom Mitchell)
- 🗺️ **3 Types of ML:**
  - 1️⃣ **Supervised Learning** — Labels ke saath (Regression vs Classification)
  - 2️⃣ **Unsupervised Learning** — Bina labels ke (Clustering, Dimensionality Reduction)
  - 3️⃣ **Reinforcement Learning** — Agent, Environment, Rewards, Bellman Equation
- 📈 **Regression Deep Dive** — Formulas, MSE loss, evaluation metrics
- 🛠️ `scikit-learn` setup

---

### Day 32: [`day32_linear_regression.ipynb`](day32_linear_regression.ipynb) — End-to-End Linear Regression Project
- 📊 **Dataset:** Medical Cost Personal Datasets (`insurance.csv`, 1,338 records)
- 🎯 **Target:** `charges` (Continuous Medical Cost)
- 🔍 **Full EDA Pipeline:**
  - Feature distributions (histograms & bar charts)
  - Target vs Feature relationships (Scatter & Boxplots)
  - Correlation Heatmap
- ⚙️ **Preprocessing & Feature Engineering:**
  - Categorical Encoding (`sex`, `smoker` binary, `region` one-hot)
  - **Interaction Feature (`bmi × smoker`):** Captured non-linear cost explosion for obese smokers!
- 🤖 **Model Training:** Scikit-Learn `LinearRegression()`
- 📊 **Rigorous Evaluation:**
  - **Baseline $R^2$:** 78.36% $\to$ **Improved $R^2$:** **86.53%** 🚀
  - **Adjusted $R^2$:** **86.05%** (Penalized Metric)
  - **MAE:** Dropped from \$4,181 down to **\$2,757**
  - **RMSE:** Dropped from \$5,796 down to **\$4,460**
- 📉 **3 Comprehensive Visualizations:**
  1. Actual vs Predicted Charges (tightly aligned along the $y=x$ diagonal)
  2. Residuals Plot (random distribution around zero error line)
  3. Feature Importance (Coefficients magnitude comparison)

---

## 🛠️ Libraries Used:
- `scikit-learn` — Model training, metrics, train/test split
- `pandas` — Data manipulation & encoding
- `numpy` — Mathematical calculations & array transformations
- `matplotlib` & `seaborn` — Statistical visualizations & heatmaps
