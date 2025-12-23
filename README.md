# business-KPIS-analysis
🎯 **Business Insights & KPI Analysis Project**  This project goal is to analyze retail transaction data to compute business metrics, derive actionable insights, and create visualizations.
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-red)
![Matplotlib](https://img.shields.io/badge/Matplotlib-New-red)

**Features:**
- Calculate 13+ key business metrics from retail transaction data
- Implement derived columns (Sales, City, Month extraction)
- Generate automated visualizations and tables

## 📊 Dataset Description 

| Column | Description |
|--------|-------------|
| Order ID | Unique identifier for each order |
| Product | Name of purchased product |
| Quantity Ordered | Number of units purchased |
| Price Each | Price per unit (USD) |
| Order Date | Date and time of order |
| Purchase Address | Customer's full address |

### ⚠️ Important Notes:
1. **Column order matters**: The first column must be `Order ID`, the second must be `Product`, etc.
2. **Works with any dataset size** (tested with 185,950+ records)
   
## 🛠️ Business Insights Calculated

### Core Metrics
1. **Total Revenue** - Sum of all sales
2. **Unique Products** - Count of distinct products
3. **Total Units Sold** - Sum of all quantities
4. **Total Orders** - Count of unique Order IDs
5. **Average Order Value (AOV)** - Revenue per order
6. **Order Value Statistics** - Median, Min, Max per order

### Product Analysis
7. **Top 10 Products by Quantity**
8. **Top 10 Products by Revenue**
9. **Bottom 5 Products by Quantity**
10. **Highest Revenue per Unit Products**
11. **Product-level Descriptive Statistics**

### Temporal & Geographic Analysis
12. **Average Sales per Month**
13. **Sales by City**
### 3 derived columns
- 🧮 **Automatically calculates 3 derived columns**: Sales (Quantity×Price), City (from address), Month (from date)

## 🔍 Explore the Data

To better understand how the analysis works, we've included **both raw and processed datasets**:

| File | Records | Description | Purpose |
|------|---------|-------------|---------|
| `data/sales_data.csv` | 185,950 | **Original dataset** before processing | See input structure |
| `data/processed_sales_data.csv` | 185,950 | **Dataset after all operations** | Check derived columns & calculations |

### **📖 How to Use These Files:**
1. **Open `sales_data.csv`** to see the original 6-column structure
2. **Open `processed_sales_data.csv`** to see:
   - The 3 derived columns added (Sales, City, Month)
   - All data cleaned and formatted
   - Ready-to-use data for KPI calculations

### **💡 Pro Tip:**
Compare both files side-by-side to understand exactly how:
- `Sales` = `Quantity Ordered` × `Price Each`
- `City` is extracted from `Purchase Address`
- `Month` is extracted from `Order Date`

**👉 Please check these datasets to understand the data transformation process!**
