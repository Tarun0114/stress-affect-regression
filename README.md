
# 🧠 Stress and Affect Prediction from Biometric Sensor Data


This project applies multiple regression models to predict stress and emotional states using biometric data collected from wearable sensors. It is built upon the **WESAD** dataset and compares model performance based on predictive accuracy and interpretability.

---

## 📌 Project Overview

- **Goal**: Predict stress levels using physiological signals.
- **Target Variable**: Blood Volume Pulse (BVP).
- **Dataset**: WESAD – multimodal data from wrist and chest sensors.
- **Models Used**: Linear, Lasso, Random Forest, XGBoost.

---

## 📂 Dataset

**WESAD (Wearable Stress and Affect Detection)**  
- Source: [UCI Repository](https://archive.ics.uci.edu/dataset/465/wesad+wearable+stress+and+affect+detection)  
- Sensors used:
  - Chest (ECG, EDA, EMG, Respiration, Temp, ACC)
  - Wrist (BVP, EDA, Temp, ACC)

---

## ⚙️ Methodology

1. **Data Preprocessing**
   - Merging multi-sensor data
   - Outlier removal using IQR
   - Feature scaling with `StandardScaler`
   - 80:20 train-test split

2. **Regression Models**
   - `Linear Regression`
   - `Lasso Regression`
   - `Random Forest`
   - `XGBoost`

3. **Evaluation Metrics**
   - 📉 Mean Squared Error (MSE)
   - 📈 R-squared (R²)

---

## 📈 Results Snapshot

| Model              | Train R² | Test R² | Test MSE |
|-------------------|----------|---------|----------|
| Linear Regression | 0.13     | 0.12    | ~267     |
| Lasso Regression  | 0.12     | 0.11    | ~270     |
| Random Forest     | 0.95     | 0.66    | ~103     |
| XGBoost           | 0.70     | 0.48    | ~159     |

✅ **Random Forest** performed best overall, showing robustness and high predictive power.

---

## 📊 Key Insights

- **BVP** is a strong physiological indicator of stress.
- **Ensemble models** (RF, XGBoost) better capture non-linear physiological responses.
- Real-time stress monitoring using wearables is feasible with ML.

---

## 🔒 Ethical Considerations

- Biometric data privacy and GDPR compliance.
- Dataset is anonymized and publicly available for research.

---

## 📁 Project Structure

```
stress-affect-regression/
├── data/                  # Raw WESAD data (downloaded externally)
├── data.csv               # Sample preprocessed data
├── code.py                # Preprocessing + model training code
├── README.md              # Project documentation
```

---

## 🧑‍💻 Author

**Tarun Raj Kumar Jillapogu** – Tarun0114(https://github.com/Tarun0114)


