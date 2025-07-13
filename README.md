# ☕ How Caffeine Affects Sleep and Focus: A Data-Driven Investigation

**Can your morning coffee cost you a good night’s sleep?**  
This project analyzes real-world data to explore how caffeine consumption—by amount, beverage type, time of day, and user demographics—impacts sleep quality and cognitive focus.

---

## 📌 Project Overview

- **Dataset:** Caffeine Intake Tracker (caffeine_intake_tracker.csv)
- **Goal:**  
  1. Explore how caffeine use affects sleep and focus  
  2. Build a predictive model to estimate whether someone’s sleep is impacted by caffeine

---

## 📁 Repository Structure

📦caffeine-sleep-focus-analysis
┣ 📊 EDA_Plots/ # Visualizations from EDA
┣ 📈 model_outputs/ # Model artifacts (confusion matrix, ROC curve, etc.)
┣ 📄 Caffeine_Analysis.ipynb # Main notebook with full analysis
┣ 📄 caffeine_intake_tracker.csv # Cleaned dataset used in the project
┗ 📄 README.md 

---

## 🛠️ Tools & Technologies

- Python (3.x)  
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

## 🔍 Key Findings from EDA

- Coffee is the most consumed caffeine source, followed by tea and energy drinks  
- Sleep quality and focus scores are generally high in the sample  
- Strong negative correlation between caffeine intake and sleep quality  
- Slight positive correlation between caffeine and focus—especially during morning hours  
- Balanced demographics by gender and time of caffeine consumption

---

## 🤖 Predictive Modeling

We built a **Logistic Regression** model to predict the binary target: `sleep_impacted`.

### 🎯 Features Used:
- `caffeine_mg`, `age`, `focus_level`, `sleep_quality`  
- Binary indicators for beverage types, time of day, and gender  

### 📊 Model Performance:
- **Accuracy:** 90%  
- **Top Predictors:** `sleep_quality`, `focus_level`, `caffeine_mg`  
- **Evaluation Metrics:** Confusion Matrix, ROC Curve, Permutation Feature Importance  

---

## ✅ Conclusion

This project confirms that caffeine—especially when combined with behavioral and demographic factors—can significantly influence sleep outcomes. The high accuracy of the logistic regression model highlights how even simple models can yield meaningful insights.

---

## 🚀 Future Enhancements

- Explore advanced models: Random Forest, XGBoost 
