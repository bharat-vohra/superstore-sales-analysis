# Superstore Sales & Profitability Analysis

## Project Overview

This project analyzes the Superstore dataset using Python and Pandas to understand sales performance, profitability, customer behavior, discounting, geographic performance, and trends over time.

The analysis focuses on identifying patterns that affect profitability and translating those findings into practical business recommendations.

## Business Questions

- How do sales and profitability vary across product categories and sub-categories?
- How is profitability affected by discount levels?
- Which customers contribute disproportionately to profit?
- Which products and states show significant profitability issues?
- How do sales and profitability change over time?

## Dataset

The project uses the Superstore sales dataset containing order-level sales information, including order and customer details, products, categories, sales, quantity, discount, profit, geography, and order dates.

The notebook performs data-quality checks, including missing-value and duplicate checks, and converts order dates to datetime format before analysis.

## Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Jupyter Notebook**

## Analytical Approach

1. Load and inspect the dataset
2. Perform data-quality checks and preparation
3. Establish overall business KPIs
4. Analyze category, sub-category, and product performance
5. Investigate discounting and profitability
6. Analyze customer segments and customer concentration
7. Compare geographic sales and profitability
8. Examine annual and monthly trends
9. Summarize findings and business recommendations

## Key Findings

### 1. Higher discounts are strongly associated with lower profitability

Aggregate profit margin declined sharply as discount levels increased. Profit margin was **29.51% at 0% discount**, fell to **11.82% at 20%**, became negative at **30% (-10.06%)**, and deteriorated further at higher discount levels, reaching **-180.03% at 80%**.

### 2. Profitability is highly concentrated among high-value customers

The **top 20% of customers by sales generated 48.14% of total sales but 81.66% of total profit**, with a **21.15% profit margin** compared with **9.74% for the remaining 80%**.

### 3. Some high-sales states are loss-making

**Texas** generated approximately **$170.2K in sales with a -15.12% profit margin**, while **Pennsylvania** generated approximately **$116.5K with a -13.35% margin**. Their average discounts were substantially higher than those of profitable high-sales states such as California and New York.

### 4. High discounts were a recurring feature of material product losses

The loss-making products investigated showed major losses concentrated in transactions with very high discounts, particularly **50–80%**. Lower-discount transactions for the investigated products were profitable, consistent with the broader relationship observed between discounting and profitability.

### 5. Sales grew substantially, but profitability did not improve consistently

Sales increased from approximately **$484K in 2019 to $733K in 2022**, while profit increased from approximately **$49.6K to $93.4K**. Profit margin peaked at **13.43% in 2021** before declining to **12.74% in 2022**, indicating that sales growth did not automatically translate into improving profitability.

## Business Recommendations

1. **Review high discounts** — introduce additional review controls for discounts of 30% or higher, where aggregate profitability becomes negative in the dataset.
2. **Protect high-value customers** — prioritize retention and relationship management for customers who contribute disproportionately to profit.
3. **Investigate loss-making states** — review pricing and discounting practices in Texas and Pennsylvania, particularly across categories with elevated discounts.
4. **Review materially loss-making products** — investigate pricing, discounting, and transaction-level economics before considering product-level changes.
5. **Monitor profitability alongside sales growth** — evaluate margin performance during high-volume periods rather than relying on sales growth alone.

## Visualizations

The notebook includes visualizations covering:

- Sales and profit by category
- Profit margin by discount level
- Loss-making products
- Profitability across major states
- Sales and profit contribution by customer group

## Project Structure

```text
Superstore-Sales-Analysis/
│
├── Superstore Sales Analysis.ipynb
├── README.md
└── data/
    └── Sample - Superstore.csv
```

## How to Run

1. Clone or download the repository.
2. Open `Superstore Sales Analysis.ipynb` in Jupyter Notebook or JupyterLab.
3. Ensure the Superstore dataset is available at the path expected by the notebook.
4. Run the notebook from top to bottom.

## Outcome

This project demonstrates a practical exploratory data-analysis workflow using Python, Pandas, and NumPy, with an emphasis on moving from raw transactional data to business insights and recommendations.
