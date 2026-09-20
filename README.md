# E-Commerce Customer Segmentation

## Project Overview

This project focuses on analyzing e-commerce customer purchasing behavior using **RFM (Recency, Frequency, Monetary) analysis**.

The goal is to segment customers based on their transaction history, understand differences in customer value, and present the results through an interactive **Power BI dashboard**.

RFM analysis evaluates customers based on:
- **Recency** — how recently a customer made a purchase
- **Frequency** — how frequently a customer makes purchases
- **Monetary** — how much a customer spends

---

## Objectives

- Clean and prepare the raw transaction dataset.
- Analyze customer purchasing behavior.
- Calculate Recency, Frequency, and Monetary metrics.
- Assign RFM scores and segment customers.
- Visualize customer segments and purchasing patterns in Power BI.
- Provide business recommendations based on the analysis.

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

The project uses the **Online Retail II** dataset, which contains e-commerce transaction records.

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

The following data preparation steps were performed:

- Removed records with missing `Customer ID`.
- Removed duplicate records.
- Excluded transactions with `Quantity <= 0`.
- Excluded transactions with `Price <= 0`.
- Converted `InvoiceDate` to datetime format.
- Created a `TotalAmount` column:

```python
TotalAmount = Quantity * Price

