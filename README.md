# 💖 GF Mood Predictor

<img width="1919" height="737" alt="Screenshot 2026-01-17 190819" src="https://github.com/user-attachments/assets/61da1c96-0b19-4595-8929-d9f0ea04d3e1" />

<img width="1916" height="738" alt="Screenshot 2026-01-17 190838" src="https://github.com/user-attachments/assets/4312e2b8-12e8-4bf7-b723-ded86823443b" />

A playful yet insightful **Machine Learning project** that predicts a *girlfriend's mood score* (1–10) based on behavioral, emotional, and lifestyle factors. This project blends data science fundamentals with real-life inspired logic and is deployed as an interactive **Streamlit web app**.

> ⚠️ **Disclaimer**: This project uses **synthetic data** and is created purely for educational, experimental, and fun purposes. It does **not** claim to model real human emotions accurately.

---

## 🎯 Objective

To develop a **regression-based Machine Learning model** that predicts a numerical mood score using contextual and behavioral inputs such as sleep, affection, arguments, work pressure, self-care, and more.

---

## 🧠 Project Overview

This project covers the **complete ML lifecycle**:

* Synthetic dataset generation (real-life inspired)
* Feature engineering & preprocessing
* Regression model training and evaluation
* Model interpretation
* Deployment using **Streamlit** for user interaction

The goal is to make ML **interpretable, relatable, and engaging**, while maintaining technical rigor.

---

## 📊 Dataset Description

* **Type**: Synthetic dataset
* **Size**: 1,000 samples
* **Target Variable**: Mood Score (range: **1–10**)
* **Features (10 total)** include:

  * Sleep hours
  * Arguments (none / mild / serious)
  * Expressions of love
  * Compliments
  * Time spent apart
  * Self-care
  * Eating favorite food
  * Work pressure
  * Menstrual cycle phase
  * Other lifestyle indicators

### Dataset Design Logic

* Generated using **domain logic + probability + behavioral weighting**
* Ordinal categories mapped logically (e.g., none < mild < serious)
* Custom weights assigned based on common-sense emotional impact
* Random noise added to simulate **unpredictable emotional variation**
* <3% missing values injected to mimic real-world data imperfections

---

## 🔢 Mood Score Formula (Conceptual)

The mood score is computed using a **weighted sum** of influential features:

* Higher weights for emotionally impactful actions (e.g., expressing love)
* Lower weights for secondary factors (e.g., favorite food)
* Added randomness to reflect emotional complexity

> Example: Even with perfect inputs, mood may fluctuate — just like real life.

---

## ⚙️ Preprocessing & Feature Engineering

* **Missing Values**:

  * Numerical → Mean Imputation
  * Categorical → Mode Imputation

* **Encoding**:

  * Ordinal Encoding for ordered categories

    * `arguments`: none < mild < serious
    * `work_pressure`: no < minor < major
    * `menstrual_phase`: unknown → PMS
  * Binary Encoding for Yes/No features

* **Scaling**:

  * Used **StandardScaler** for normalization

---

## 📈 Exploratory Data Analysis

* Target variable distribution is approximately **normal (bell-shaped)**
* Mean mood score centered around **6–7**, indicating balanced data
* Correlation analysis revealed:

  * Adequate sleep → Improved mood
  * More time apart → Lower mood

---

## 🤖 Model Training

* **Model Used**: Linear Regression
* **Why Linear Regression?**

  * High interpretability
  * Suitable for continuous prediction
  * Clear understanding of feature influence

### Evaluation Metrics

* **Mean Absolute Error (MAE)**: **0.36**
* **R² Score**: **0.87**

### Interpretation

* On average, predictions deviate by only **±0.36 mood points**
* Model explains **87% of mood variability**
* Strong performance for a synthetic, logic-driven dataset

---

## 🚀 Deployment (Streamlit App)

The trained model is deployed using **Streamlit**, providing:

* Interactive questionnaire-style input
* Instant mood score prediction
* Fun, mood-based feedback messages
* User-friendly UI for non-technical users

---

## 🛠️ Tech Stack

* **Python**
* **NumPy & Pandas** – Data handling
* **Scikit-learn** – ML modeling
* **Seaborn & Matplotlib** – Visualization
* **Streamlit** – Web app deployment

---

## 📌 Future Improvements

* Replace synthetic data with anonymized real-world survey data
* Experiment with non-linear models (Random Forest, XGBoost)
* Add NLP-based text emotion inputs
* Improve UI with mood insights & trends

---

## ❤️ Final Note

This project demonstrates how **Machine Learning can be applied creatively** to everyday human-centric problems while still respecting technical correctness and ethical boundaries.

If you enjoyed this project, feel free to ⭐ it and explore further enhancements.

---

**Made with curiosity, logic, and a little love.**
