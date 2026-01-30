# E-Commerce Data Engineering Pipeline

A comprehensive data engineering lab demonstrating the 15-step roadmap from raw data ingestion to feature engineering and serialization. Built for **PROG8245 - Machine Learning Programming**.

## Project Synopsis

This project implements a complete data pipeline for e-commerce transaction data, including:
- Custom Python classes for data encapsulation (`SalesRecord` with `clean()` and `total()` methods)
- Data quality profiling and cleaning workflows
- Feature engineering (recency metrics, value segmentation)
- Multi-format serialization (CSV + JSON)

## Quick Start

```bash
# Clone the repository
git clone https://github.com/chooksemmanuel/ml-data-preprocessing-lab.git
cd ml-data-preprocessing-lab

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook data_engineering_lab.ipynb
```

## Data Sources

| File | Description | Source |
|------|-------------|--------|
| `data/ecommerce_sales.csv` | 550 synthetic e-commerce transactions | Generated with `generate_data.py` |
| `data/product_metadata.csv` | Product catalog with categories and prices | Secondary metadata source |
| `data/coupon_details.json` | Coupon code discount mappings | Secondary metadata source |

**Note**: The synthetic dataset includes intentional data quality issues (missing values, negative prices, inconsistent casing) for cleaning exercises.

## Project Structure

```
ml-data-preprocessing-lab/
├── README.md
├── requirements.txt
├── .gitignore
├── data_engineering_lab.ipynb    # Main notebook (all 12 steps)
├── data/
│   ├── ecommerce_sales.csv       # Primary dataset
│   ├── product_metadata.csv      # Product details
│   ├── coupon_metadata.csv       # Coupon info
│   ├── coupon_details.json       # Coupon JSON format
│   └── generate_data.py          # Data generation script
└── output/
    ├── cleaned_sales_data.csv    # Cleaned output
    └── cleaned_sales_data.json   # JSON serialization
```

## Author

Emmanuel (Chooks) - Graduate Student, Applied AI & Machine Learning

## License

This project is for educational purposes as part of coursework.
