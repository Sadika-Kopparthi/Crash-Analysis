# 🚗 Injury Severity Prediction in Vehicle Crashes (CRSS Dataset)

This project was developed as part of the *MSIS 5633 – Predictive Analytics Technologies* course at Oklahoma State University. Our goal was to build a predictive classification model that determines whether a crash injury is *Minor* or *Major* using real-world crash data from the *Crash Report Sampling System (CRSS), published by the **National Highway Traffic Safety Administration (NHTSA)*.

---

## 🎯 Objective

To leverage supervised machine learning models and CRISP-DM methodology to predict injury severity outcomes, enabling traffic safety officials and policy makers to take data-driven action for safer roads.

---

## 🧪 Data Workflow

- 💾 *Data Source*: CRSS (NHTSA) — 4 tables: Accident, Vehicle, Person, Distraction
- 🧹 *Data Cleaning*: Removed missing/placeholder values from 23,000+ records
- 🧠 *Feature Engineering*: Created 28 variables including:
  - Crash Time Category
  - Driver Ejection Status
  - Use of Restraints
  - Alcohol/Drug Involvement
  - Light & Weather Conditions
  - OverSpeed and Visibility indicators
- ⚖️ *Balancing: Used **Equal Size Sampling* to handle class imbalance
- 🔄 *Platform: Entire workflow implemented in **KNIME Analytics Platform*
- 🔁 *Methodology: Followed the **CRISP-DM* process

---

## 🤖 Models Built and Evaluated

We trained and evaluated six classification models using identical sampling and preprocessing:

- Logistic Regression  
- Decision Tree  
- Gradient Boosted Trees (GBT)  
- Random Forest  
- K-Nearest Neighbors (KNN)  
- Multi-Layer Perceptron (MLP)

---

## 📊 Evaluation Metrics

Each model was evaluated based on:
- *Accuracy*
- *Sensitivity* (True Positive Rate)
- *Specificity* (True Negative Rate)
- *AUC* (Area Under ROC Curve)

| Model                | Accuracy | Sensitivity | Specificity | AUC   |
|---------------------|----------|-------------|-------------|-------|
| Logistic Regression | 72.7%    | 68.5%       | 73.7%       | 0.783 |
| Decision Tree       | 62.9%    | 61.2%       | 63.3%       | 0.630 |
| GBT                 | 72.6%    | 70.2%       | 73.1%       | 0.791 |
| Random Forest       | 73.5%    | 65.9%       | 75.3%       | 0.780 |
| KNN                 | 59.4%    | 60.3%       | 59.1%       | 0.633 |
| MLP                 | 71.3%    | 68.6%       | 72.0%       | 0.775 |

---

## 🔍 Insights

- *Gradient Boosted Trees* and *Random Forest* were top performers based on AUC and overall accuracy
- *Logistic Regression* provided a strong interpretable baseline
- The use of engineered variables significantly improved prediction quality

---

## 📚 Tools & Technologies

- 🧩 *KNIME Analytics Platform*
- 🐍 Python (for validation and analysis)
- 📈 CRISP-DM Methodology
- 📊 NHTSA’s CRSS Dataset 

---

## ✅ Conclusion

This project highlights the impact of *predictive and prescriptive analytics* in real-world scenarios like traffic safety. By understanding what leads to severe crash injuries, authorities can proactively design safer infrastructure, interventions, and response strategies.
