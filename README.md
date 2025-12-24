# 📞 Telco Customer Churn Classification

A machine learning project to predict customer churn in a telecommunications company using classification algorithms.

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![ML](https://img.shields.io/badge/ML-Classification-green)
![Status](https://img.shields.io/badge/Status-Complete-success)

## 🎯 Objective

Predict whether a telecom customer will **churn** (leave the service) based on:
- Demographics
- Subscription details
- Service usage patterns
- Billing information

## 📊 Dataset

The Telco Customer Churn dataset contains customer information including:

| Category | Features |
|----------|----------|
| **Demographics** | Gender, SeniorCitizen, Partner, Dependents |
| **Services** | PhoneService, InternetService, OnlineSecurity, etc. |
| **Account** | Contract, PaymentMethod, MonthlyCharges, TotalCharges |
| **Target** | Churn (Yes/No) |

## 🔄 Project Pipeline

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│  Data Loading   │───►│       EDA       │───►│  Preprocessing  │
└─────────────────┘    └─────────────────┘    └─────────────────┘
                                                      │
                                                      ▼
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Evaluation    │◄───│  Model Training │◄───│ Feature Eng.    │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

## 🛠️ Techniques Used

### Data Preprocessing
- Missing value imputation
- Duplicate removal
- Outlier detection (IQR method)
- Feature encoding (Label Encoding)

### Feature Engineering
- Feature scaling (StandardScaler)
- Class imbalance handling (if applicable)

### Models Implemented
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)

### Evaluation Metrics
- Accuracy
- Precision, Recall, F1-Score
- Confusion Matrix
- ROC-AUC Curve

## 📁 Project Structure

```
telco-churn-classification/
├── README.md
├── requirements.txt
├── notebooks/
│   └── telco_churn_classification.ipynb
├── data/
│   └── .gitkeep (add your data here)
└── src/
    └── utils.py (helper functions)
```

## 🚀 Getting Started

### Prerequisites

```bash
pip install -r requirements.txt
```

### Required Libraries

```
pandas
numpy
scikit-learn
matplotlib
seaborn
```

### Usage

1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/telco-churn-classification.git
cd telco-churn-classification
```

2. Add your dataset to `data/` folder

3. Open and run the Jupyter notebook
```bash
jupyter notebook notebooks/telco_churn_classification.ipynb
```



## 🔑 Key Insights

1. **Contract Type**: Month-to-month contracts have higher churn rates
2. **Tenure**: New customers are more likely to churn
3. **Payment Method**: Electronic check users show higher churn
4. **Services**: Customers without online security/backup churn more

## 📚 Learning Outcomes

This project demonstrates:
- Binary classification problem solving
- Handling imbalanced datasets
- Feature importance analysis
- Model comparison and selection
- Business metric interpretation

## 👨‍💻 Author

**Mohammed (Joox)**
- IoT & AI Developer @ VoltX
- CS Student @ Helwan University 



---

⭐ Star this repo if you find it useful!
