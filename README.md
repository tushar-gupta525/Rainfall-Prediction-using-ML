# Rainfall-Prediction-using-ML
Machine learning–based rainfall prediction using weather data. Includes data cleaning, exploratory data analysis, feature selection, class balancing via down sampling, and a Random Forest classifier to predict rainfall occurrence (Yes/No).

---

## 📂 Dataset
- File: `Rainfall.csv`
- Records: 366
- Target Variable: `rainfall` (Yes / No)

### Features
- Pressure  
- Maximum Temperature  
- Temperature  
- Minimum Temperature  
- Dew Point  
- Humidity  
- Cloud Cover  
- Sunshine  
- Wind Direction  
- Wind Speed  

---

## 🛠️ Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## 🔍 Exploratory Data Analysis
- Distribution plots for numerical features  
- Boxplots for outlier detection  
- Correlation heatmap  
- Rainfall class distribution analysis  

EDA helped identify feature relationships and data imbalance.

---

## ⚙️ Data Preprocessing
- Removed non-informative column (`day`)
- Handled missing values:
  - Wind direction → mode
  - Wind speed → median
- Encoded target variable (`yes → 1`, `no → 0`)
- Manual feature reduction based on correlation

---

## ⚖️ Class Imbalance Handling
The dataset was imbalanced, so **random downsampling** of the majority class was applied to balance the data before training.

---

## 🤖 Machine Learning Model
### Random Forest Classifier
- Handles non-linear relationships
- Robust to noise and outliers
- Suitable for tabular weather data

---

## 📊 Model Evaluation
- Accuracy Score  
- Confusion Matrix  
- Classification Report  

---

## ✅ Conclusion
This project provides a solid baseline for rainfall prediction using classical machine learning techniques and establishes a foundation for further accuracy improvements.

---

## 🚀 Future Improvements
- SMOTE for better class balancing  
- Hyperparameter tuning  
- Cyclic encoding for wind direction  
- Advanced models like XGBoost or LightGBM  
