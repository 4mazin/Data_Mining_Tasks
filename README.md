# 🧠 Data Mining Tasks

This repository contains two machine learning tasks built using Scikit-learn:

- **📈 Regression Task** – Predicting sales based on advertisement spending
- **🧪 Classification Task** – Predicting customer car-buying decisions using K-Nearest Neighbors (KNN)

Each notebook includes complete data preparation, handling of missing values, modeling, evaluation, and interpretation.

---

## 🔨 Task 1: Sales Prediction (Linear Regression)

### 🎯 Objective:
Predict the `Sales` value based on advertisement spending on **TV**, **Radio**, and **Newspaper**.

### 📊 Dataset Features:
- `TV`: TV advertisement budget
- `Radio`: Radio advertisement budget
- `Newspaper`: Newspaper advertisement budget
- `Sales`: Product sales (target)

### ⚙️ Steps:
- Removed duplicates
- Filled missing values using **mean imputation**
- Split data into training/test sets
- Built and trained a **Linear Regression** model

### 📐 Evaluation Metrics:
- **R² Score**: Measures prediction accuracy
- **Mean Error**: Mean difference between predicted and actual sales
- **Mean Squared Error (MSE)**


---

## 🔍 Task 2: Car Buyer Decision (KNN Classification)

### 🎯 Objective:
Choose the best `Decision` (e.g. `unacc`, `acc`, `vgood`, `good`) that a customer makes about buying a car based on vehicle features.

### 📊 Dataset Features:
- `buying_price`
- `maitenance_cost`
- `num_of_doors`
- `num_of_persons`
- `lug_boot`
- `safety`
- `Decision` (target)

### ⚙️ Preprocessing:
- Handled missing values using **mode** for categorical and **mean** for numeric features
- Normalized categorical labels using `LabelEncoder`
- Converted special text labels like `'5more'`, `'more'` into numeric
- Balanced imbalanced classes using **oversampling**

### 🤖 Model:
- **K-Nearest Neighbors (KNN)** classifier
- Trained on a balanced dataset for improved accuracy

### 📐 Evaluation:
- Used bar plot to confirm class balancing
- Suitable for multi-class classification tasks
