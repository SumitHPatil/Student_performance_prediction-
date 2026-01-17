# 🎓 Student Performance Prediction

## 📌 Project Overview
This project demonstrates an end-to-end machine learning workflow to analyze and predict student academic performance. The focus is on data preprocessing, exploratory data analysis (EDA), and baseline modeling rather than achieving high predictive accuracy.

The dataset includes demographic, academic, and behavioral features such as study hours, attendance rate, previous grades, parental support, and extracurricular activities.

---

## 📂 Project Structure

```text
student-performance-project/
│
├── data/
│   ├── student_performance_updated_1000.csv
│   └── cleaned_student_data.csv
│
├── pp.py            # Data preprocessing
├── eda.py           # Exploratory Data Analysis
├── model.py         # Baseline model training & evaluation
├── requirements.txt
└── README.md
```


---

## 🧹 Data Preprocessing
- Removed duplicate and non-informative columns  
- Handled missing values:
  - Numerical features → mean imputation  
  - Categorical features → mode imputation  
- Encoded categorical variables  
- Ensured correct data types for numerical features  

The cleaned dataset is saved as `cleaned_student_data.csv` for reproducibility.

---

## 📊 Exploratory Data Analysis (EDA)
Key observations from EDA:
- The dataset contains 1,000 records with no missing values after preprocessing
- Final grades follow an approximately normal distribution
- Previous grades, study hours, and attendance rate show the strongest relationship with final performance
- Categorical features such as parental support and extracurricular activities have moderate impact
- Gender shows minimal influence on final grades

EDA confirms that linear regression is a reasonable baseline modeling choice.

---

## 🤖 Modeling Approach
A **baseline Linear Regression model** was implemented to establish a performance benchmark.

### Evaluation Metrics:
- **Mean Absolute Error (MAE):** 8.03  
- **R² Score:** -0.014  

The low and negative R² score indicates weak predictive relationships between the available features and final grades, highlighting limitations in the dataset rather than issues with model implementation.

---

## 📈 Key Takeaways
- This project emphasizes correct ML workflow over model optimization
- Baseline modeling helps identify data limitations early
- Not all real-world datasets produce strong predictive models
- Transparent reporting of results is critical in data analysis projects

---

## 🔮 Future Improvements
- Reframe the problem as a **Pass/Fail classification task**
- Incorporate additional behavioral or assessment-level features
- Explore model deployment using Streamlit or Flask

---


