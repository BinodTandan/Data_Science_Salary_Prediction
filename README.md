# 💼 Data Scientist Salary Prediction (2024)

This project builds a machine learning pipeline to predict the salary of data scientists based on job descriptions and features extracted from unstructured text (e.g., job summaries) using regular expressions.

---

## 📈 Project Stages

1. **Data Collection**  
   - Source: Kaggle dataset with job listings, summaries, titles, and salaries
2. **Data Preprocessing**  
   - Null handling, type conversion, and categorical encoding
3. **Feature Engineering**  
   - Extracted salary from free-text summaries using **regular expressions**
   - Added binary/ordinal variables for job level, location, remote/hybrid tags
4. **Model Selection**  
   - Random Forest  
   - Decision Tree
5. **Model Validation**  
   - Train/Test split with cross-validation
6. **Evaluation**  
   - Best model: **Random Forest with 78% accuracy**

---

## 🧪 Tools & Libraries

- Python (Pandas, NumPy, Regex)
- Scikit-learn
- Matplotlib & Seaborn
- Jupyter Notebooks

---

## 📊 Key Highlights

- Used **Regex-based pattern extraction** to engineer salary features from unstructured job summaries
- Conducted **advanced EDA** to explore patterns in job titles, location, seniority, and salary bands
- Applied both regression and classification strategies for salary buckets

---

## 🔍 Sample Regex Extraction Snippet

```python
import re
text = "This role offers a salary of $120,000 - $150,000 annually"
salary = re.findall(r"\$[\d,]+", text)
