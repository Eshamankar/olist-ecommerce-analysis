# Brazilian E-Commerce Data Analysis \--- Olist

An exploratory business analysis of the Brazilian E-Commerce Public Dataset by Olist, using Python, SQL and data visualisation.

## Project Overview

This project examines historical e-commerce transactions to understand sales performance, customer purchasing behaviour, product category performance, seller contributions and delivery efficiency.

The analysis combines data preparation in Python, relational queries in SQLite, customer segmentation using RFM metrics, and visualisations to communicate business findings.

## Tools & Technologies

- Python  
- Pandas and NumPy  
- SQLite and SQL  
- Matplotlib and Seaborn  
- Google Colab

## Analysis

- Data loading and quality assessment across nine CSV datasets  
- Data preparation and timestamp-derived features  
- SQLite database creation and SQL business analysis  
- Monthly product revenue trends  
- Product category and seller performance  
- One-time versus repeat-purchase behaviour  
- RFM customer segmentation  
- Delivery duration and delivery-delay analysis  
- Consolidated business performance dashboard

## Key Findings

- Analysed 99,441 orders across the Olist dataset.  
- 96,478 orders were marked as delivered.  
- Delivered orders generated approximately **R\$13.22 million in product revenue**, excluding freight.  
- **Health & Beauty** was the highest-revenue product category.  
- Approximately **97% of delivered customers** placed one order during the dataset's observation window.  
- Average delivery time was **12.56 days**.  
- **8.11% of delivered orders** arrived after the estimated delivery date.  
- Average delivery delay was **−11.18 days**, meaning orders arrived earlier than estimated on average.

## Repository Structure

```
Olist_project/
├── Data/
│   ├── olist_orders_dataset.csv
│   ├── olist_customers_dataset.csv
│   ├── olist_order_items_dataset.csv
│   ├── olist_order_payments_dataset.csv
│   ├── olist_order_reviews_dataset.csv
│   ├── olist_products_dataset.csv
│   ├── olist_sellers_dataset.csv
│   ├── olist_geolocation_dataset.csv
│   └── product_category_name_translation.csv
├── outputs/
│   └── Exported analysis tables
├── Olist_Ecommerce_Analysis_GoogleDrive.ipynb
├── olist.db
├── olist_dashboard.png
└── README.md
```

## Dataset Source

[Olist Brazilian E-Commerce Public Dataset \--- Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## Limitations

- The dataset contains historical transactions from 2016--2018 and may not represent current marketplace behaviour.  
- Product revenue and freight charges are sales-value measures, not profit; cost and margin data are unavailable.  
- Repeat-purchase analysis is limited by the dataset's observation window. A customer with one recorded order may have purchased outside that period.  
- RFM thresholds and segment labels are analyst-defined exploratory rules, not validated churn predictions.  
- Missing timestamps and product attributes may affect some analyses.  
- Seller revenue alone does not measure seller profitability or service quality.

## How to Reproduce

1. Download the dataset from the Kaggle source above.  
2. Place the nine CSV files in the `Data/` folder.  
3. Open `Olist_Ecommerce_Analysis.ipynb` in Google Colab.  
4. Mount Google Drive and set the project path to your `Olist_project` folder.  
5. Run the notebook cells sequentially.