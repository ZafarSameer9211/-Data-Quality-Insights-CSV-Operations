# -Data-Quality-Insights-CSV-Operations
## Project Overview
This project cleans a raw sales dataset (`sales_raw.csv`) with Pandas, analyzes revenue by region and category, and then edits the cleaned file.

- **Part A (70 marks):** load, inspect, clean, calculate revenue, groupby summaries, two charts, two findings, save `cleaned_sales.csv`
- **Part B (30 marks):** add `tax_amount`, update Books prices, remove a row, add and drop a temporary column, save `sales_updated.csv`

## Files
| File | Description |
|---|---|
| `Sunday_Project.ipynb` | Notebook with Part A and Part B |
| `sales_raw.csv` | Original input (never modified) |
| `cleaned_sales.csv` | Output of Part A |
| `sales_updated.csv` | Output of Part B |
| `chart_revenue_by_region.png` | Chart 1 |
| `chart_revenue_by_category.png` | Chart 2 |

## How to Run

### Option 1: Jupyter Notebook
1. Put all files in one folder.
2. Install the libraries: `pip install pandas matplotlib jupyter`
3. Run `jupyter notebook` and open `Sunday_Project.ipynb`.
4. Click **Kernel > Restart & Run All**.

### Option 2: Google Colab
1. Open `Sunday_Project.ipynb` in Colab.
2. Upload `sales_raw.csv` using the Files panel on the left.
3. Click **Runtime > Run all**.

The notebook uses relative paths, so no path changes are needed.

## Cleaning Rules
- Trimmed spaces and standardized text case in `region` and `category`
- Filled the missing region with `Unknown`
- Removed duplicate rows
- Removed rows with missing, invalid, or negative `quantity` or `unit_price`
- Removed one extreme price outlier
- Rows: 21 before cleaning, 15 after cleaning

## Key Findings
1. North is the top region, with about 31% of total revenue.
2. Books earn the most of any category, about 50% of total revenue.

## Tools Used
Python, Pandas, Matplotlib
