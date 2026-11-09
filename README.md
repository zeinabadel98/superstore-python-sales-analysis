# Superstore Sales & Profitability Analysis using Python

## Project Overview
I used Python to explore Superstore sales data and understand which products, regions, and customer segments generate revenue and profit. I also looked at discounting and loss-making products to find areas worth investigating.

## Business Questions
- Which category has the highest sales and profit?
- Which regions and customer segments drive the most sales?
- Which sub-categories are losing money?
- How do sales change over time?
- What is the relationship between discounts and profit?

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, and Jupyter/Google Colab.

## Dataset
The analysis uses the **Orders** sheet of `Sample - Superstore.xlsx`: **10,194 rows and 21 original columns**. The workbook also includes Returns and People sheets, which are not part of this analysis.

## What I Did
1. Loaded the Excel dataset and checked data types, missing values, duplicates, and sales outliers.
2. Cleaned text fields and removed exact duplicates, if any.
3. Created profit margin, shipping duration, and sales performance categories.
4. Explored sales and profit by category, region, segment, and sub-category.
5. Built charts for monthly trends, distributions, and correlations.
6. Calculated KPIs and exported the cleaned data.

## Key Findings
| Metric | Result |
|---|---:|
| Total Sales | $2,326,534.35 |
| Total Profit | $292,296.81 |
| Overall Profit Margin | 12.56% |
| Highest Sales Category | Technology ($839,893.28) |
| Highest Profit Category | Technology ($146,543.38) |
| Highest Sales Region | West ($739,813.61) |
| Highest Sales Segment | Consumer ($1,170,659.79) |

- **Furniture** generated $754,747.76 in sales but only $19,730.00 in profit.
- **Tables** lost $17,753.21, **Bookcases** lost $3,632.07, and **Supplies** lost $1,171.39.
- The correlation between discount and profit is approximately **-0.22**. This is an association, not proof that discounts cause losses.

## Recommendations
- Investigate pricing, discounting, and costs for loss-making sub-categories, especially Tables.
- Compare profit margins, not just sales, when reviewing category performance.
- Break down discounts by category and product before making pricing decisions.

## Files
- `Superstore_Sales_Analysis.ipynb` — analysis notebook
- `Sample - Superstore.xlsx` — source workbook
- `requirements.txt` — Python dependencies

## How to Run
1. Download the repository files.
2. Open the notebook in Google Colab or Jupyter Notebook.
3. Keep `Sample - Superstore.xlsx` in the same working folder as the notebook. In Colab, upload the Excel file to the session first.
4. Install dependencies with `pip install -r requirements.txt` if needed.
5. Run all notebook cells in order. The notebook creates `cleaned_superstore.csv` locally.

## Next Steps
Returns and regional manager data are available in separate workbook sheets and could be analyzed in a future extension.
