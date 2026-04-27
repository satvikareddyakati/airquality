# 🌫️ Air Quality Analysis & Prediction

## 📌 Overview  
This project focuses on analyzing air quality data to understand how different environmental and sensor-based factors influence pollution levels, particularly **CO (carbon monoxide)**.  

We explored the dataset to uncover patterns over time and built multiple regression models to predict CO levels accurately. The project emphasizes both **data understanding (EDA)** and **model building with proper evaluation**.

---

## 👥 Team Members  

<div align="center">

### **Group 9**

**Satvika Reddy Akati**  
**Tanushri Aenugula**  
**Hasini Kavuru**

</div>

---

## 📂 Dataset  
We used the **UCI Air Quality dataset**, which contains hourly sensor readings of various pollutants and environmental variables.

Some key features include:
- CO(GT) → Target variable  
- NO2(GT), C6H6(GT) → Pollutants  
- Temperature (T), Relative Humidity (RH), Absolute Humidity (AH)  

---

## ⚙️ Project Workflow  

### 1. Data Cleaning & Preprocessing  
- Handled missing values (originally marked as `-200`)  
- Removed unnecessary or empty columns  
- Converted all values into numeric format  
- Combined date and time into a single datetime column  
- Sorted the data chronologically  

---

### 2. Feature Engineering  
To better capture patterns, we created additional features:
- Hour of the day  
- Day of the week  
- Month  

These helped in identifying time-based trends in pollution levels.

---

### 3. Exploratory Data Analysis (EDA)  
We performed detailed analysis to understand the data:
- Visualized pollutant levels over time  
- Checked distributions using histograms and boxplots  
- Built correlation heatmaps to identify relationships  
- Analyzed hourly and daily trends  
- Observed non-linear relationships between variables  

---

## 🤖 Modeling Approach  

### 🔹 Polynomial Regression  
We trained polynomial regression models with varying degrees to capture non-linear patterns in the data.

---

### 🔹 Ridge Regression  
To reduce overfitting in polynomial models, we applied **Ridge regularization**, which improved model stability.

---

### 🔹 Spline Models  
We also implemented spline-based models to allow more flexible curve fitting while maintaining smoothness.

---

### 🔹 Model Selection  
- Used **cross-validation (5-fold)** to compare models  
- Selected the best-performing models based on error metrics  

---

## 📊 Evaluation Metrics  
We evaluated model performance using:
- RMSE (Root Mean Squared Error)  
- MAE (Mean Absolute Error)  
- R² Score  

---

## 📈 Key Insights  
- Pollution levels show strong **time-based patterns**  
- Many relationships in the dataset are **non-linear**  
- Polynomial models can fit well but may overfit  
- Regularization improves model performance  
- Spline models provide a good balance between flexibility and generalization  

---

## 🚀 How to Run  

### 1. Install Dependencies  
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```
### 2. Run the notebook
```bash
jupyter notebook STAT656_Group_9_Code.ipynb
