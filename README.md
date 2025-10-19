# 🪨 Lithofacies Prediction Pipeline from Well Log Data

## 📌 Overview  
This project implements a **machine learning pipeline** for **lithofacies prediction** using **well log data**.  
It integrates **data preprocessing**, **exploratory analysis**, and a **two-stage classification model** to accurately predict lithofacies from geophysical inputs.  
The workflow is documented both in a **Jupyter Notebook** and a **technical report** that provides in-depth analysis and results interpretation.


## 🚀 Features  
✅ Automated data cleaning and preprocessing  
✅ Stability-based filtering for robust data selection  
✅ XGBoost-driven missing value imputation  
✅ Comprehensive feature engineering and anomaly detection  
✅ Two-stage classification pipeline (Binary → Multi-Class)  
✅ Comparative analysis of ML strategies  
✅ Detailed visualizations and performance evaluation  


## 📦 Requirements  
- pandas  
- numpy  
- scikit-learn  
- xgboost  
- catboost  
- matplotlib  
- seaborn  


## 📂 Project Structure  
```
├── Data/
│ └── train.csv
├── Code/
│ └── Startegies.ipynb
│ └── Challenge_V1.ipynb
│ ── Challenge_V2.ipnb
├── Reports/
│ └── Final_Report.pdf
│ └── Strategies_Report.pdf
└── README.md
```


## 🔧 Installation  

### **Clone the repository:**  
```
git clone https://github.com/your-repo/lithofacies-prediction.git
cd lithofacies-prediction
```

### **Install dependencies:**
```
pip install -r requirements.txt

```
## 📊 Usage

### 🧹 Data Preprocessing
Run the preprocessing cells in the notebook:
- ✔ Load raw well log data
- ✔ Clean and filter unstable records
- ✔ Handle missing values using XGBoost-based imputation
- ✔ Generate stability and feature summaries

### 📈 Exploratory Data Analysis (EDA)
- ✔ Visualize log distributions and correlations
- ✔ Identify unstable zones and anomalies
- ✔ Extract geophysical feature patterns

#### 🧠 Two-Stage Classification Model
- Stage 1: Binary Classification (XGBoost) -> Task: Shale (1) vs Non-Shale (0)
- Stage 2: Multi-Class Classification (CatBoost) -> Task: Predict lithofacies for Non-Shale samples

## 🔍 Model Evaluation
- ✔ Compute classification metrics (Weighted F1-score)
- ✔ Generate confusion matrices and ROC Curves
- ✔ Compare performance across models and configurations

## 🧩 Methodology Summary
The pipeline follows a structured 9-step workflow:
- Data Loading & Cleaning
- Exploratory Data Analysis (EDA)
- Stability Filtering
- Train/Test Split
- XGBoost Imputation
- Feature Engineering
- Anomaly Detection
- Model Training (Two-Stage)
- Evaluation & Validation

For detailed methodology evolution and comparisons, refer to:

📖 Section 1.3 — “Methodology Evolution and Strategy Comparison” in Strategies_Report.pdf.

## 📊 Results
Key outcomes from the final workflow include:
- ✔ Accurate lithofacies classification with improved shale detection
- ✔ Robust handling of unstable and missing data
- ✔ Enhanced interpretability through feature importance visualization
- ✔ High reproducibility with structured, modular code

## 🤝 Contributing
1. **Fork the repository**
2. **Create your feature branch** (`git checkout -b feature-branch`)
3. **Commit your changes** (`git commit -m 'Add new feature'`)
4. **Push to the branch** (`git push origin feature-branch`)
5. **Submit a pull request** 🎉  

## 🙌 Acknowledgments
Data provided as part of my SLB Internship Challenge (or at Force-2020-Machine-Learning-competition: https://github.com/bolgebrygg/Force-2020-Machine-Learning-competition)

Special thanks to contributors and reviewers involved in the lithofacies analysis and interpretation.

## 📘 About
Machine learning-based lithofacies prediction pipeline leveraging XGBoost and CatBoost, with a focus on data quality, geological interpretability, and model robustness.
