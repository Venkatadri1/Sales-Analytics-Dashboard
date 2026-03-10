# power Bi
see the full dashboard here
https://app.powerbi.com/groups/me/reports/81e6e895-2ca2-4486-9557-26694f682e8b/58803e01706aba9aa751?experience=power-bi
**📊 Sales Analytics Dashboard**
**📌 Project Overview**
The Sales Analytics Dashboard project focuses on analyzing company sales data to identify key business insights such as sales trends, product performance, and regional sales distribution.
The dashboard was developed using Power BI to provide interactive visualizations that help businesses make data-driven decisions.

**🎯 Project Objectives**

Analyze company sales performance.
Identify top-selling products and profitable regions.
Track monthly and yearly sales trends.
Provide a visual dashboard for business insights.

**🛠 Tools & Technologies Used**
Excel – Data cleaning and preprocessing
Power BI – Data visualization and dashboard development

**📂 Dataset Information**
The dataset contains sales transaction details including:
Order Date,Product Name,Customer Name,Region / Country,Order Quantity,Unit Price,Discount,Sales Amount,Profit

**🔄 Data Processing Steps**
Cleaned and organized raw sales data using Excel.
Removed duplicates and handled missing values.
Used SQL queries to extract and transform the data.

Created calculated fields such as:
Total Sales,Profit,Year,Month,Quarter

**Imported the processed data into Power BI for visualization.**
**📈 Dashboard Features**
The dashboard includes the following insights:
Total Sales KPI,Total Profit KPI,Year-wise Sales Analysis,Monthly Sales Trend,Top 10 Products by Sales,Region-wise Sales Performance,Category-wise Sales Distribution

**🔍 Key Insights**
Identified the best-performing products based on total sales.
Analyzed seasonal sales trends across different months and years.
Determined regions generating the highest revenue.
Evaluated the relationship between discounts and profit margins.

**💼 Business Impact**
This dashboard helps stakeholders to:
Monitor overall sales performance
Identify high-performing products
Understand regional sales patterns
Make better strategic business decisions
**👨‍💻 Author**
Data Analyst | Excel | Power BI

**✅ Pro Tip:**
Also upload these files to GitHub:
Sales_Dataset.xlsx
Sales_Dashboard.pbix
README.md
screenshorts and pics

**Formulas**📱
Total Sales = SUM(shipments[Sales])
Total Profit = [Total Sales]-[Total Costs]
Profit % = DIVIDE([Total Profit],[Total Sales])
Last Mom Sales Change % = 
VAR ld= [Latest Date]
VAR this_mon_sales = [Total_Sales Latest Month]
VAR prev_Month_Sales = CALCULATE([Total Sales],'calendar'[Start of Month]= EDATE(ld,-1))
RETURN
DIVIDE(this_mon_sales-prev_Month_Sales,prev_Month_Sales)
Latest Date = LASTDATE('calendar'[Start of Month])
LBS % = DIVIDE([LBS Count],[Total Shipment])
LBS Count = CALCULATE([Total Shipment],shipments[Boxes]<50)
MOM Boxes change% = 
VAR this_month= [Total Boxes]
VAR prev_month=CALCULATE([Total Boxes],PREVIOUSMONTH('calendar'[Date]))
RETURN
DIVIDE(this_month-prev_month,prev_month)
MoM costs change % = 
VAR  this_month = [Total Costs] 
VAR prev_month = CALCULATE([Total Costs],PREVIOUSMONTH('calendar'[Date]))
RETURN
DIVIDE(this_month-prev_month,prev_month)
Mom profit changes % = 
 VAR this_month = [Total Profit]
VAR prev_month = CALCULATE([Total Profit],PREVIOUSMONTH('calendar'[Date]))
RETURN
DIVIDE(this_month-prev_month,prev_month)
Mom Sales change% = 
VAR this_month = [Total Sales]
VAR prev_Month = [Total Sales (Prev month)]
RETURN 
DIVIDE(this_month-prev_Month,prev_Month)
Mom shipment changes % = 
 VAR this_month = [Total Shipment]
VAR prev_month = CALCULATE([Total Shipment],PREVIOUSMONTH('calendar'[Date]))
RETURN
DIVIDE(this_month-prev_month,prev_month)



  
