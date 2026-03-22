# 📊 Employee Data Analysis using Python

## 📌 Project Description
This project focuses on analyzing employee data using Python libraries such as NumPy, Pandas, and Matplotlib. 
The dataset contains information about employees including their ID, name, age, gender, department, salary, and experience.

The goal of this project is to perform data cleaning, exploration, and visualization to extract meaningful insights.

---

## 🛠️ Technologies Used
- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib

---

## 📂 Dataset Information
The dataset includes the following columns:
- EmpID
- Name
- Age
- Gender
- Department
- Salary
- Experience

---

## 🔍 Data Analysis Steps

### 📥 Data Loading
- Imported CSV file using Pandas

### 👀 Data Exploration
- `df.head()` → View first 5 rows  
- `df.tail()` → View last 5 rows  
- `df.info()` → Data types and structure  
- `df.describe()` → Statistical summary  
- `df.shape` → Number of rows and columns  
- `df.columns` → Column names  

---

### 🧹 Data Cleaning
- Checked missing values using:
  - `df.isnull().sum()`
- Handled missing values:
  - `df.fillna(0)`

---

### 📊 Data Selection
- Selected single column:
  - `df["name"]`
- Selected multiple columns:
  - `df[["name", "salary"]]`
- Accessed rows:
  - `df.loc[5]`

---

### 🔎 Filtering Data
- Employees with age greater than 25:
  - `df[df["age"] > 25]`

---

### 📈 Data Aggregation
- Grouped data by department:
  - `df.groupby("department").count()`

---

### ➕ Feature Engineering
- Added new column:
  - `df["exsalary"] = [40000, 50000, 60000, 70000, 40000, 20000]`
- Removed column:
  - `df.drop("exsalary", axis=1)`

---

### 🔃 Sorting
- Sorted data by age:
  - `df.sort_values("age")`

---

## 📊 Data Visualization
- Created charts using Matplotlib
- Visualized:
  - Salary distribution
  - Department-wise employee count
  - Age distribution

---

## 📈 Key Insights
- Identified salary patterns across departments  
- Analyzed age distribution of employees  
- Observed missing data and handled it  
- Compared employee counts by department  

---

## 🚀 How to Run the Project
1. Install required libraries:
   ```bash
   pip install numpy pandas matplotlib
