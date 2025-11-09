# 📊 Sales Analysis Dashboard Project USA

## Project Overview

This repository showcases a comprehensive **Sales Analysis Dashboard** designed to provide actionable insights into sales performance, profitability, and trends across various dimensions. The dashboard allows users to dynamically filter and analyze sales data by **Category, Person (Sales Rep), Ship Mode, City, and Time (Year/Month)**.

The primary goal of this analysis is to identify top-performing areas, potential weaknesses, and significant sales drivers to inform business strategy and operational efficiency.

📂 Download `.pbix` file and open it with **Microsoft Power BI Desktop**.  
👉 [Download USA_Sales_Analysis_dashboard.pbix](https://github.com/sujithts31618-ui/Sales_Analysis_Performance_USA/blob/main/USA_Sales_Analysis_dashboard.pbix?raw=true)


---

## Key Features & Insights

The dashboard is structured into several interconnected views, providing a multi-layered analysis:

## 📊 Report Snapshot (Power BI DESKTOP)
1.
![Bike Sales Dashboard 1](https://raw.githubusercontent.com/Sujithts12/Power_BI_Bike_sales/main/Screenshot%202025-08-13%20193424.png)
2.
![Bike Sales Dashboard 2](https://raw.githubusercontent.com/Sujithts12/Power_BI_Bike_sales/main/Screenshot%202025-08-13%20193457.png)
3.
![Bike Sales Dashboard 3](https://raw.githubusercontent.com/Sujithts12/Power_BI_Bike_sales/main/Screenshot%202025-08-13%20193520.png)
4.
![Bike Sales Dashboard 4](https://raw.githubusercontent.com/Sujithts12/Power_BI_Bike_sales/main/Screenshot%202025-08-13%20193545.png)
5.
![Bike Sales Dashboard 5](https://raw.githubusercontent.com/Sujithts12/Power_BI_Bike_sales/main/Screenshot%202025-08-13%20193653.png)
6.
![Bike Sales Dashboard 6](https://raw.githubusercontent.com/Sujithts12/Power_BI_Bike_sales/main/Screenshot%202025-08-13%20193728.png)



### 1. Sales Performance Summary (Report View)

* **Total Sales & Total Profit:** Headline figures for the selected filters.
* **Sales YoY (%):** Year-over-Year growth percentage to assess performance trajectory.
* **Revenue by Month:** A bar chart illustrating the monthly sales trend to identify peak seasons and troughs.
* **Revenue by City:** A ranked list of cities by revenue, highlighting the most lucrative urban markets.
* **Category Performance Summary:** Text summaries that quantify category contributions and sales ranges.

### 2. Detailed Breakdown Analysis (Drill-Down View)

This view uses a flow diagram visualization to show the volume of sales through different hierarchical levels.

* **Hierarchy:** The breakdown follows the sequence: **Category → Sub-Category → Ship Mode → State**.
* **Insight:** It clearly illustrates how sales flow (e.g., from the **Furniture** category to **Standard Class** shipping in **California**), which is vital for understanding logistics and inventory demands.

---

## Dynamic Filtering

The dashboard supports extensive filtering to enable granular analysis:

| Filter Dimension | Purpose | Examples from Snapshots |
| :--- | :--- | :--- |
| **Year** | Compare performance across different years. | 2014, 2015, 2016 |
| **Category** | Focus on specific product groups. | Furniture, Office Supplies, Technology |
| **Person** | Evaluate the performance of individual sales representatives. | Kelly Williams, Magee, Cassandra Brand |
| **Ship Mode** | Analyze the impact of different shipping methods on sales. | First Class, Same Day, Second Class, Standard Class |

---
## 🧩Few of the DAX Queries used
- **Total Sales = Sum ('orders'[Sales])
- **Sales LY = CALCULATE (SUM ('Orders'[Sales]), SAMEPERIODLASTYEAR(DateTable[Date]))
- **Sales YoY % = DIVIDE([Total Sales]-[Sales LY],[Sales LY],0)
- **Calender_table = 
ADDCOLUMNS (
    CALENDAR (DATE(2014,1,1), DATE(2016,12,31)),
    "Year", YEAR([Date]),
    "Month Number", MONTH([Date]),
    "Month Name", FORMAT([Date], "MMMM"),
    "Month Short", FORMAT([Date], "MMM"),
    "MonthYear", FORMAT([Date], "MMM-YYYY"),
    "Quarter", "Q" & FORMAT([Date], "Q")
)
## Technologies Used

* **Visualization Tool:** [**Power BI**]
 
## 👨‍💻 Author
*Dashboard Created By:* Sujith TS 

*Date:* 9th November 2025


## 🎥 [Watch the interactive video demo on LinkedIn] 
 - Link : 
 [https://l1nk.dev/pHWeS](https://www.linkedin.com/posts/sujith-siddarth-514830208_powerbi-microsoftpowerbi-powerbidashboard-activity-7393243627050864640-GmtL?utm_source=share&utm_medium=member_android&rcm=ACoAADTN1eABJYc0svIfomu6QfBYptguHuLDHic)
----------------------------------------------------------------------------------------------------
