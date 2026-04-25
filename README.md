# Amazon Sales Analytics Project

## Overview

This project analyzes Amazon marketplace product data to uncover insights related to pricing strategy, customer satisfaction, and customer demand across product categories.

Using Python, SQL, and PostgreSQL (Supabase), the project simulates a real-world analytics workflow involving data cleaning, exploratory analysis, cloud database querying, and business reporting.

---

## Objectives

The project was designed to answer key business questions such as:

- Which categories offer the highest discounts?
- Which categories maintain premium pricing?
- Do discounts improve customer ratings?
- Which categories dominate customer demand?
- Which products balance high ratings with strong value?

---

## Tech Stack

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- PostgreSQL (Supabase)  
- SQLAlchemy  
- python-dotenv  
- Jupyter Notebook

---

## Key Features

### Data Cleaning & Preparation

- Removed currency symbols and formatting issues
- Converted prices, percentages, and review counts into numeric format
- Created structured category features:
  - `main_category`
  - `sub_category`

### Exploratory Data Analysis

- Pricing trends by category
- Discount strategy comparisons
- Ratings and review behavior
- Customer engagement analysis

### SQL Analytics

Uploaded cleaned dataset to cloud PostgreSQL database and executed business queries including:

- Average price by category
- Most reviewed categories
- Best rated categories
- Premium products
- High discount + high rating products

---

## Key Insights

- Electronics and Accessories dominated customer engagement.
- Premium pricing was strongest in Electronics and Home segments.
- Discounts showed only weak relationship with ratings.
- Product quality appeared more important than markdown size.
- Mobile accessories, audio devices, and kitchen products showed strong demand.

---

## Project Structure

```text
amazon-sales-analytics/
│── README.md
│── REPORT.md
│── notebooks/
│   └── analysis.ipynb
│── requirements.txt
│── .env.example
│── data/
│   └── amazon.csv
```

## How to Run
### Clone Repository
```bash
git clone https://github.com/iamkaus/amazon-sales-analytics.git
cd amazon-sales-analytics
```

## Create Virtual Environment (Optional)
```bash
python -m venv .venv
source .venv/bin/activate
```

### For Windows:
```bash
.venv\Scripts\activate
```

## Install Dependencies
```bash
pip install -r requirements.txt
```

## Configure Environment Variables

### Create ```.env```
```bash
DATABASE_URL=your_supabase_postgresql_url
```
**NOTE:** Local MySQL or PostgreSQL servers or any other cloud Database can be used instead if python compatible

## Launch Notebook
```bash
Launch Notebook
```
**NOTE:** An IDE like Pycharm or Text Editor like Visual Studio Code can be used as well.

## Documentation

For full methodology, analysis, and findings:

See [REPORT.md](report/REPORT.md)