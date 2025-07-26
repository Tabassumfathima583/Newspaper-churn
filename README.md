# 📰 Newspaper Churn Prediction

A machine learning project to predict whether a newspaper customer will churn, based on demographic and behavioral data. This end-to-end solution covers data cleaning, feature engineering, model training, evaluation, and insightful visualizations.

---

## 📁 Dataset

- **Source**: [Kaggle – Newspaper Churn](https://www.kaggle.com/datasets/leiyiting01/newspaper-churn)
- **Records**: 15,855  
- **Target Variable**: `Subscriber` (`YES` → 1, `NO` → 0)

---

## 🧼 Data Preprocessing

- Handled null values (`Language`, `Age range`, `weekly fee`)
- Cleaned and encoded categorical features
- Converted income, fee, and age ranges into numeric bins
- Standardized and split data into training and test sets

---

## 📊 Exploratory Data Analysis

### 📌 Churn Distribution  
Shows class imbalance between churned and retained subscribers.

![Churn Distribution](https://github.com/Tabassumfathima583/Newspaper-churn/blob/main/Images/Churn%20Distribution.png)

---

### 📌 Correlation Heatmap  
Visual representation of numerical feature relationships.

![Correlation Heatmap](https://github.com/Tabassumfathima583/Newspaper-churn/blob/main/Images/Correlation%20heatmap.png)

---

## 🤖 Model Building & Comparison

Three models were trained:

| Model                | Accuracy |
|---------------------|----------|
| Logistic Regression | 81.68%   |
| Random Forest       | 84.48%   |
| **XGBoost**         | **84.83% ✅** |

---

## ✅ Final Model: XGBoost

### 🧠 Top 10 Features  
Features that contributed most to predictions.

![Top 10 Features](https://github.com/Tabassumfathima583/Newspaper-churn/blob/main/Images/Top%2010%20features(XGBoost).png)

---

### 📈 Evaluation Metrics  
Detailed precision, recall, and F1-score for each class.

![Evaluation Metrics](https://github.com/Tabassumfathima583/Newspaper-churn/blob/main/Images/Evaluation%20metrics.png)

---

## 🖼️ Project Poster  
A visual summary of the project in one slide.

![Poster](https://github.com/Tabassumfathima583/Newspaper-churn/blob/main/Images/poster.png)

---

## 📌 Conclusion

- **XGBoost** was the most accurate and stable model
- Feature importance insights help interpret model behavior
- Imbalanced class performance could be improved using SMOTE or class weights

---

## 🚀 Future Work

- Try advanced techniques for imbalance (SMOTE, Ensemble tuning)  
- Deploy model via Streamlit/Flask for user prediction  
- Add SHAP/ELI5 explainability for transparency  

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

