# AdventureWorks Cycles - Power BI Dashboard

 ### 📊 Project Overview 

This repository contains a Power BI report developed as part of a Business Intelligence Analyst course project for AdventureWorks Cycles, a fictional manufacturing company. The project involves transforming raw data into professional-quality reports and dashboards to track key performance indicators (KPIs), compare regional performance, analyze product-level trends, and identify high-value customers.

### Problem Statement

AdventureWorks Cycles, a fictional manufacturing company, requires a comprehensive Business Intelligence solution to enhance its decision-making processes. The company needs to transform raw data into insightful, actionable reports and dashboards that effectively track key performance indicators (KPIs), compare regional performance, analyze product-level trends, and identify high-value customers. 

The challenge lies in efficiently connecting, shaping, and modeling this data, followed by applying advanced DAX calculations and data visualizations to deliver a professional-quality, interactive Power BI dashboard. This solution must be robust enough to handle the dynamic and complex nature of the business, providing clear and accurate insights for strategic decision-making.

### 🚀 Key Features 

- __1 : Data Connection & Transformation__  
Automated Data Pipelines: Seamlessly connected to various data sources.  
Data Cleansing: Transformed raw data using Power Query to ensure accuracy.  
Advanced Shaping: Utilized techniques like pivoting, unpivoting, and merging to prepare data for analysis.

For creating new column for months short form following DAX expression was written;
       
        Month Short = 
        UPPER(
        LEFT(
        'Calendar Lookup'[Month Name], 3
        )  
Snap of new calculated column ,

![Snap_1](https://github.com/user-attachments/assets/fe308cd3-1aec-4942-9c12-daa48a648293)


- __2 :Building the Data Model__  
Star Schema Design: Created a robust relational model with fact and dimension tables.  
Relationship Management: Established primary and foreign key relationships to maintain data integrity.  
Optimized Filtering: Leveraged bi-directional filters and calculated columns to enhance data exploration. 
        
Snap of model view ,

![Snap_1](https://github.com/user-attachments/assets/53aff335-2fb9-44ed-b2be-daece254e600)

- __3 : DAX-Driven Insights__  
Custom Calculations: Developed calculated columns and measures with DAX for deeper insights.  
Time Intelligence: Implemented time-based functions to analyze historical trends and forecast future performance.  
Advanced DAX Functions: Used tools like CALCULATE, FILTER, and iterators to derive meaningful metrics.  

For calculating weekend orders following DAX expression was written;
       
        Weekend Orders = 
        CALCULATE(
        [Total Orders],
        'Calendar Lookup'[Weekend] = "Weekend" 
        )  

- __4 : Interactive Data Visualization__  
User-Centric Design: Crafted an intuitive dashboard layout for easy navigation and exploration.  
Dynamic Reports: Enhanced interactivity with slicers, bookmarks, and drillthrough options.  
Custom Visuals: Incorporated unique visuals to represent data effectively and engage users.  


Snap of Tooltips visuals ,

![Snap_1](https://github.com/user-attachments/assets/72a3186a-3deb-4a21-b823-1084a6a1c1c8)

Snap of cards visuals

![Snap_1](https://github.com/user-attachments/assets/89b4e8da-0a38-4fda-ab84-a308473e7e58)



 
 # 📸 Dashboard Snapshots (Power BI DESKTOP)

- __🌟 Executive Dashboard__
 
![Dashboard_upload](https://github.com/user-attachments/assets/af3f7755-b5a7-4238-abd8-0d7d959b880b)



- __🌍 Map__
 
![Dashboard_upload](https://github.com/user-attachments/assets/9b5dc801-f181-403e-954d-0089c553c54c)


- __📈 Product Details__
 
![Dashboard_upload](https://github.com/user-attachments/assets/57463f56-8b0e-47ea-994c-c1e00aab8fc8)



- __👥 Customers Details__
 
![Dashboard_upload](https://github.com/user-attachments/assets/e5b7404c-5094-456d-b747-cc47e713f869)


- __🌟 Decomposition Tree__
 
![Dashboard_upload](https://github.com/user-attachments/assets/3bd7095b-4849-4855-8bc7-e7c9bc3daa49)


- __🌟 Key Influencers__
 
![Dashboard_upload](https://github.com/user-attachments/assets/7a59d57d-f4f8-4adf-b31f-8262c69537a6)


# Insights

Following inferences can be drawn from the dashboard;

### [1] Ruben Suarez drove the most revenue  = $6483
Among all other customers in skilled manual role in 2022 Ruben Suarez drove the most revenue of $6483            

 ### [2] Some other insights about products
 
 1.1) Total orders for ﻿Road Tire Tube﻿ were ﻿213﻿
 
 1.2) Adjusted profit (260.00% increase) and Total profit (260.00% increase) both trended up between Monday, June 28, 2021 and Monday, June 27, 2022.
 
 1.3) Profit experienced the longest period of growth (+$25) between Monday, August 16, 2021 and Monday, February 7, 2022.


 __⚙️ Prerequisites__  
 
- [Power BI Desktop]([URL](https://www.microsoft.com/en-us/power-platform/products/power-bi/desktop))
 
