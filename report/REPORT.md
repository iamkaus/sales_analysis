# Amazon Sales Analytics Report

## Project Overview

This project presents an end-to-end analytical case study on an Amazon product sales dataset sourced from Kaggle. The goal was to simulate a real-world e-commerce analytics workflow by combining data cleaning, exploratory analysis, business intelligence, SQL reporting, and visualization.

The project demonstrates practical use of Python, SQL, cloud databases, and business-focused storytelling through data.

---

## Dataset Source

**Kaggle:** Amazon Sales Dataset

The dataset contains product-level information such as:

- Product ID  
- Product Name  
- Category Hierarchy  
- Discounted Price  
- Actual Price  
- Discount Percentage  
- Rating  
- Rating Count  
- Product Description  
- Product Links  
- Review Information  

---

## Tech Stack

| Category | Tools Used |
|----------|------------|
| Language | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Database | PostgreSQL (Supabase) |
| SQL Access | SQLAlchemy |
| Environment Variables | python-dotenv |
| Development | Jupyter Notebook / PyCharm |

---

# Project Workflow

## Step 1 — Data Loading

The CSV dataset was imported into Pandas for preprocessing and analysis.

## Step 2 — Data Cleaning

The raw dataset required several transformations:

- Removed currency symbols (`₹`)
- Removed commas from numeric columns
- Converted prices to numeric format
- Converted percentage values to numeric
- Converted rating counts to integers
- Handled missing values
- Standardized column naming

## Step 3 — Feature Engineering

The category hierarchy was split into two analytical features:

- `main_category`
- `sub_category`

Example:

Electronics|Mobiles&Accessories

Converted into:

- main_category = Electronics  
- sub_category = Mobiles&Accessories

This significantly improved category-level analysis.

---

# Section A — Pricing Insights

## Objective

Understand pricing structures, category positioning, and discount strategies.

---

## Analysis Performed

### 1. Average Discount by Category

Measured which categories rely most heavily on markdowns.

### 2. Highest Priced Categories

Calculated average selling price across categories.

### 3. Biggest Markdown Categories

Detected aggressive discounting patterns.

---

## Key Findings

- Electronics and appliance-related categories had the highest average selling prices.
- Several low-ticket categories used high percentage discounts.
- Discount size alone does not imply premium pricing.

---

# Section B — Product Quality Insights

## Objective

Measure customer trust, engagement, and perceived quality.

---

## Analysis Performed

### 1. Highest Rated Products (1000+ Reviews)

Filtered for products with strong ratings and reliable review volume.

### 2. Most Reviewed Categories

Used total review counts as a proxy for demand and customer engagement.

### 3. Discount vs Rating Relationship

Studied whether deeper discounts lead to better ratings.

---

## Correlation Result

Overall correlation between:

- `discount_percentage`
- `rating`

was approximately:

-0.15

---

## Interpretation

- Weak negative relationship
- Heavy discounts do not strongly improve ratings
- Ratings are more influenced by product quality than markdowns
- Discounting alone does not create customer satisfaction

---

## Category-Level Correlation Findings

Most categories showed:

- Weak negative relationship between discounting and ratings
- No strong positive trend
- Some small categories lacked sufficient sample size

---

# Section C — SQL Business Analytics

## Objective

Replicate a professional analyst workflow using SQL on a cloud-hosted relational database.

The cleaned dataset was uploaded to PostgreSQL using Supabase.

---

## Infrastructure Setup

Configured:

- Supabase PostgreSQL instance
- SQLAlchemy engine connection
- `.env` secure credential storage

---

## SQL Queries Executed

### 1. Average Price by Category

Identified category pricing tiers.

### 2. Most Reviewed Categories

Measured engagement concentration.

### 3. Best Rated Categories

Compared average satisfaction across categories.

### 4. High Discount + High Rating Products

Found products balancing strong value and customer approval.

### 5. Premium Products

Detected highest-priced items in the catalog.

---

## SQL Concepts Demonstrated

- SELECT
- WHERE
- GROUP BY
- ORDER BY
- Aggregations
- Sorting
- Filtering
- PostgreSQL casting
- Cloud DB connectivity

---

# Visualizations Created

Charts were used to improve interpretability:

- Customer engagement by category
- Review concentration
- Category comparison plots
- Price distributions
- Correlation analysis
- Top category demand charts

---

# Major Business Insights

## Pricing Strategy

- Premium categories maintain higher average selling prices.
- Large discounts do not necessarily improve product perception.

## Demand Concentration

- Electronics dominated customer review activity.
- Accessories and mobile-related products showed strong demand signals.

## Customer Trust

- High-review products generally sustained stable ratings.
- Review count can be used as a proxy for product traction.

---

# Technical Achievements

This project progressed from simple CSV exploration into a full analytics pipeline:

CSV → Data Cleaning → Feature Engineering → EDA → Visualization → Cloud PostgreSQL Upload → SQL Reporting → Insight Generation

---

# Resume Value

This project demonstrates:

- Data Cleaning & Wrangling
- Exploratory Data Analysis
- SQL Reporting
- Cloud Database Usage
- Visualization
- Business Intelligence
- Environment Variable Management
- Real-world Workflow Simulation
---

# Final Conclusion

This project simulates a practical e-commerce analytics engagement using real product data.

It demonstrates the ability to:

- Work with messy commercial datasets
- Clean and structure data professionally
- Extract business insights
- Use SQL databases in production style
- Communicate findings clearly

This is a strong portfolio-ready analytics project combining technical and business skills.

---

# Author
iamkaus