# Sales Forecasting Report — Olist Dataset

This repository contains a comprehensive Jupyter Notebook, `sales_forecasting_final.ipynb`, which documents a complete data science workflow to build a sales forecasting model using the Olist e-commerce dataset.

## Project Summary

The notebook demonstrates an end-to-end process for sales forecasting, including:

- Data ingestion and integration from multiple CSV tables.
- Data cleaning and validation (handling missing values, fixing inconsistencies, and removing duplicates).
- Exploratory Data Analysis (EDA) with descriptive statistics and visualizations to identify trends and outliers.
- Feature engineering for time-series and tabular modeling, including seasonality and aggregated metrics.
- Model training and evaluation using scikit-learn and XGBoost, with model selection and validation.

Key libraries used: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`.

## Dataset

This project uses the Brazilian E-Commerce Public Dataset provided by Olist. The relevant CSV files are expected to be placed in `data/full/` and include:

- `olist_orders_dataset.csv` — orders and timestamps (purchase, approval, delivery).
- `olist_order_items_dataset.csv` — order line items, product IDs, prices, shipping costs, seller IDs.
- `olist_products_dataset.csv` — product attributes (category, weight, dimensions).
- `olist_customers_dataset.csv` — customer identifiers and locations (ZIP code, city, state).
- `olist_geolocation_dataset.csv` — ZIP code latitude/longitude for geospatial analysis.
- `olist_order_payments_dataset.csv` — payment methods and installment details.
- `olist_order_reviews_dataset.csv` — customer ratings and review text.
- `olist_sellers_dataset.csv` — seller information and locations.

Notes:

- Raw data files are typically large and are excluded from this repository by `.gitignore` (see `data/full/`).
- Model artifacts (e.g., `*.pkl`) are also excluded from version control.

## Usage

1. Create a Python environment and install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

   If a `requirements.txt` file is not present, install the essentials:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost jupyter
   ```

2. Place the Olist CSV files in `data/full/`.
3. Launch Jupyter and open `sales_forecasting_final.ipynb` to run the analysis and reproduce the results.

## License

This project is licensed under the MIT License — see `LICENSE` for details.

---

If you would like, I can also add a shorter English summary for the notebook header and a `requirements.txt` file listing the exact package versions used for reproduction.
