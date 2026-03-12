# Assignment 2: Data Quality Assessment & Preprocessing

## Dataset: Car Details from Car Dekho

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `CAR_DETAILS_FROM_CAR_DEKHO.csv` | Raw dataset used in this assignment |
| `README.md` | Dataset description and project overview |
| `ARTI406_Assignment2_CarDekho.ipynb` | Jupyter Notebook with full preprocessing pipeline |

---

## 📊 Dataset Description

**Source:** [Kaggle — Vehicle Dataset from CarDekho](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho)

**Domain:** Automotive / Used Car Market

**Size:** 4,340 rows × 8 columns

**Overview:**
This dataset contains listings of used cars available for sale on CarDekho, one of India's largest online automotive platforms. Each row represents a single used car listing, including details about the car's specifications, history, and listed selling price. The dataset reflects real-world data quality challenges such as duplicate entries, extreme outlier values, and the need for type conversion and normalization before any machine learning model can be applied.

---

## 🗂️ Column Details

| Column | Type | Description |
|--------|------|-------------|
| `name` | Categorical | Full model name of the car (e.g., Maruti 800 AC, Honda City) |
| `year` | Numerical | Year the car was manufactured (1992–2020) |
| `selling_price` | Numerical | Listed selling price in Indian Rupees (INR) |
| `km_driven` | Numerical | Total kilometers driven by the car |
| `fuel` | Categorical | Fuel type: Petrol, Diesel, CNG, LPG, Electric |
| `seller_type` | Categorical | Type of seller: Individual, Dealer, Trustmark Dealer |
| `transmission` | Categorical | Gearbox type: Manual or Automatic |
| `owner` | Categorical | Ownership history: First, Second, Third, Fourth & Above, Test Drive Car |

---

## ⚠️ Data Quality Issues Identified

- **763 duplicate rows** found in the original dataset
- **Outliers** detected in `selling_price` (max = 8,900,000 INR) and `km_driven` (max = 806,599 km)
- **Suspicious low value**: `km_driven` minimum = 1 km — likely a data entry error
- **High cardinality**: `name` column contains 1,491 unique car model names
- **Categorical columns** require encoding before being used in ML models

---

## 🔧 Preprocessing Steps Applied

| Task | Description |
|------|-------------|
| **Task 1** | Data Quality Assessment — checked data types, missing values, duplicates, outliers, and categorical distributions |
| **Task 2** | Missing Value Handling — demonstrated 3 strategies: row removal, mean imputation, and median imputation |
| **Task 3** | Outlier Detection & Handling using IQR — detected and removed outliers, then applied percentile capping |
| **Task 4** | Feature Normalization — applied Min-Max Scaling and Z-Score Standardization to numerical features |
| **Task 5** | Dimensionality Reduction — applied PCA and interpreted explained variance with Scree Plot and 2D projection |

---

## 🛠️ Libraries Used

```
pandas       — data loading and manipulation
numpy        — numerical operations
matplotlib   — data visualization
seaborn      — statistical plots
scikit-learn — normalization (MinMaxScaler, StandardScaler) and PCA
```

---

## 👤 Student Information

- **Course:** ARTI406 — Machine Learning
- **Assignment:** Assignment 2 — Data Quality Assessment & Preprocessing
