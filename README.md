# 📰 Newspaper Churn Prediction

A machine learning project to predict whether a newspaper subscriber will churn based on demographic and subscription data.

---

## 📁 Dataset

- **Source**: [Kaggle - Newspaper Churn Dataset](https://www.kaggle.com/datasets/leiyiting01/newspaper-churn)
- **Rows**: 15,855
- **Features**: Income, Age, Weekly Fee, Ethnicity, Subscription Info, etc.

---

## 🔧 Process

1. **Data Cleaning**
   - Converted income ranges to numeric midpoints
   - Encoded categorical features
   - Handled missing values
   - Removed address-level columns (e.g., Address, City)

2. **EDA**
   - Visualized class balance
   - Correlation heatmap
   - Feature importances

3. **Modeling**
   - Logistic Regression, Random Forest, and XGBoost
   - **XGBoost** performed best:
     - **Accuracy**: 84.83%
     - **F1-score (churn class)**: 0.53

4. **Feature Importance**
   - Top features: Weekly Fee, Age, Home Ownership, etc.

---

## 🔍 Sample Output

📊 XGBoost Feature Importances  
![Feature Importance](plots/feature_importance.png)

📈 Correlation Heatmap  
![Heatmap](plots/heatmap.png)

---

## 📦 Requirements

```bash
pandas
matplotlib
seaborn
xgboost
scikit-learn

git clone https://github.com/your-username/Newspaper-Churn-Prediction.git
cd Newspaper-Churn-Prediction
pip install -r requirements.txt

