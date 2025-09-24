summary:

1. Load Dataset – Import Superstore.csv into Power BI.


2. Create Measures – Define DAX measures:

Total Sales = SUM('Orders'[Sales])

Total Profit = SUM('Orders'[Profit])

Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)

Total Quantity = SUM('Orders'[Quantity])

Average Discount = AVERAGE('Orders'[Discount])

Monthly Sales = CALCULATE(SUM('Orders'[Sales]), DATESMTD('Orders'[Order Date]))

Top Customers Sales = RANKX(ALL('Orders'[Customer Name]), [Total Sales], , DESC, Skip)



3. Build Visuals – Use cards, tables, line/column charts with these measures.


4. Format & Export – Adjust visuals and export dashboard as PDF.



