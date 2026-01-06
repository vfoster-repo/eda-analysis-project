# Instacart Market Basket Analysis

An exploratory data analysis of customer shopping behavior using Instacart's grocery shopping dataset.

## Project Overview

This project analyzes shopping patterns, product preferences, and customer reordering behavior from Instacart's transactional data. The analysis provides actionable insights for inventory management, marketing strategies, and customer retention.

## Key Questions Answered

1. **When do people shop?**
   - What time of day are groceries most commonly ordered?
   - Which day of the week sees the most activity?

2. **What do people buy?**
   - Which products are most popular overall?
   - What items are most frequently reordered?
   - What gets added to the cart first?

3. **How do people shop?**
   - How many items are in a typical order?
   - How long do customers wait between orders?
   - What proportion of products are reorders vs. new purchases?

## Dataset

The analysis uses five interconnected CSV files:

| Dataset | Description | Records |
|---------|-------------|---------|
| `instacart_orders.csv` | Order history with timestamps | ~479k orders |
| `products.csv` | Product catalog | ~50k products |
| `departments.csv` | Department categories | 21 departments |
| `aisles.csv` | Aisle classifications | 134 aisles |
| `order_products.csv` | Order line items | ~30M items |

**Note:** All CSV files use semicolon (`;`) as the delimiter instead of comma.

## Key Findings

### Shopping Patterns
- **Peak Hours**: Most orders occur between 9:00 AM - 5:00 PM, with peaks at 10:00 AM and 3:00 PM
- **Weekly Trends**: Orders concentrate at the beginning of the week (Sunday/Monday)
- **Reorder Frequency**: Most customers reorder within 7 days, with common patterns at 7, 14, 21, and 28 days

### Product Insights
- **Top Categories**: Fresh produce and dairy dominate both total orders and reorders
- **Basket Size**: Typical orders contain 5-6 items, with most orders having 1-20 items
- **First Additions**: Produce, dairy, and beverages are most commonly added to cart first

### Customer Behavior
- **Reorder Rate**: Customers show strong loyalty to specific products
- **Order Frequency**: Most customers place 1-10 orders in the dataset
- **Subscription Patterns**: Notable spike at 30-day intervals suggests subscription-based ordering

## Technologies Used

- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **matplotlib** - Data visualization
- **Jupyter Notebook** - Interactive analysis environment

## Repository Structure

```
eda-analysis-project/
│
├── README.md
├── requirements.txt
├── index.html
├── instacart-market-basket-analysis.ipynb
└── datasets/
    ├── instacart_orders.csv
    ├── products.csv
    ├── departments.csv
    ├── aisles.csv
    └── order_products.csv
```

## Getting Started

### Prerequisites

```bash
python 3.7+
```

### Running the Analysis

1. Clone this repository
2. Navigate to the project directory
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook instacart-market-basket-analysis.ipynb
   ```
5. Run all cells to reproduce the analysis

Alternatively, view the analysis directly in the HTML file without running any code.

## Analysis Sections

### Data Preparation
- Loading and exploring datasets
- Handling missing values
- Removing duplicates
- Data type conversions

### Exploratory Analysis
1. **Easy Tasks** - Basic distributions and patterns
2. **Medium Tasks** - Comparative analysis and product rankings
3. **Hard Tasks** - Advanced metrics including reorder proportions and basket composition

### Visualizations
- Time series plots for shopping patterns
- Bar charts for product rankings
- Histograms for distribution analysis
- Comparative visualizations for behavioral insights

## Business Applications

This analysis can inform:

- **Inventory Optimization**: Stock high-demand products during peak hours
- **Marketing Campaigns**: Time promotions for maximum engagement
- **Recommendation Systems**: Suggest products based on reorder patterns
- **Customer Segmentation**: Identify loyal vs. occasional shoppers
- **Subscription Services**: Design recurring order programs

## Methodology

### Data Cleaning
- Identified and handled missing values (product names, days_since_prior_order, add_to_cart_order)
- Removed duplicate entries while preserving data integrity
- Standardized text fields for consistent analysis

### Analysis Approach
- Grouped aggregations for summary statistics
- Temporal analysis for time-based patterns
- Product-level and customer-level metrics
- Comparative visualizations for insights

## Data Source

This analysis uses a subset of the Instacart Online Grocery Shopping Dataset 2017, which was made publicly available for research purposes.

## License

This project was completed as part of the TripleTen AI/ML Engineering program.

## Author

**Victor Foster**
- GitHub: [@vfoster-repo](https://github.com/vfoster-repo)
- LinkedIn: [Victor Foster](https://linkedin.com/in/vfoster-connect)
- Email: victorfoster@hotmail.com

## Acknowledgments

- TripleTen  AI/ML Engineering Program Sprint 3 "Exploratory Data Analysis"

---

If you found this project helpful, please consider giving it a star!