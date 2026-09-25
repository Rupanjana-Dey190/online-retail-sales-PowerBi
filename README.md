# Online Retail Sales Analytics Dashboard

An interactive **Power BI sales analytics project** built using the UCI Machine Learning Repository's **Online Retail** dataset. The project transforms transaction-level e-commerce data into an interactive dashboard for monitoring sales, order activity, quantity sold, customers, product performance, country-level sales, and sales trends over time.

## Dashboard Preview

> Add your Power BI dashboard screenshot here as `docs/dashboard.png`.

[📊 Click here to view the Power BI Dashboard Screenshot](Screenshot%202026-09-25%20122427.png)
## Project Objective

The objective of this project is to analyze online retail transactions and build an interactive business intelligence dashboard that helps users explore:

- Overall sales performance
- Transaction/order activity
- Quantity sold
- Customer activity
- Sales trends over time
- Sales by country
- Top-performing products
- Geographic sales contribution

## Dataset

**Source:** UCI Machine Learning Repository — Online Retail

The dataset contains transactions from a UK-based non-store online retailer. The company primarily sells unique all-occasion giftware, and many customers are wholesalers.

**Official source:**  
https://archive.ics.uci.edu/dataset/352/online+retail

**Dataset DOI:** `10.24432/C5BW33`

**License:** Creative Commons Attribution 4.0 International (CC BY 4.0)

### Dataset period

**1 December 2010 – 9 December 2011**

### Original variables

| Variable | Description |
|---|---|
| InvoiceNo | Transaction/invoice number |
| StockCode | Product code |
| Description | Product description |
| Quantity | Quantity of items in the transaction |
| InvoiceDate | Transaction date and time |
| UnitPrice | Unit price in sterling |
| CustomerID | Customer identifier |
| Country | Customer country |

The project adds a calculated **Sales** field:

`Sales = Quantity × UnitPrice`

## Dataset Snapshot

| Metric | Value |
|---|---:|
| Transaction rows | 541,909 |
| Unique invoice numbers | 25,900 |
| Countries | 38 |
| Unique products/descriptions | 4,223 |
| Non-null customer records | 406,829 |
| Unique customer IDs | 4,372 |
| Total quantity | 5,176,450 |
| Calculated sales | £9,747,747.93 |
| Date range | Dec 2010 – Dec 2011 |

> Note: These figures are calculated from the supplied workbook before additional business-rule filtering. The dashboard's displayed values depend on the aggregations and filters configured in Power BI.

## Power BI Dashboard

### KPI Cards

The dashboard includes:

- **Total Sales**
- **Transaction/Invoice Count**
- **Total Quantity Sold**
- **Customer Records**

### Visualizations

1. **Sales Trend Over Time** — Line chart
2. **Sales by Country** — Bar chart
3. **Top Products by Sales** — Bar chart
4. **Product Sales Comparison** — Column chart
5. **Sales Share by Country** — Pie chart

### Interactive Filters

- **Country slicer**
- **Invoice Date slicer**

The slicers allow the user to explore the dashboard dynamically by geography and time period.

## Data Preparation

The main calculated field used in the dashboard is:

```text
Sales = Quantity × UnitPrice
```

This converts transaction-level quantity and price information into a monetary sales measure.

The original dataset also contains cancelled transactions and negative quantities/prices in some records. These are retained in the supplied source workbook unless additional filtering is explicitly applied in Power BI.

## Repository Structure

```text
Online-Retail-Sales-PowerBI/
│
├── README.md
│
├── data/
│   └── Online_Retail.xlsx
│
├── powerbi/
│   └── Online_Retail_Sales_Dashboard.pbix
│
└── docs/
    └── dashboard.png
```

## Tools & Technologies

- **Power BI Desktop**
- **Microsoft Excel**
- **DAX**
- Data visualization
- Business intelligence
- Exploratory data analysis

## Key Skills Demonstrated

- Data importing and preparation
- Calculated columns/measures
- DAX
- KPI development
- Interactive dashboard design
- Time-series sales analysis
- Product performance analysis
- Geographic analysis
- Slicers and interactive filtering
- Business-oriented data storytelling

## How to Use

1. Download or clone this repository.
2. Open:
   `powerbi/Online_Retail_Sales_Dashboard.pbix`
3. If Power BI asks for the source file, point it to:
   `data/Online_Retail.xlsx`
4. Open the report in **Power BI Desktop**.
5. Use the **Country** and **Invoice Date** slicers to explore the dashboard.

## Data Source & Attribution

This project uses the **Online Retail** dataset provided by the UCI Machine Learning Repository.

Chen, D. (2015). *Online Retail* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5BW33

The original dataset is associated with:

Chen, D., Sain, S. L., & Guo, K. (2012). Data mining for the online retail industry: A case study of RFM model-based customer segmentation using data mining. *Journal of Database Marketing & Customer Strategy Management, 19*(3), 197–208. https://doi.org/10.1057/dbm.2012.17

## Disclaimer

This is an educational and portfolio project. The dashboard is intended to demonstrate data analytics and Power BI skills and should not be interpreted as an official report of the original retailer.

## Author

**Rupanjana Dey**

Economics Student | Data Analytics | Power BI | Python | Machine Learning

