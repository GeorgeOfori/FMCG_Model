# FMCG_Model
## Overview
 A company called Drinco, which operates in the Fast Moving Consumer Goods (FMCG) industry. It involves in the production and sale of non-durable goods, such as soft drinks, toiletries, processed foods, and other consumable products. It is a business known for its high volumes and margins.
 
### Objective:
To build a model that allows the company management to view the volumes sold, the revenue generated, and the margins obtained, with breakdowns by month, client, client type, brand, size, and pack.

### Data Extraction and Acquisition
•	SAP Business Objects to extract data from ERP systems, downloaded into Excel for analysis.

•	The data extraction includes descriptive fields (material number, brand, client,period, client type, ) and financial information ( volume, gross sales, discounts, net sales, costs of sales, distribution, warehousing).

•	The extraction displayed here contains 88,000 rows and spans 17 columns. 

![image](https://github.com/user-attachments/assets/3d9e8194-60a5-4aa9-99e1-84246df0ced2)


### Creating a Master Pivot Table: The main data source for the FMCG report
•	We add the Year field to the table's columns area. This separates the data for the two years.

•	We  also add the Month field, placing it below Year in the columns area.

•	For the rows of the table, We would like to show the quantity we had for each of the brands in our database. Therefore, we drag the Brand field and place it in the Rows area.

•	Then we populate the table with data from the fields Volume, Gross Sales, Discounts, Net Sales, Cost of Goods Sold, Distribution, and Warehousing.


![image](https://github.com/user-attachments/assets/2d7da2b0-29fa-4257-b761-b7739b609c85)

### Creating an Output Structure, Inserting Formulas and Automating Calculations of the FMCG Model
•	The report structure includes two years of data: 2015 and 2016.

•	Volume sold is a key driver for FMCG businesses and is placed at the top of the report.

•	Financial measures include Gross Sales Income, Discounts, Net Sales, Cost of Goods Sold, Gross Profit, Distribution, and Warehousing expenses.

•	Full Delivered Margin is a profitability measure accounting for production, warehouse, and transportation costs.

•	Including columns for absolute and percentage variance alongside KPIs provides deeper insights into data analysis.

### Extracting data from the Master Pivot Table
The next stage is to fill out the output sheet. Our goal here is to extract data from the Pivot Table and populate the cells of the output sheet. We use excel function GETPIVOTDATA to populate the output sheet. 

![image](https://github.com/user-attachments/assets/f06f47d9-75ef-4a29-b6c6-0e33fe0665c3)

### Adding Slicers
We added slicers to the output. We select Month, Brand, Size, Pack Client, and Client Type. Below is the final output.


![image](https://github.com/user-attachments/assets/92780a1f-7e65-435c-96e5-143167ff1d0a)

### Key Insights
• Volume dropped by 6.9% (−4,101 units), from 59,838k to 55,736k. This volume decline likely reflects reduced market demand, customer loss, or possible price-driven churn.The volume contraction is a leading cause behind the -5.3% drop in Gross Sales and -5.1% drop in Net Sales.We have to investigate product or regional drivers of volume decline. Could pricing, competition, or distribution changes be affecting demand?

• Discounts dropped by 8.6% (a reduction of $311k), which is typically a good sign (less margin erosion). However, Gross Sales still fell by $2.95M, showing that the sales drop is not primarily due to higher discounting.

• Gross Profit dropped by $2.27M (-9.3%), while Cost of Goods Sold improved slightly (lower by $375k). Gross Margin declined from 46.7% to 44.6%, a 2.1 percentage point reduction.

• FDM dropped from $22.3M to $20.1M, a $2.24M loss, which is sharper than the net sales drop (-5.1%). FDM % also fell from 42.9% to 40.7%, confirming profitability is being squeezed even after gross margin—particularly due to rising distribution costs and fluctuating warehousing expenses. Distribution are eroding overall profitability. Even minor increases in cost here have big impact given low-margin nature of FMCG.

•  Distribution costs increased by 2.3% ($31k) even though volume declined by 6.9%. Warehousing costs dropped by 10.7% ($59k), which helped—but not enough to offset the squeeze. Distribution inefficiency is emerging. With lower volumes, costs should have decreased—not increased.


### Recommendation

##### Launch a Targeted Volume Recovery Plan

 • We should identify and reactivate underperforming customer segments using targeted promotions or product bundling.

 • Partner with the commercial/sales team to review client churn, shelf space, and retail presence.

 • Consider small-pack offerings or price restructuring to regain price-sensitive consumers without increasing discount spend.

#### Optimize Distribution Strategy to Protect Margin

 • Conduct a route and logistics efficiency review—optimize delivery schedules, load planning, or third-party logistics contracts.

 • Consider consolidating shipments or revisiting delivery frequency per customer segment.

 • Introduce performance KPIs for distribution partners (e.g., cost per unit, on-time delivery vs. cost trade-off).

 
