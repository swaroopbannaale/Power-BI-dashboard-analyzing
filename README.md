# Power-BI-dashboard-analyzing
Interactive Power BI dashboard analyzing AdventureWorksLT sales data with customer insights, geographic trends, and product performance metrics.

Business Problem
Build a comprehensive sales analytics dashboard connecting to AdventureWorksLT database, featuring:
- Customer segmentation analysis
- Geographic sales distribution (US states, cities)
- Product category performance tracking
- Target vs actual sales monitoring (2% growth target)

Data Sources
1. AdventureWorksLT Database (SQL Server)
   - Customers table (customer demographics & addresses)
   - Sales table (order details, quantities, pricing)
2. Wikipedia (Web scraping)
   - US State codes for geographic mapping

Key Features

Data Transformation
- Customers Table: Cleaned 7 fields; added FullAddress concatenation
- Sales Table: Created LineTotal calculation (OrderQty × ListPrice)
- States Data: Web-scraped US state codes; merged with sales data
- Measures: TargetSales (LineTotal + 2% growth)

Visualizations (2 Pages)

Page 1: Sales Performance
1. Gauge Chart: LineTotal vs TargetSales (max: $1.46M)
2. Pie Chart: Top Selling Companies by revenue
3. Stacked Bar: Sales by Main Category (500-unit threshold line)
4. Donut Chart: Category revenue distribution
5. Stacked Column: Top Selling Bikes (>$32K, filtered to bikes only, 35K threshold)

Page 2: Geographic Analysis
1. Map Visual: World Sales by City
2. US Map: Sales by State (YTD performance)
