# 🎓 Student Performance Predictor

This project predicts whether a student is likely to **pass or fail exams before the actual scores are known**, using only demographic and preparation-related factors.  
The goal is to identify at-risk students early, so educators can provide timely support.

---

## 📊 Dataset
- **Source**: [Kaggle - Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)  
- Features used for prediction:
  - Gender  
  - Race/Ethnicity  
  - Parental level of education  
  - Lunch type (standard/free-reduced)  
  - Test preparation course (completed/not completed)  

- Target variable:
  - **Pass/Fail**, calculated from average exam scores (threshold = 60).  
  - Note: Exam scores were **not used as features**, only for defining the target.  

---

## 🛠️ Tech Stack
- **Python**: Pandas, NumPy, Matplotlib, Seaborn  
- **ML**: Scikit-learn (Logistic Regression, Random Forest)  
- **Pipelines**: Preprocessing + Modeling with ColumnTransformer & Pipeline  
- **Model Saving**: Joblib  

---

## 🚀 Workflow
1. **Exploratory Data Analysis (EDA)**  
   - Pass rates by gender, parental education, lunch type, and preparation course  

2. **Feature Engineering**  
   - Derived target (`pass` / `fail`) from average exam scores  

3. **Modeling**  
   - Logistic Regression (baseline)  
   - Random Forest Classifier (better performance)  

4. **Evaluation**  
   - Accuracy, Precision, Recall, F1-score  
   - Confusion Matrix  
   - ROC Curve & AUC  
---

## 📈 Results
- **Random Forest Accuracy**: 71%
