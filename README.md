# Data Preprocessing Lab 4

## 📌 Project Overview

This project focuses on applying essential data preprocessing techniques on a dataset of student performance. The goal is to prepare the data for machine learning by improving its quality and structure.

---

## 📊 Dataset

The dataset used is **Students Performance Dataset**, which includes:

* Math scores
* Reading scores
* Writing scores
* Additional categorical features

Only numerical features were used for preprocessing and analysis.

---

## ⚙️ Tasks Performed

### 1️⃣ Data Quality Assessment

* Checked dataset structure using `.info()`
* Generated statistical summary using `.describe()`
* Verified missing values using `.isnull()`

---

### 2️⃣ Handling Missing Values

* Artificially introduced a missing value in the *math score* column
* Replaced missing values using the **mean** of the column

👉 Reason: Mean is suitable for numerical data and preserves overall distribution.

---

### 3️⃣ Outlier Detection and Handling

* Used the **IQR (Interquartile Range)** method to detect outliers
* Instead of removing them, applied **capping (clipping)**
  to limit extreme values within acceptable bounds

👉 This prevents loss of important data.

---

### 4️⃣ Normalization

Two scaling techniques were applied:

* **Min-Max Scaling** → transforms values between 0 and 1
* **Z-score Standardization** → centers data around mean with unit variance

👉 This ensures fair comparison between features.

---

### 5️⃣ Principal Component Analysis (PCA)

* Checked correlation between numerical features
* Applied PCA to reduce dimensions from 3 features to 2 components
* Visualized the result using a scatter plot

👉 PCA helps in simplifying data while preserving important patterns.

---

## 📈 Results

* Cleaned dataset with no missing values
* Outliers handled effectively
* Data scaled and normalized
* PCA visualization shows distribution of data in reduced dimensions

---

## 🧠 Conclusion

Data preprocessing is a critical step before applying machine learning models.
In this project, multiple techniques were applied to improve data quality, making it more reliable and suitable for analysis.

---

## 🚀 Tools Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib / Seaborn

---
