
# 🛒 Kaggle Engage-2: Customer Purchase Prediction

![Kaggle Badge](https://img.shields.io/badge/Kaggle-Competition-blue)
![Python Badge](https://img.shields.io/badge/Python-3.9+-green)
![ML Badge](https://img.shields.io/badge/Machine%20Learning-Regression-orange)

---

## 📌 Overview

This repository contains my solution for the **MLP Project T22025 (Kaggle Engage-2 competition)**.

The task is to **predict a customer’s purchase value** based on their **multi-session behavior** across digital touchpoints. Each data row represents a user session with details such as **browser, traffic source, device attributes, and geographic context**.

The project covers:

* Building the first baseline ML model
* Data preprocessing & feature engineering
* Training advanced ML models (XGBoost, LightGBM, Stacking)
* Generating a submission file in the required format

---

## 🗓️ Timeline

* **Start:** April 23, 2025
* **Close:** July 28, 2025

---

## 📊 Dataset Description

The dataset contains **session-level digital commerce interactions**.

### 🔑 Key Feature Categories:

* **User Behavior & Session Metrics** → `totalHits`, `pageViews`, `sessionNumber`, etc.
* **Device & Technical Attributes** → `deviceType`, `os`, `browser`, `screenSize`, etc.
* **Traffic & Marketing Sources** → `trafficSource`, `campaign`, `referralPath`, etc.
* **Geographical Context** → `city`, `country`, `region`, `continent`, etc.
* **Identifiers** → `userId`, `sessionId`
* **Target Variable** → `purchaseValue` (total session spend in currency units)

📦 **Files included:**

* `train_data.csv`
* `test_data.csv`
* `sample_submission.csv`

---

## 🎯 Evaluation Metric

Submissions are evaluated on **`r2_score()`**:

$$
R^2 = 1 - \frac{\sum (y - \hat{y})^2}{\sum (y - \bar{y})^2}
$$

---

## 📂 Submission Format

The final submission must follow the format:

```
id,purchaseValue
0,0
1,0
2,10990000
4,36500
5,0
...
```

---

## ⚡ How to Run

1. Run the notebook to train models and generate predictions on kaggle.
2. Save predictions in CSV → submit on Kaggle.

---

## 🏆 Project Structure

```
├── notebooks/         # Jupyter notebooks (exploration + modeling)
├── data/              # (Optional) Local copy of dataset
├── outputs/           # Submission files, figures, logs
└── README.md          # Project documentation
```

---

## 📌 License

Data is subject to **Kaggle Competition Rules**.

