# 🏭 Predicting Manufacturing Defects

This project is a mini data science case study using a real-world manufacturing dataset to predict product defects based on various production parameters. It's designed as a hands-on demonstration of the typical machine learning pipeline — from data exploration to model evaluation.

---

## 📊 Dataset

The dataset used in this project was sourced from Kaggle ([here](https://www.kaggle.com/datasets/rabieelkharoua/predicting-manufacturing-defects-dataset?resource=download)) and includes features such as:

- `ProductionVolume`
- `ProductionCost`
- `EnergyConsumption`
- `DefectRate`
- Target: `DefectStatus` (0 = No Defect, 1 = Defective)

The dataset reflects an **imbalanced classification problem**, which adds to the real-world complexity.

---

## Project Steps

### 1. Data Loading & Cleaning
- Read and inspect the dataset
- Check for missing values
- Understand feature types

### 2. Exploratory Data Analysis (EDA)
- Class distribution visualization
- Correlation matrix heatmap
- Feature distribution plots

### 3. Data Preprocessing
- Train/test split
- Feature scaling using `StandardScaler`

### 4. Model Training
- Used `RandomForestClassifier` with `class_weight='balanced'` to handle imbalance

### 5. Model Evaluation
- Classification Report
- Confusion Matrix
- ROC Curve and AUC Score

---

## 📷 Results

Classification Report:
```
               precision    recall  f1-score   support

           0       0.93      0.77      0.84       102
           1       0.96      0.99      0.97       546

    accuracy                           0.96       648
   macro avg       0.94      0.88      0.91       648
weighted avg       0.95      0.96      0.95       648

Confusion Matrix:
 [[ 79  23]
 [  6 540]]

 ```

### 📈 Defect Status Distribution
![image](https://github.com/user-attachments/assets/f6bc9bb1-2891-4cae-a315-7dbd3b33a7f4)

### 🔥 Correlation Heatmap
![image](https://github.com/user-attachments/assets/2836837c-ec15-4688-8159-b859bf704f96)

### 🎯 Model Evaluation
![image](https://github.com/user-attachments/assets/d10c64ca-5811-40dc-bf01-09f68fe246c0)

