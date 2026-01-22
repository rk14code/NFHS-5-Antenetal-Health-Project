# NFHS-5-Antenetal-Health-Project
# Socioeconomic Determinants of Antenatal Care Utilization in India: An NFHS-Based Analysis

![License](https://img.shields.io/badge/Status-Completed-brightgreen)

This project investigates the **socioeconomic factors influencing antenatal care (ANC) utilization** among women in India using data from the **National Family Health Survey (NFHS-5)**. The analysis involves data preprocessing, exploratory data analysis, machine learning modeling, and policy insights.

## 📌 Objective

To identify and quantify the **key socioeconomic and demographic determinants** affecting the likelihood of Indian women receiving adequate antenatal care (at least 4 visits as per WHO guidelines).

---

## 📂 Dataset

- **Source**: [NFHS-5 (2019-21)](https://mohfw.gov.in/sites/default/files/NFHS-5_Phase-II_0.pdf)
- **Target Group**: Women aged 15–49 who gave birth in the last 5 years.
- **Sample Size**: 172,702 respondents after cleaning.

---

## 🧹 Data Preprocessing

- **Missing values**: Handled with median/mode imputation and logical replacement.
- **Outlier Treatment**: Z-score, IQR, and capping applied.
- **Encoding**:
  - Ordinal: Label Encoding (e.g., education, wealth index)
  - Nominal: One-Hot Encoding (e.g., religion, caste, region)
- **Scaling**: Standardization (Z-score)
- **Class Imbalance**: Addressed using SMOTE
- **Feature Selection**: Based on correlation, domain knowledge

---

## 📊 Exploratory Data Analysis (EDA)

- Summary statistics for key variables
- Histograms and bar plots for:
  - ANC usage
  - Education level, Wealth index, Residence type
  - Religion, Caste, Region
- Correlation matrix visualization
- Box plots and distribution charts

---

## 🤖 Models Used

| Model               | Description                                                      |
|--------------------|------------------------------------------------------------------|
| **Logistic Regression** | Interpretable baseline model for binary classification        |
| **Support Vector Machine (SVM)** | Non-linear classification with kernel trick                |

---

## 📈 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Confusion Matrix

**Model Performance Highlights**:

| Metric        | Logistic Regression | SVM        |
|---------------|---------------------|------------|
| Accuracy      | 83.4%               | **87.1%**  |
| Precision     | 14.5%               | **17.0%**  |
| Recall        | **51.1%**           | 43.9%      |
| F1 Score      | 22.6%               | **24.5%**  |
| AUC Score     | 0.77                | 0.76       |

---

## 🔍 Feature Importance

- **Top Predictors**: Region > Religion > Caste > Residence > Age
- Regional disparities dominate ANC utilization. Women in Nagaland, Bihar, and UP were significantly more likely to **miss ANC visits**.

---

## 📌 Key Findings

- **Education** and **wealth** significantly improve ANC utilization.
- **Rural women** and those from disadvantaged **caste/religion groups** face access barriers.
- **Region** emerged as the strongest determinant.

---

## 📚 References

1. [NFHS-5 Report (GoI)](https://mohfw.gov.in/sites/default/files/NFHS-5_Phase-II_0.pdf)  
2. [WHO ANC Recommendations](https://www.who.int/publications/i/item/9789241549912)  
3. [BMC Pregnancy and Childbirth (2023)](https://link.springer.com/article/10.1186/s12884-023-06117-z)  
4. [Plos One Study (2021)](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0247935)  

---

