# Amazon Sales Analytics Project Report

## Business Problem

Amazon sellers operate in highly competitive markets where pricing, product quality, and visibility directly affect sales performance.

This project analyzes marketplace data to identify where sellers should compete on price, where they should compete on quality, and which categories attract the highest demand.

---

## Objectives

- Analyze category-level pricing trends
- Identify strongest demand segments
- Measure effect of discounts on ratings
- Evaluate product quality signals
- Recommend marketplace growth strategies

---

## Dataset Summary

Rows: Product listings  
Columns: Pricing, category, rating, review metrics, descriptions

Key variables:

- discounted_price
- actual_price
- discount_percentage
- rating
- rating_count

---

## Cleaning Steps

- Converted string prices to numeric
- Converted review counts to numeric
- Removed formatting symbols
- Split hierarchical category field

---

## Analysis Sections

### 1. Pricing Insights

- Electronics maintained highest average prices
- Accessory segments showed heavy markdown behavior

### 2. Quality Insights

- Several products achieved high ratings at scale
- Ratings were not strongly explained by discounts

### 3. Demand Insights

- Electronics generated highest review activity
- Subcategories like audio and mobile accessories led demand

---

## Strategic Recommendations

1. Expand high-demand accessory inventory
2. Protect margins in premium trusted segments
3. Use discounting tactically
4. Improve quality rather than relying on markdowns

---

## Conclusion

This project demonstrates how marketplace data can be transformed into actionable commercial intelligence using Python-based analytics.

---

## Tools

Python, Pandas, NumPy, Seaborn, Matplotlib