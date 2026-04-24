# Amazon Sales Analytics Project  
### Pricing Strategy, Product Quality & Customer Demand Insights

---

# Introduction

In highly competitive e-commerce marketplaces, understanding customer behavior, pricing strategy, and product quality signals is essential for improving revenue and decision-making.

Amazon hosts thousands of products across multiple categories, making it an ideal environment to analyze how discounts, ratings, and customer engagement vary across segments.

This project uses real marketplace data to extract business insights through exploratory data analysis and performance metrics.

---

# Project Objective

The objective of this project is to analyze Amazon product listings and identify meaningful patterns related to:

- Pricing and discount strategy  
- Product quality perception through ratings  
- Customer engagement through review volume  
- Category-wise product performance  
- Demand concentration across product segments

---

# What We Aim to Accomplish

Through this analysis, we aim to answer the following business questions:

1. Which categories provide the highest discounts?  
2. Which categories command premium prices?  
3. Do discounts improve customer ratings?  
4. Which products attract the most customer attention?  
5. Which categories dominate marketplace demand?  
6. What strategic opportunities exist for sellers?

---

# Dataset Overview

**Source:** Kaggle Amazon Sales Dataset

The dataset includes:

- Product Name  
- Category  
- Discounted Price  
- Actual Price  
- Discount Percentage  
- Rating  
- Rating Count  
- Product Description

Each row represents a listed product with customer engagement and pricing information.

---

# Data Cleaning & Preparation

To ensure accurate analysis, the following preprocessing steps were completed:

- Removed currency symbols (`₹`) and commas from price columns  
- Converted prices into numeric format  
- Converted discount percentages into numeric values  
- Converted review counts into numeric values  
- Split category hierarchy into:
  - `main_category`
  - `sub_category`
- Checked for missing values and corrected datatypes

---

# Section A — Pricing Insights

This section focuses on how pricing strategy differs across categories.

---

## A1. Average Discount by Category

Analyze average discount percentages across major categories.

### Insights

- Electronics and accessories showed consistently higher discounts.
- Competitive categories rely heavily on markdowns.
- Niche categories maintained relatively lower discount dependency.

### Key Finding

Price-sensitive markets tend to use discounts aggressively to attract conversions.

---

## A2. Highest Priced Categories

Analyze categories with highest average discounted selling price.

### Insights

- Electronics dominated premium pricing tiers.
- Home appliances maintained strong average selling prices.
- Low-ticket accessory categories remained inexpensive.

### Key Finding

Premium categories can generate stronger margins if trust and quality remain high.

---

## A3. Discount vs Rating Relationship

Correlation between `discount_percentage` and `rating`:

**Correlation = -0.155**

### Insights

- Discounts do not strongly improve ratings.
- Slight negative association exists between larger discounts and ratings.
- Product quality matters more than markdown strategy.

### Key Finding

Discounting alone is not an effective strategy for improving customer satisfaction.

---

# Section B — Product Quality Insights

This section evaluates customer trust and product satisfaction.

---

## B1. Highest Rated Products (1000+ Reviews)

Products with strong ratings and sufficient review volume were identified.

### Insights

- Several products sustained excellent ratings with large review counts.
- High trust products often belong to utility / repeat-purchase categories.

### Key Finding

Products combining scale + rating signal strong long-term marketplace fit.

---

## B2. Most Reviewed Products

Products with the highest review counts indicate customer attention and likely sales volume.

### Insights

- Electronics and accessories dominated review counts.
- Frequently purchased everyday products gained large engagement.

### Key Finding

Review volume acts as a strong proxy for product popularity.

---

## B3. Best Rated Categories

Average rating compared across categories.

### Insights

- Certain niche categories showed stronger average satisfaction.
- High-demand categories sometimes had slightly lower ratings due to larger scale.

### Key Finding

Mass-market demand does not always guarantee higher customer satisfaction.

---

# Section C — Customer Demand Insights

This section focuses on customer engagement and demand concentration.

---

## C1. Review Volume by Category

Total ratings/reviews aggregated by category.

### Insights

- Electronics generated the largest customer engagement.
- Computers & Accessories followed closely.
- Home & Kitchen showed strong mid-tier demand.

### Key Finding

Demand is heavily concentrated in technology-driven categories.

---

## C2. Top Subcategories by Customer Engagement

Review volume analyzed at subcategory level.

### Insights

Top performing subcategories included:

- Headphones / Earbuds  
- Mobiles & Accessories  
- Home Theater / TV  
- Accessories & Peripherals  
- Kitchen Appliances

### Key Finding

Subcategory analysis provides sharper demand signals than category-level summaries.

---

# Strategic Recommendations

Based on the findings:

1. Focus inventory on high-demand accessory and electronics segments.  
2. Use discounts selectively; prioritize quality improvements over aggressive markdowns.  
3. Expand into high-engagement subcategories with repeat purchase behavior.  
4. Protect premium pricing in trusted categories with strong ratings.

---

# Final Conclusion

This project reveals that Amazon demand is concentrated in Electronics, Accessories, and Home utility categories, while customer satisfaction is influenced more by product quality than discount size.

The analysis demonstrates how pricing data, ratings, and engagement metrics can be transformed into practical marketplace strategy decisions.

---

# Tools Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook