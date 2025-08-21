# Garment Employee Productivity Predictor 🏭

A machine learning project that predicts garment factory worker productivity using **Random Forest regression**, achieving **83% R² accuracy**.

---

## 📋 Project Overview

This project analyzes and predicts the productivity of garment factory employees using various operational and environmental factors. The model helps manufacturing managers understand key drivers of productivity and make data-driven decisions to optimize workforce performance.

---

## 🎯 Key Results

- **Model Performance:** 83% R² score on test data  
- **Primary Predictors:** Incentives (75% importance) and Targeted Productivity (13% importance)  
- **Data Processing:** Handled 1,197 records with comprehensive feature engineering  
- **Missing Data:** Successfully addressed 42% missing values in WIP (Work in Progress) feature  

---

## 📊 Dataset

The dataset comes from the **UCI Machine Learning Repository** and contains productivity data from garment manufacturing teams, including:

- **Temporal Features:** Date, Day of Week, Quarter  
- **Team Metrics:** Team number, Number of workers, Department  
- **Production Factors:** Standard Minute Value (SMV), Work in Progress (WIP), Style changes  
- **Performance Indicators:** Targeted vs Actual productivity, Overtime, Incentives  
- **Operational Metrics:** Idle time, Idle workers  

---

## 🔧 Technologies Used

- **Python 3.x**  
- **Pandas** - Data manipulation and analysis  
- **Scikit-learn** - Machine learning algorithms  
- **Matplotlib / Seaborn** - Data visualization  
- **NumPy** - Numerical computing  

---

## 📈 Model Development Process

### 1. Exploratory Data Analysis (EDA)
- Identified data quality issues (missing values, inconsistent categories)  
- Analyzed feature distributions and correlations  
- Discovered key insights about factory operations  

### 2. Data Preprocessing
- **Feature Engineering:** Created binary WIP indicator, cleaned department categories  
- **Data Cleaning:** Standardized quarter categories, handled missing values  
- **Scaling:** Applied MinMax scaling for consistent feature ranges  
- **Encoding:** One-hot encoded categorical variables  

### 3. Model Selection & Tuning
- **Initial Models:** Decision Tree (25% R²)  
- **Hyperparameter Tuning:** GridSearchCV optimization  
- **Feature Selection:** Identified top contributing features  
- **Final Model:** Random Forest with optimized parameters  

### 4. Key Findings
- Incentives are the strongest predictor (75% feature importance)  
- Targeted Productivity significantly influences actual performance  
- Missing WIP data indicated different operational patterns  
- Day of week and department had minimal impact  

---


## 📊 Model Performance
Model	R² Score	Key Features
Decision Tree (Basic)	25.9%	Simple depth-limited tree
Decision Tree (Tuned)	39.5%	GridSearch optimized
Random Forest (Final)	83.0%	Ensemble with feature selection

---

## 💡 Business Insights

Incentive Programs: Financial incentives are the most critical factor for productivity
Target Setting: Realistic productivity targets significantly impact performance
Data Quality: Missing operational data may indicate systemic issues
Operational Focus: Standard processes (SMV, overtime) matter more than temporal factors

---

## 🔮 Future Enhancements

Implement classification model for productivity categories
Add more sophisticated feature engineering techniques
Integrate real-time prediction capabilities
Expand dataset with additional operational variables
Develop automated model retraining pipeline

---

## 📝 Model Limitations

Dataset limited to first quarter of 2015
44% data reduction when handling missing values optimally
Model assumes consistent operational conditions
Limited external factors (market conditions, seasonal effects)
