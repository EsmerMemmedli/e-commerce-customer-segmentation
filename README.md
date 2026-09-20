
### E-Commerce Customer Segmentation

## Project Overview

This project focuses on analyzing e-commerce customer purchasing behavior using **RFM (Recency, Frequency, Monetary) analysis**.

The goal is to segment customers based on their transaction history, identify differences in customer value, and visualize the results through an interactive **Power BI dashboard**.

---

## Objectives

- Analyze **1M+ e-commerce transaction records**.
- Clean and preprocess transaction data using **Python and Pandas**.
- Calculate **Recency, Frequency, and Monetary** metrics.
- Segment **5,878 customers** into four customer value groups.
- Visualize customer segments and key insights using **Power BI**.
- Provide business recommendations based on customer purchasing behavior.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Power BI

---

## Dataset

The project uses the **Online Retail II** dataset, which contains over **1 million e-commerce transaction records**.

The dataset includes:

- `Invoice`
- `StockCode`
- `Description`
- `Quantity`
- `InvoiceDate`
- `Price`
- `Customer ID`
- `Country`

---

## Data Cleaning

The following preprocessing steps were performed:

- Removed records with missing `Customer ID`.
- Removed duplicate records.
- Removed transactions with `Quantity <= 0`.
- Removed transactions with `Price <= 0`.
- Converted `InvoiceDate` to datetime format.
- Created a `TotalAmount` column.

```python
TotalAmount = Quantity * Price
````

After cleaning and preprocessing, the data was prepared for customer-level RFM analysis.

---

## RFM Analysis

RFM analysis was performed using three key metrics:

| Metric        | Description                                       |
| ------------- | ------------------------------------------------- |
| **Recency**   | Number of days since the customer's last purchase |
| **Frequency** | Number of purchases made by the customer          |
| **Monetary**  | Total amount spent by the customer                |

RFM scores were calculated for each customer and combined to create an overall **RFM Score**.

---

## Customer Segmentation

A total of **5,878 customers** were segmented into four customer value groups:

* **Top Customers**
* **High Value Customers**
* **Medium Value Customers**
* **Low Value Customers**

The segmentation was based on the combined RFM score.

---

## Power BI Dashboard

A **Power BI dashboard** was developed using the customer-level RFM dataset.

The dashboard includes:

* Customer distribution across segments.
* Recency, Frequency, and Monetary metrics.
* Comparison of customer purchasing behavior.
* **Frequency vs Monetary** scatter plot.
* Key customer segmentation insights.

### Main Visualization

**Frequency vs Monetary — Scatter Plot**

This visualization helps analyze the relationship between purchase frequency and customer spending.

### Dashboard 

<img width="1298" height="728" alt="image" src="https://github.com/user-attachments/assets/13566716-f000-4881-83ce-9b7df4211376" />


---

## Key Findings

* **Top Customers** showed the highest average purchase frequency and monetary value.
* **Low Value Customers** showed lower average purchase frequency and spending.
* RFM segmentation revealed clear differences in customer purchasing behavior.

---

## Business Recommendations

* Develop customer retention strategies for **Top Customers**.
* Encourage repeat purchases among **Medium Value Customers**.
* Use targeted engagement strategies for **Low Value Customers**.
* Monitor customer purchasing behavior to identify changes in activity.
* Use RFM segments to support targeted marketing strategies.

---

## Project Structure

```text
E-Commerce-Customer-Segmentation/
│
├── E-Commerce Customer Segmentation.ipynb
├── README.md
└── Power BI Dashboard
```

---

## Project Status

* [x] Data Cleaning
* [x] RFM Analysis
* [x] Customer Segmentation
* [x] Power BI Dashboard
* [x] Data Visualization
* [x] Business Recommendations

---
