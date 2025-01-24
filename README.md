# Big Mart Sales Analysis

## **Introduction**
In our journey to understand sales performance and uncover key drivers of growth, we delved into a comprehensive analysis of Big Mart’s product and outlet data. We started by examining top-selling products and pricing strategies to identify patterns that influence revenue. Our focus on visibility and item categories helped highlight actionable areas for optimizing sales potential. 

Next, we shifted to outlet-level insights, exploring how size, type, and location impact overall sales performance. By comparing outlet sales trends, we revealed high-performing segments and pinpointed underutilized opportunities. This data-driven approach equips us with the knowledge to enhance business strategies, improve product placement, and fine-tune pricing for sustained growth.

- BigMart Sales [Dataset](https://github.com/NishaChandila/BigMart-Sales-Prediction/blob/main/Train.csv)
- BigMart Sales [Power Bi Dashboard](https://github.com/NishaChandila/BigMart-Sales-Prediction/blob/main/Bigmart-sales-dashboard.pdf)
- BigMart Sales [Python EDA](https://github.com/NishaChandila/BigMart-Sales-Prediction/blob/main/BigMart-Sales-Prediction.ipynb)

---

## **Data Structure**
The dataset provides a detailed view of product and outlet-level attributes, enabling a comprehensive analysis of sales trends, pricing strategies, and outlet performance. Each column represents a specific aspect of the business, contributing to actionable insights.

![Dataset](https://github.com/NishaChandila/project-assets/blob/main/Bigmart-sales-dataset.PNG)

### Columns in the Dataset:
- **Item_Identifier**: Unique code for each product.
- **Item_Weight**: Weight of the product, reflecting size and shipping needs.
- **Item_Fat_Content**: Categorizes products as Low Fat or Regular.
- **Item_Visibility**: Percentage of display area for each product.
- **Item_Type**: Product category, such as Snack Foods or Dairy.
- **Item_MRP**: Maximum Retail Price, indicating product pricing.
- **Outlet_Identifier**: Unique code for each outlet location.
- **Outlet_Establishment_Year**: Year the outlet was established.
- **Outlet_Size**: Size of the outlet (Small, Medium, High).
- **Outlet_Location_Type**: Geographic tier of the outlet (Tier 1, Tier 2, Tier 3).
- **Outlet_Type**: Type of outlet, like Supermarket or Grocery Store.
- **Visibility Category (Derived)**: Classifies products into High, Medium, and Low visibility.
- **Price Range (Derived)**: Groups products into price segments.

This structure provides a clear view of sales drivers, pricing, and outlet performance.

- BigMart Sales [Dataset](https://github.com/NishaChandila/BigMart-Sales-Prediction/blob/main/Train.csv)

---

## **Executive Summary**

![Home](https://github.com/NishaChandila/project-assets/blob/main/Bigmart-sales-dashboard1.PNG)

The Power BI dashboard is structured across two pages, providing valuable insights into both sales performance and outlet dynamics.

### **Page 1: Top Sellers and Pricing Insights**

![Top](https://github.com/NishaChandila/project-assets/blob/main/Bigmart-sales-dashboard2.PNG)

- **Total Sales**: The total sales value is **2M**, providing a comprehensive view of overall sales across all items.
- **Top-Selling Item**: **Snack foods** and **fruits & vegetables** are the highest-selling items, each with sales of approximately **0.29M**.
- **Average Price**: The **average price** is **141**, offering insights into pricing trends across items.
- **Sales by Item Type**: Snack foods lead in sales with **0.29M**, followed by fruits & vegetables at **0.29M**, while dairy has the lowest sales at **0.17M**.
- **Visibility Impact on Sales**: **High visibility** items account for **91.47%** of total sales, while low visibility items contribute **6.66%**.

### **Page 2: Outlet Insights**

![Outlet](https://github.com/NishaChandila/project-assets/blob/main/Bigmart-sales-dashboard3.PNG)

- **Total Outlets**: There are **10 total outlets**, giving a view of the outlet network and its spread.
- **Outlet with Highest Sales**: The outlet with the highest sales is **OUT027**, contributing significantly to overall revenue.
- **Average Outlet Size**: The average outlet size is categorized as **medium**, indicating the size distribution across the network.
- **Sales by Outlet Type**: **Supermarket Type 1** has the highest sales at **1,311K**, while **Supermarket Type 2** has the lowest at **218K**.
- **Outlet Size and Location Analysis**: Medium-sized outlets generate the highest sales at **0.66M**, while high-sized outlets have the lowest at **0.22M**. Additionally, outlet distribution shows **4.6K medium outlets** and **1.5K high outlets**.

This dashboard layout delivers a clear picture of both product performance and outlet insights, helping guide decisions to improve sales strategies and optimize outlet performance.

- BigMart Sales [Power Bi Dashboard](https://github.com/NishaChandila/BigMart-Sales-Prediction/blob/main/Bigmart-sales-dashboard.pdf)

---

## **EDA in Python**

In our exploratory data analysis (EDA) phase, we focused on understanding the dataset's structure and identifying key insights for building the model.

### Key Steps in the EDA Process:
1. **Data Distribution**: We visualized the distribution of numeric columns using histograms, KDE plots, and violin plots. These helped reveal patterns and outliers, guiding us in data cleaning.
2. **Categorical Insights**: We analyzed categorical columns, including **Item_Fat_Content**, **Item_Type**, and **Outlet_Size**, using count plots and pie charts. This showed the distribution of various categories and allowed us to handle missing values.
3. **Missing Data Handling**: For missing data, we imputed categorical columns (e.g., **Outlet_Size**) with the mode and numeric columns (e.g., **Item_Weight**) with the mean.
4. **Outlier Detection and Removal**: We identified and removed outliers in the **Item_Visibility** and **Item_Outlet_Sales** columns using the IQR method, improving data integrity.
5. **Encoding**: Ordinal columns such as **Item_Fat_Content** and **Outlet_Type** were label-encoded, while **Item_Type** and other categorical features were one-hot encoded to prepare for machine learning.

This EDA process helped refine the dataset, making it ready for modeling by addressing missing values, outliers, and encoding categorical data effectively.

- BigMart Sales [Python EDA](https://github.com/NishaChandila/BigMart-Sales-Prediction/blob/main/BigMart-Sales-Prediction.ipynb)

---

## **Recommendation**
- **Focus on High-Selling Products**: Snack foods and fruits & vegetables, which each contribute **0.29M** in sales, should be prioritized for restocking, promotions, and marketing to sustain strong performance.
- **Optimize Pricing Strategy**: With an average item price of **141**, it’s important to review and maintain competitive pricing for top-performing items while considering price adjustments for lower-performing ones.
- **Increase Visibility for Low Visibility Items**: High visibility items contribute **91.47%** of total sales. Improving visibility for low visibility items (**6.66%**) could unlock additional sales opportunities.
- **Expand Medium-Sized Outlets**: Medium-sized outlets show the highest sales (**0.66M**). Expanding more medium-sized outlets could potentially drive higher overall sales across the network.
- **Leverage Successful Outlets**: Outlet **OUT027**, which has the highest sales, can be used as a model to replicate its strategies in other outlets to boost overall performance.
- **Reevaluate Outlet Types and Locations**: **Supermarket Type 1** performs significantly better in sales than **Supermarket Type 2**. A more targeted strategy for Type 2 outlets could help improve their performance, while further expanding Type 1 outlets could increase total revenue.

These recommendations will help optimize product and outlet performance, ultimately contributing to higher sales and better strategic decisions.

- BigMart Sales [Dataset](https://github.com/NishaChandila/BigMart-Sales-Prediction/blob/main/Train.csv)
- BigMart Sales [Power Bi Dashboard](https://github.com/NishaChandila/BigMart-Sales-Prediction/blob/main/Bigmart-sales-dashboard.pdf)
- BigMart Sales [Python EDA](https://github.com/NishaChandila/BigMart-Sales-Prediction/blob/main/BigMart-Sales-Prediction.ipynb)

---
