

---

## Credit Card Fraud Detection (Anomaly Detection)

**Dataset:**

* [Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)
* Contains 284,807 transactions over 2 days, with 492 fraud cases (\~0.172%).
* Features: PCA components V1–V28, `Time`, `Amount`; target: `Class` (0 = legit, 1 = fraud).

**Algorithms Used:**

* **Isolation Forest:** Detects anomalies by isolating points using random splits; effective for rare and different events.
* **Local Outlier Factor (LOF):** Computes local density deviation; points with substantially lower density than neighbors are outliers.
* **One-Class SVM:** Classifies data points as normal or anomaly using an SVM approach for outlier detection.

**Observations:**

* Isolation Forest detected anomalies more effectively (27% of frauds) compared to LOF (2%) and SVM (0%).
* Overall accuracy: Isolation Forest 99.74%, LOF 99.65%, SVM 70.09%.

---
