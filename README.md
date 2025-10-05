# 🧠 Credit Score Prediction

## 📘 Project Overview
This project focuses on building a **machine learning model to predict an individual’s credit score** based on various financial and behavioral features such as income, credit history, outstanding debts, loan behavior, and payment patterns.  

The goal is to analyze the relationship between different customer attributes and their creditworthiness, then classify them into categories like **Good**, **Standard**, or **Poor** credit scores.

This repository contains a detailed **Jupyter Notebook (`Credit_Score_Prediction.ipynb`)** that walks through every stage of the process — from **data cleaning** and **exploratory data analysis (EDA)** to **model training**, **evaluation**, and **interpretation** of results.  

📊 For detailed analysis with **graphs, visualizations, and data tables**, please **open the notebook file** in Jupyter Notebook, JupyterLab, or Google Colab.

---

## 📂 Dataset
The dataset (`Score.csv`) contains customer-level financial data with the following key attributes:
- **Demographic features:** Age, Occupation, Annual Income, Monthly Salary  
- **Financial metrics:** Number of Bank Accounts, Credit Cards, Outstanding Debt, Monthly Balance  
- **Credit behavior:** Number of Delayed Payments, Credit Mix, Payment of Minimum Amount  
- **Target variable:** `Credit_Score` (Good / Standard / Poor)

The dataset was loaded and analyzed for inconsistencies such as missing values, invalid entries, and mixed data types, which were cleaned before analysis.

---

## 🧹 Data Preprocessing
Steps performed include:
1. **Handling missing values** and incorrect data types  
2. **Encoding categorical variables** (e.g., Occupation, Credit Mix)  
3. **Feature scaling** to normalize income and debt-related fields  
4. **Outlier detection** and removal to improve model performance  
5. **Feature selection** based on correlation and importance  

---

## 📊 Exploratory Data Analysis (EDA)
The notebook explores patterns and insights such as:
- Distribution of credit scores among customers  
- Relationship between income, debt, and credit utilization ratio  
- Number of delayed payments vs. credit score  
- Visualizations of age vs. outstanding debt, occupation-based income differences, and more  

🖼️ *All graphs and data tables are available in the notebook.*

---

## 🧠 Model Training
Multiple machine learning models were tested to find the best-performing one for credit score prediction, including:
- **Logistic Regression**  
- **Decision Tree Classifier**  
- **Random Forest Classifier**  
- **XGBoost Classifier**

The dataset was split into training and testing sets, and evaluation was based on accuracy, precision, recall, and F1-score metrics.

---

## 📈 Model Evaluation & Results
After experimentation, the **Random Forest Classifier** (and in some cases XGBoost) achieved the best accuracy, demonstrating strong performance in distinguishing between different credit score categories.

Example performance metrics (illustrative summary):

| Metric | Random Forest | Logistic Regression | Decision Tree |
|:-------|:--------------|:-------------------|:---------------|
| Accuracy | 91.2% | 82.5% | 87.0% |
| Precision | 0.90 | 0.80 | 0.85 |
| Recall | 0.91 | 0.81 | 0.86 |
| F1-Score | 0.90 | 0.80 | 0.85 |

📈 *See the notebook for confusion matrices, feature importance plots, and detailed classification reports.*

---

## 💡 Key Insights
- Customers with **higher income and lower debt** tend to have better credit scores.  
- Frequent **delayed payments** and **high credit utilization ratios** significantly reduce creditworthiness.  
- **Occupation type** and **loan activity** are also strong indicators of credit behavior.  
- The **Random Forest model** effectively captures nonlinear relationships between financial features.

---

## ⚙️ Technologies Used
- **Python**  
- **Pandas, NumPy** – for data processing  
- **Matplotlib, Seaborn** – for data visualization  
- **Scikit-learn** – for model building and evaluation  
- **XGBoost** – for advanced ensemble modeling  
- **Jupyter Notebook / Google Colab** – for code execution and analysis  

---

## ▶️ How to Run
1. Clone this repository:  
   ```bash
   git clone https://github.com/yourusername/Credit_Score_Prediction.git
2. Opent the notebook in Jupyter or Google Colab:
   ```bash
   Credit_Score_Prediction.ipynb
3. Run all cells sequentially to reproduce results.
   (Ensure the dataset file score.csv is in the correct path)
   
