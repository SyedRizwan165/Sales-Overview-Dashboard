# Sales Overview Dashboard -MySQL-PowerBI

The purpose of this project is to enhance the sales reporting and follow-up processes for sales team by implementing visual dashboards using Power BI. These dashboards will leverage data from the CRM system and provide a comprehensive overview of internet sales. The project aims to improve sales performance monitoring and decision-making, facilitating more effective strategies for customer engagement and product promotion.

The dataset is taken from https://www.sendspace.com/file/z2s0gv

# Data Cleaning

To create the necessary data to prepare data model, data is first cleaned and transformed using SQl. One file i.e Sales Budget was recieved in excel format that was later connected in data model.

# Measures
Following Analytic measures were created using DAX

**Budget**
- Budget = SUM ( FACT_Budget[Budget] )

**Sales**
- Sales = SUM ( FACT_InternetSales[SalesAmount] )

**Sales / Budget**
- Sales / Budget = [Sales] - [Budget]

# Dashboard
The final dashboard consist of three files, sales, customer and product. The filters and slicers are placed by keeping the business request in mind. Multi dynamic KPI card have been used for the better visualization of Sales vs Budget comparison.

![image](https://github.com/SyedRizwan165/Sales-Overview-Dashboard/blob/main/1.png)
![image](https://github.com/SyedRizwan165/Sales-Overview-Dashboard/blob/main/2.png)
![image](https://github.com/SyedRizwan165/Sales-Overview-Dashboard/blob/main/3.png)
