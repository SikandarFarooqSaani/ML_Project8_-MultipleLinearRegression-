# 🎓 Student Performance Prediction using Multiple Linear Regression  

This project applies **Multiple Linear Regression (MLR)** on a **student performance dataset** from Kaggle.  
The goal was to predict student performance based on multiple input features, while validating the results using both **Scikit-Learn** and a **custom MLR implementation** (coded from scratch).  

📂 Dataset Link: [Student Performance Dataset](https://www.kaggle.com/datasets/nikhil7280/student-performance-multiple-linear-regression)  

---

## 🚀 Project Steps  

### 1. Importing Libraries  
- **NumPy, Pandas** → Data handling  
- **Matplotlib, Seaborn** → Visualization  
- **Scikit-Learn (train_test_split, LinearRegression, r2_score)** → Model building and evaluation  
- **os, kagglehub** → Dataset access  

### 2. Loading & Cleaning the Data  
- Loaded dataset and checked the structure.  
- **Null values:** None found.  
- **Duplicates:** 127 duplicates removed → dataset reduced from **10,000 to 9,873 rows**.  
- **Columns:** 6 total.  

### 3. Handling Categorical Data  
- Found one column with categorical values (object dtype).  
- Mapped categories to **0 and 1**.  
- Converted the column into integer type for model training.  

### 4. Splitting the Data  
- Divided dataset into **X (features)** and **y (target)**.  
- Applied **train-test split (80:20)**.  

### 5. Training with Scikit-Learn  
- Created a **LinearRegression** object and fitted it.  
- Results:  
  - **R² Score:** `0.98`  
  - **Adjusted R² Score:** `0.98`  
  - **Intercept:** `-34`  

### 6. Training with Custom MLR (From Scratch)  
- Reused the **custom linear regression class** coded with the **Normal Equation**.  
- Trained and tested with the same data.  
- Results were **identical to Scikit-Learn** (R², coefficients, intercept).  
- ✅ This validated that our implementation works as expected.  

---

## 📈 Results  

- **R² Score:** `0.98`  
- **Adjusted R² Score:** `0.98`  
- **Intercept:** `-34`  
- Model explains **98% of the variance** in student performance.  
- Both **Scikit-Learn and custom model matched perfectly**.  

---

## 🛠️ Tech Stack  

- **Python**  
- **NumPy, Pandas**  
- **Matplotlib, Seaborn**  
- **Scikit-Learn**  

---

## 📌 Conclusion  

This project showed how to:  
- Clean a dataset (handle duplicates and categorical values).  
- Train a multiple linear regression model with both **Scikit-Learn** and **custom implementation**.  
- Achieve a very high **R² score of 0.98**, showing the dataset has strong linear relationships.  

📓 Full implementation and code are included in the **Jupyter Notebook** provided in this repository.  

---
