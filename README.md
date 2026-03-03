# 📊 Customer Churn Analysis & Retention Dashboard (Telco)

An interactive **Customer Churn Analysis Dashboard** built using **HTML + Plotly (generated from Python/Google Colab)** to analyze churn patterns, identify high-risk customer segments, and support retention strategy decisions.

This project uses the **IBM Telco Customer Churn dataset** and focuses on business-oriented insights such as churn by contract type, tenure, internet service, payment method, and support services.

---

## 🚀 Project Objective

The goal of this project is to:

- Analyze customer churn behavior using data-driven insights
- Identify high-risk segments likely to churn
- Create an interactive dashboard for churn monitoring and retention analysis
- Support decision-making with KPI tracking and segment-level insights

---

## 📁 Dataset

- **Dataset:** IBM Telco Customer Churn
- **File used:** `WA_Fn-UseC_-Telco-Customer-Churn.csv`

### Key columns used
- `Churn`
- `tenure`
- `MonthlyCharges`
- `TotalCharges`
- `Contract`
- `InternetService`
- `PaymentMethod`
- `TechSupport`
- `OnlineSecurity`
- `SeniorCitizen`
- `gender`

---

## 🛠️ Tools & Technologies

- **Python** (Google Colab)
- **Pandas** (data loading / preprocessing)
- **HTML / CSS / JavaScript**
- **Plotly.js** (interactive visualizations)

---

## ✅ Dashboard Features

- **Interactive filters** (multi-select + numeric ranges)
- **KPI cards**
  - Total Customers
  - Churned Customers
  - Retained Customers
  - Churn Rate %
  - Avg Monthly Charges
  - Avg Total Charges
- **Interactive charts**
  - Churn distribution
  - Churn rate by contract type
  - Churn rate by tenure group
  - Churn rate by internet service
  - Churn rate by payment method
  - Churn rate by tech support
  - Monthly charges distribution by churn
  - Churn rate trend by tenure (months)
- **High-risk heatmap**
  - Contract × Payment Method churn rate
- **Segment-level analysis table**
  - Top high-churn combinations (Contract + Internet + Payment)
- **Auto-generated insight summary**
- **Filtered data export (CSV)** *(if using the standalone HTML version with export enabled)*

---

## 🧹 Data Cleaning & Preparation

The following preprocessing steps were applied:

- Converted `TotalCharges` from text to numeric
- Removed rows with invalid/missing `TotalCharges`
- Converted `SeniorCitizen` from `0/1` to `Yes/No`
- Created derived fields:
  - `Churn_Flag`
  - `tenure_group`
  - `monthly_charge_band`
  - `total_charge_band`
  - `service_count` (optional feature for segmentation)

---

## 📌 Key Business Insights (Example)

Some common insights observed from this dataset include:

- **Month-to-month contract** customers show significantly higher churn than long-term contracts
- Customers with **short tenure (early lifecycle)** have higher churn risk
- Customers using **Electronic check** often show higher churn rates
- Customers without **TechSupport / OnlineSecurity** tend to churn more
- Higher monthly charges may be associated with increased churn in some segments

> Exact values may change when filters are applied.

---

## ▶️ How to Run

### Option 1: Open the HTML dashboard directly
1. Download or clone this repository
2. Open `telco_churn_dashboard.html` in your browser

### Option 2: Generate the dashboard using Google Colab
1. Upload `WA_Fn-UseC_-Telco-Customer-Churn.csv`
2. Run the provided Colab notebook/script
3. Export `telco_churn_dashboard.html`
4. Open it in a browser or upload to GitHub

---

## 📸 Screenshots

Add screenshots in a `screenshots/` folder and link them here.

Example:

```markdown
![Dashboard Overview](screenshots/dashboard_overview.png)
![Churn Heatmap](screenshots/churn_heatmap.png)
![Segment Table](screenshots/segment_table.png)
