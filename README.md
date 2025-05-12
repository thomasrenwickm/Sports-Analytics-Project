# 📊 Predicting Injury Risk in Elite Football

*Using Integrated GPS, Recovery, and Physical Performance Data*

## 📘 Overview

This project aims to predict the probability of injury in elite football players based on daily workload, recovery, and physical capability data. It was developed as part of a Sports Analytics elective for the Master in Data Science program at IE University.

By integrating datasets from the Chelsea FC Performance Insights Vizathon, this study leverages player movement (GPS), recovery metrics, and physical testing data to create a machine learning model capable of flagging elevated injury risk. Our ultimate goal is to build a scalable and interpretable framework that can support proactive player health management and training decisions.

---

## 🎯 Project Objective

To build and evaluate a supervised machine learning model that can predict whether a player is at risk of injury on a given day using historical and session-level performance data.

---

## 📂 Datasets Used

The project uses simulated yet realistic datasets provided publicly by Chelsea FC’s Performance Insights Team:

* `GPS Data.csv`: Daily movement and load metrics (e.g., total distance, high-speed running, acceleration counts).
* `Recovery Status Data.csv`: Aggregated scores across sleep, soreness, subjective recovery, and biomarkers.
* `Physical Capability Data.csv`: Strength, sprint, jump, and movement capacity metrics.

📌 **Data Source:**
[Performance Insights Vizathon Homepage](https://chelsea-fc-performance-insights.github.io/Competition/#data)
[GitHub Repository](https://github.com/Chelsea-Fc-Performance-Insights/Competition)

---

## 🛠️ Methodology

### 🔧 Data Processing

* Merged datasets using date as the primary key.
* Converted and standardized all time-based and categorical features.
* Simulated injury labels based on changes in workload and recovery to support supervised learning.
* Addressed class imbalance using methods such as SMOTE and class weighting.

### 📈 Modeling

* **Baseline Model:** Logistic Regression
* **Advanced Models:** Random Forest and XGBoost
* **Validation Strategy:** Time-based splitting to avoid data leakage

### 🧪 Evaluation Metrics

* Precision, Recall, F1 Score
* AUC-ROC

---

## 🚀 Deliverables

* A trained machine learning model capable of predicting injury likelihood.
* A Streamlit web app that allows users to:

  * Input session data manually or via CSV
  * View model predictions for injury risk
* A reproducible codebase for sports analytics teams or students

---

## 📌 Limitations

* The dataset represents only a single (synthetic) player.
* Injury labels are simulated based on performance indicators.
* Future work would involve validation on multi-player, real-world datasets.

---

## 👥 Team Members

* Santiago Botero
* Sebastián de Wind
* Thomas Arturo Renwick Morales
* Santiago Ruiz

---

## 📄 License & Acknowledgments

This project is based on data provided by the **Chelsea FC Performance Insights Vizathon** and is used strictly for academic and non-commercial purposes. All data remains the property of its original creators.
