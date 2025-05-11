# cybersecurity-breach-analysis-ml
“End‑to‑end ML pipeline for detecting and clustering cybersecurity breaches.”
# 💳 Credit Card Fraud Detection with Explainable AI (SHAP)

A real-world machine learning solution for detecting credit card fraud using feature-rich preprocessing, class imbalance techniques, SHAP explainability, and XGBoost classification. This project includes impactful visualizations and model interpretability tools, ideal for stakeholder trust and real-time deployment.

---

## 🚀 Project Highlights

- 📦 Real-world fraud dataset with class imbalance
- 📊 Visual Exploratory Data Analysis with Plotly
- ⚙️ Models: XGBoost (with `scale_pos_weight` tuning)
- 📈 Model Evaluation: ROC Curve, AUC, GridSearchCV, Cross-Validation
- 🧠 Explainability with SHAP: global, local, and feature-level insights
- 🌐 Deployment-Ready with Streamlit UI potential

---

## 📂 Dataset

- **Source**: [Kaggle or domain-specific dataset] *(insert actual link if possible)*
- **Target Variable**: `Class` (1 = Fraud, 0 = Non-fraud)
- **Challenge**: Highly **imbalanced dataset** (typically <1% fraud)

---

## 🛠️ Technologies & Tools

| Category           | Tools / Libraries                              |
|-------------------|--------------------------------------------------|
| Language          | Python                                           |
| Data Handling     | Pandas, NumPy                                    |
| Visualization     | Plotly, Matplotlib                               |
| ML Models         | XGBoost, Scikit-learn                            |
| Evaluation        | AUC, ROC, Cross-Validation, GridSearchCV         |
| Explainability    | SHAP                                             |
| Deployment (Opt.) | Streamlit                                        |

---

## 📊 Visual Explorations

- **📌 Correlation Heatmap**
- **📌 Violin Plot for Transaction Amounts**
- **📌 Distribution Analysis: Fraud vs. Non-Fraud**
- **📌 SHAP Summary and Dependence Plots**

> SHAP enhances understanding by showing **why** a transaction was flagged as fraud.

![SHAP Summary](./assets/shap_summary.png)
![SHAP Force Plot](./assets/shap_force.png)

---

## 🤖 Machine Learning Workflow

1. **Preprocessing**
   - Handling class imbalance with `scale_pos_weight`
   - Feature transformation and outlier handling
   - Winsorization for skewed features

2. **Model Training**
   - XGBoost Classifier (robust to imbalance)
   - GridSearchCV for hyperparameter tuning

3. **Evaluation**
   - AUC-ROC, Confusion Matrix
   - `cross_val_score()` to test generalizability

---

## 🔍 Explainability with SHAP

Used SHAP (SHapley Additive exPlanations) for:
- ✅ **Global feature importance**: Which features influence predictions most
- ✅ **Force plots**: Local explanations for individual cases
- ✅ **Dependence plots**: Visualizing interactions and nonlinear effects

---

## 📦 How to Run the Project

```bash
# Clone the repository
git clone https://github.com/yourusername/credit-card-fraud-shap.git
cd credit-card-fraud-shap

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook project003.ipynb
