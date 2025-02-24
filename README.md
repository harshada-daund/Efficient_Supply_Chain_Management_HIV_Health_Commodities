# 🏥 Efficient Supply Chain Management for HIV Health Commodities

## 📌 Project Overview
This project aims to optimize the supply chain for HIV health commodities, including antiretroviral (ARV) medications and HIV testing kits, using predictive analytics and machine learning techniques. The goal is to improve delivery timelines, reduce costs, and identify key factors contributing to shipment delays and inefficiencies.

---

## ✨ Objectives
1. **Prediction Goals:**
   - Classify shipments as On-Time, Less Delay, Moderate Delay, or Severe Delay.
   - Predict the number of delay days as a continuous metric.

2. **Inference Goals:**
   - Analyze relationships between shipment attributes (e.g., cost, weight, vendor) and delivery delays.
   - Identify key logistical factors contributing to delays by region or shipment mode.

3. **Actionable Goals:**
   - Provide recommendations for cost reduction and process improvements.
   - Prioritize resource allocation for time-sensitive shipments.
   - Highlight areas for vendor and regional optimization.

---

## 📂 Dataset Overview
- **Source:** [USAID Supply Chain Shipment Pricing Dataset](https://data.usaid.gov/HIV-AIDS/Supply-Chain-Shipment-Pricing-Dataset/a3rc-nmf6/about_data)
- **Size:** ~10,000 rows and 33 columns.
- **Time Frame:** Data spans from 2006 to 2015.
- **Geographic Coverage:** Global shipments with regional breakdowns.
- **Key Features:**
  - Shipment Mode, Country, Vendor, Weight, Freight Cost, Line Item Value.
  - Delivery details such as Scheduled Delivery Date and Delivered to Client Date.

---

## 🔍 Methodology

1. **Data Preprocessing:**
   - Handled missing values using imputation techniques.
   - Standardized date columns for consistency.
   - Applied SMOTE to balance delay categories.
   - Created features like "Scheduled-to-Delivered Days" and "Freight Cost per Weight Unit."

2. **Exploratory Data Analysis (EDA):**
   - Analyzed trends in delivery times and shipment costs.
   - Visualized shipment modes, delivery timelines, and vendor performance.
   - Conducted correlation and ANOVA tests to uncover key relationships.

3. **Modeling Techniques:**
   - **Random Forest Classifier:** Achieved 99.58% accuracy in classifying shipment delays.
   - **Linear Regression:** Used to predict the number of days delayed, with limited success (R² = 0.07).

4. **Model Evaluation:**
   - Used metrics like accuracy, precision, recall, F1-score, mean absolute error (MAE), and mean squared error (MSE).
   - Identified important features influencing shipment delays: Shipment Mode, Line Item Value, Pack Price.

---

## 📈 Key Insights

- **Top Delivery Bottlenecks:** Congo, Togo, and Benin have the longest average delivery times.
- **High-Value Regions:** Southern Africa shows the highest total line item values.
- **Delivery Status:** 88.5% of shipments were on time, while 11.5% experienced delays.
- **Delay Patterns:** Ocean and truck modes are associated with moderate delays, while air mode is more reliable.
- **Cost Factors:** Freight Cost, Shipment Mode, and Line Item Value are major predictors of delays.

---

## 🛠️ Technologies Used

- **Data Cleaning & Processing:** Python (Pandas, NumPy), PySpark, Tableau Prep
- **Modeling:** Random Forest, Linear Regression, ANOVA, SMOTE
- **Visualization:** Tableau, Matplotlib, Seaborn
- **Data Source:** USAID Supply Chain Shipment Pricing Dataset

---

## 📂 Getting Started

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd <repository-folder>
