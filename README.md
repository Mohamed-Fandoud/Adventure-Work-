# Adventure Works Power BI Dashboard Project

This Power BI project is a comprehensive analysis of **Adventure Works** sales data, focusing on customer behavior, sales performance, and product profitability. The project covers data from 2020 to 2022 and includes advanced data transformation, modeling, and visualization techniques.

## Project Objective

The goal of this dashboard is to provide key insights into Adventure Works' sales performance across various dimensions such as products, customers, and regions. This project aims to help stakeholders make data-driven decisions to improve business outcomes by analyzing trends, comparing KPIs, and exploring customer demographics.

## Tools and Technologies Used

- **Power BI Desktop** (Version: Latest)
- **DAX** (Data Analysis Expressions) for creating custom measures.
- **Power Query** for data transformation and cleansing.
- **Star Schema Modeling** for optimized query performance.
- **Field Parameters** for dynamic visuals.
- **Custom Visuals** for advanced charting.

## Datasets Used

The following CSV files were imported and transformed to build the data model:
- **Calendar Lookup**
- **Customer Lookup**
- **Product Lookup**
- **Product Categories Lookup**
- **Product Subcategory**
- **Territory Lookup**
- **Return Data**
- **2020 Sales Data**
- **2021 Sales Data**
- **2022 Sales Data**

## ETL Process (Extract, Transform, Load)

### Data Transformation:
1. **Calendar Table Enhancements**:
   - Extracted fields: `Year`, `Month`, `Start of Week`, `Start of Month`, `Start of Quarter`.
2. **Customer Table Refinement**:
   - Merged `First Name` and `Last Name` to create a full name.
   - Added a conditional column to distinguish between parent and non-parent customers.
   - Standardized `Marital Status` and `Gender` by replacing abbreviations with full words.
   - Removed null values for cleaner data.
3. **Product and Lookup Tables**:
   - Ensured correct data types for consistency.
4. **Sales Data Consolidation**:
   - Merged the 2020, 2021, and 2022 sales data into a single fact table: **Total Sales**.

### Data Model:
The data model follows a **star schema**, where **Sales** and **Return** act as fact tables, connected directly to dimension tables like Customer, Product, and Calendar in one-to-many relationships. This schema ensures high query performance and simplicity in analyzing data.

![Data Model View](https://github.com/user-attachments/assets/5c463552-ff63-435d-a8a0-7c98646709f8)

## Performance Optimization

- **Calculated Columns vs. Measures**: Used DAX measures for performance improvements by avoiding unnecessary storage of calculated values.
- **Data Type Consistency**: Ensured optimized model performance through correct data types across tables.
- **Dynamic Filtering**: Incorporated **date** and **country filters** for faster, relevant querying of data.

## Dashboard Highlights

The dashboard is designed to be fully interactive with dynamic filtering options, providing key insights across four major pages:

### 1. **Overview Page**:
   - **KPIs**: Total Revenue, Profit, Orders, and Return Rate.
   - **Weekly Line Chart** to track revenue trends.
   - **Monthly Orders and Revenue Comparison** against the previous month.
   - **Top 10 Products Metrics Table**, with drill-through to the product details page.

   ![Overview Page](https://github.com/user-attachments/assets/052c5e9b-aa06-47be-8de2-278ecc2c1ef8)

### 2. **Geographical Analysis (Map Page)**:
   - Displays orders by country and city, providing a geographical view of sales distribution.

   ![Map Page](https://github.com/user-attachments/assets/29dc6a03-daf1-4c24-b6f8-5a6fdc92f202)

### 3. **Product Performance Page**:
   - **Gauges** showing monthly revenue, profit, and orders vs. target.
   - **Line Chart** comparing actual vs. adjusted profit (based on adjusted price ranges).
   - **Comprehensive Line Chart** showing revenue, profit, orders, costs, returns, and return rate.

   ![Product Page](https://github.com/user-attachments/assets/ded40a64-5759-495b-a8fe-d3b692212304)

### 4. **Customer Analysis Page**:
   - **KPIs**: Customer Count and Revenue per Customer.
   - **Line Chart** with field parameters for viewing total customers and revenue per customer trends.
   - **Pie Charts** displaying customer occupation and education levels.
   - **Top 100 Customers Metrics**, with detailed insights on top customers.
   - **Highlight Card** showcasing the top customer by revenue, along with their order count and total revenue.

   ![Customer Page](https://github.com/user-attachments/assets/27000ab5-3410-4269-be2d-6b99d5911248)

## Custom Measures

A dedicated **Measures Table** was created to support advanced calculations, including:
- **Total Sold Units**, **Total Revenue**, **Total Profit**, **Total Orders**.
- **Revenue per Customer**, **Return Rate**, **Profit Margin**, **Revenue and Profit Targets**.
- **Previous Month Orders and Revenue**, **Overall Average Retail Price**.
- **Adjusted Revenue and Profit**, **Order Gap Target**, **Order Target**.
- **Percentage of Profit**, **Percentage of Orders**, **Total Orders by Parent Customers**.

## Future Improvements

- **Real-time Data Integration**: Integrating real-time data sources for more up-to-date insights.
- **Predictive Analytics**: Adding machine learning models for sales forecasting.
- **Expanded Datasets**: Incorporating more dimensions such as marketing spend or customer satisfaction data.

## Contact

For further inquiries or collaboration, feel free to reach out:

**Email**: mohamedelsayedfandoud@gmail.com

---

This dashboard highlights my expertise in transforming raw data into actionable insights through Power BI. It showcases advanced data modeling, dynamic visualizations, and interactive features that enable users to make informed business decisions.
