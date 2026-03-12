# Used Cars Dataset Description

## Overview
This dataset contains information about 500 used cars in the Saudi Arabian market. It includes various features that influence the price of used vehicles.

## Dataset Information
- **Number of Records:** 500
- **Number of Features:** 10
- **File Format:** CSV
- **File Name:** used_cars_dataset.csv

## Features Description

| Column Name | Data Type | Description | Values/Range |
|------------|-----------|-------------|--------------|
| **Brand** | String | Car manufacturer | Toyota, Honda, Ford, BMW, Mercedes, Nissan, Hyundai, Kia |
| **Model_Year** | Integer | Year the car was manufactured | 2010 - 2023 |
| **Mileage_KM** | Integer | Total distance traveled in kilometers | 5,000 - 250,000 KM |
| **Engine_Size** | Float | Engine displacement in liters | 1.5, 1.6, 2.0, 2.5, 3.0, 3.5, 4.0 L |
| **Fuel_Type** | String | Type of fuel used | Petrol, Diesel, Hybrid, Electric |
| **Transmission** | String | Transmission type | Manual, Automatic |
| **Color** | String | Exterior color of the car | White, Black, Silver, Blue, Red, Gray |
| **Number_of_Owners** | Integer | Number of previous owners | 1 - 4 |
| **Accident_History** | String | Whether the car had accidents | Yes, No |
| **Price_SAR** | Float | Selling price in Saudi Riyals | 15,000 - 115,000 SAR |

## Data Quality Notes

### Missing Values
- **Engine_Size:** ~3% missing values (filled with median)
- **Accident_History:** ~5% missing values (filled with mode)

### Outliers
- Price contains some outliers (luxury cars or special conditions)
- Mileage has natural variation based on car age and usage

## Target Variable
**Price_SAR** is the target variable for prediction models. It represents the selling price of the car in Saudi Riyals.

## Key Relationships
1. **Price vs Model_Year:** Newer cars have higher prices
2. **Price vs Mileage:** Higher mileage reduces price
3. **Price vs Brand:** Luxury brands (BMW, Mercedes) command premium prices
4. **Price vs Fuel_Type:** Hybrid and Electric cars are more expensive
5. **Price vs Accident_History:** Cars without accidents are more valuable

## Use Cases
This dataset can be used for:
- Price prediction models
- Market analysis
- Feature importance analysis
- Classification tasks (price categories)
- Regression analysis
- Data visualization practice

## Statistics Summary

### Price Distribution
- **Mean:** ~21,500 SAR
- **Median:** 15,000 SAR
- **Min:** 15,000 SAR
- **Max:** ~115,000 SAR
- **Std Dev:** ~16,800 SAR

### Brand Distribution
The dataset includes a balanced mix of economy and luxury brands, reflecting real market conditions.

### Fuel Type Distribution
- Petrol: ~50%
- Diesel: ~30%
- Hybrid: ~15%
- Electric: ~5%

### Transmission Distribution
- Automatic: ~70%
- Manual: ~30%

## Data Collection
This is a synthetic dataset created for educational purposes, simulating realistic patterns in the used car market based on Saudi Arabian market conditions.

## Recommended Analysis Steps
1. Exploratory Data Analysis (EDA)
2. Handle missing values
3. Detect and treat outliers
4. Feature engineering (e.g., Car_Age)
5. Correlation analysis
6. Visualization of key relationships
7. Model building and evaluation

## Citation
Dataset created for ARTI406 - Machine Learning Course Assignment 1

## Contact
For questions about this dataset, please contact your course instructor.

---
**Last Updated:** February 2024
**Version:** 1.0
