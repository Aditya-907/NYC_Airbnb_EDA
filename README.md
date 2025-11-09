<h1 align="center">  NYC Airbnb Market Analysis (2019) </h1>
<p align="center">
  <i>Exploratory Data Analysis of Airbnb Listings Across New York City's Boroughs</i>
</p>
<p align="center">
  <img src="images/New_York_City_.png" width="400">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9+-blue.svg" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange.svg" />
  <img src="https://img.shields.io/badge/License-MIT-green.svg" />
  <img src="https://img.shields.io/badge/EDA-Project-lightgrey.svg" />
</p>

---

## Project Overview

This project performs a **comprehensive Exploratory Data Analysis (EDA)** on the **New York City Airbnb Open Data (2019)** to uncover insights into pricing behavior, spatial trends, availability, and customer engagement patterns across boroughs.

The analysis explores:

- Market segmentation by location and accommodation type
- Spatial price distribution and outlier behavior
- Temporal availability and review activity
- Categorical and numerical feature interactions
- Correlation and dependency structures among variables

By combining **statistical rigor** and **data visualization**, this study captures both the macro-level market structure and micro-level behavioral dynamics of Airbnb listings across New York City.

---

## Tech Stack and Libraries

| Category          | Tools / Libraries               |
| ----------------- | ------------------------------- |
| Language          | Python                          |
| Environment       | Jupyter Notebook                |
| Data Handling     | `pandas`, `numpy`           |
| Visualization     | `matplotlib`, `seaborn`     |
| Environment Setup | `pip`, `venv`               |
| Dataset Source    | Airbnb Open Data (InsideAirbnb) |

---

## Dataset Information

- **Dataset Name:** NYC Airbnb Open Data (2019)
- **Records:** ~49,000 listings
- **Features:** 16 (original) → 20 (engineered)
- **Primary Variables:**
  - `neighbourhood_group` – Borough location (Manhattan, Brooklyn, etc.)
  - `room_type` – Entire home/apartment, Private room, Shared room
  - `price` – Listing cost per night
  - `availability_365` – Days available per year
  - `number_of_reviews`, `reviews_per_month` – Engagement metrics

---

## Repository Structure

```bash
NYC_Airbnb_EDA/
│
├── data/
│   └── AB_NYC_2019.csv
│
├── notebooks/
│   ├── EDA_Report.ipynb
│   └── AB_NYC_2019_engineered.csv
│
├── images/
│   └── New_York_City_.png
│
├── README.md
└── requirements.txt
```

## EDA Workflow

### Data Preprocessing

- Handling missing values (`name`, `host_name`, `reviews_per_month`)
- Type conversion (`last_review` → datetime)
- Outlier treatment using quantile capping (99th percentile)
- Feature engineering (review metrics, host attributes)

### Univariate Analysis

- Distribution plots for price, reviews, and availability
- Categorical frequency for boroughs and room types

### Bivariate and Multivariate Analysis

- Price variation across boroughs and room types
- Correlation analysis for numeric variables
- Price–availability–review interactions
- Market segmentation through cross-feature visualization

### Deriving Insights

- Identifying high-value clusters and budget zones
- Understanding the role of privacy and exclusivity in pricing
- Detecting demand elasticity through availability metrics

---

## Key Insights

💡 **Spatial Segmentation:**
Manhattan and Brooklyn dominate both in listing count and average price, forming the premium tier of the Airbnb ecosystem.

💡 **Price Hierarchy:**
“Entire home/apartment” listings exhibit substantially higher mean prices than private or shared rooms.

💡 **Demand Dynamics:**
Listings with more reviews are generally lower-priced, reflecting higher guest turnover.

💡 **Availability Patterns:**
High-priced listings display lower annual availability, implying higher occupancy or controlled seasonal listing behavior.

💡 **Weak Numeric Correlations:**
Most numeric features (reviews, availability, minimum nights) have low collinearity, indicating orthogonal market features primarily shaped by categorical dimensions.

---

## Conclusion

This EDA establishes that **Airbnb’s New York City market is spatially stratified, economically polarized, and behaviorally elastic**.
Manhattan and Brooklyn dominate the premium segment, while Queens, Bronx, and Staten Island represent affordable alternatives.
The platform exhibits classical microeconomic features of **price–demand elasticity**, **market segmentation**, and **value differentiation by privacy**.

---

## Author

**Aditya (@Aditya-907)**

Email - adityasinght970@gmail.com  

**“Busy trying my best.”**

---
