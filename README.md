# Sales Performance Analytics Dashboard

This folder contains a simple analytics project for **sales performance**.  The data here is synthetic, but the structure reflects a typical multi‑region, multi‑product sales database.  It’s intended as a starting point for building a Power BI dashboard.

## Dataset (`sales_data.csv`)

The CSV file holds monthly records from **January 2023 to August 2025**.  Each row represents the sales of a specific product in a specific region for a given month.  Columns include:

| Column | Description |
|---|---|
| `Date` | Year‑month (YYYY‑MM) of the sales record. |
| `Region` | Geographic area (North, South, East, West or Central). |
| `Product` | The product sold (Product A, B, C or D). |
| `Sales` | Total revenue in euros for the product/region/month. |
| `Units` | Quantity of items sold. |
| `Profit` | Gross profit in euros (calculated from a random profit margin of 10–30 %). |

The synthetic data was generated with a normal distribution for sales and units so that results look realistic (average sales ~50 k€ per product/region/month).  To modify or refresh the dataset, open the Python script used to generate it in the notebook or write your own logic.

## Visualisations

Three PNG files illustrate how the data can be visualised:

| Image | What it shows |
|---|---|
| **`sales_trend.png`** | A line chart of total sales across all products and regions over time.  This helps spot seasonality and overall growth trends. |
| **`sales_by_region.png`** | A horizontal bar chart comparing total sales by region for the entire period. |
| **`sales_by_product.png`** | A horizontal bar chart comparing total sales by product. |

You can reproduce these charts or build richer dashboards using Power BI.  For example, import the CSV file via *Get Data → Text/CSV* and create:

1. **Line chart:** plot `Sales` over `Date`, optionally with slicers for region or product.
2. **Stacked column chart:** breakdown monthly sales by product or region.
3. **KPI cards:** show total revenue, average profit margin and total units sold.

Feel free to add measures such as year‑over‑year growth or profit margin ratio to explore the data further.