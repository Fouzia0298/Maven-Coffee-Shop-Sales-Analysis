# ☕Maven-Coffee-Shop-Sales-Analysis
## Project Overview
This project provides a comprehensive analysis of sales transactions from **Maven Roasters**, a fictitious coffee shop chain operating across three locations in New York City (Lower Manhattan, Hell's Kitchen, and Astoria). The goal was to explore the dataset, perform data quality assurance, analyze sales trends using Excel PivotTables, and build an interactive dashboard to derive actionable insights and recommendations for the business.

![Dashboard Screenshot](https://github.com/Fouzia0298/Maven-Coffee-Shop-Sales-Analysis/blob/main/coffee%20sales%20dashboard.PNG)

The analysis covers sales performance over time, identifies peak hours and days, and evaluates product-level trends to optimize sales strategies, improve operational efficiency, and enhance customer satisfaction.

## Objectives

This project was structured around three main objectives:

### 1. Data Preparation and QA
- Explore the raw `Transactions.csv` dataset.
- Conduct basic data quality assurance (QA) and profiling to identify and address any errors or inconsistencies.
- Add calculated date and time fields (e.g., Revenue, Day of Week, Month, Hour) to prepare the data for in-depth analysis.

### 2. Exploratory Data Analysis with PivotTables
- Utilize Excel PivotTables to slice and dice the coffee shop data.
- Create various views to analyze time-series trends (e.g., sales by month, day of week, hour of day) and product-level trends (e.g., sales by product category, type, and detail).

### 3. Dynamic Dashboard Creation & Insights
- Visualize the key findings using Excel Pivot Charts.
- Design and build an interactive dashboard that allows users to explore sales data dynamically.
- Identify and present key insights and actionable recommendations for Maven Roasters based on the data analysis.

## Dataset

The dataset used for this analysis is `Coffee Shop Sales.xlsx` (source: `Transactions.csv`). It contains detailed transaction records with the following columns:

- **transaction_id**: Unique identifier for each transaction.
- **transaction_date**: Date when the transaction occurred.
- **transaction_time**: Time of the transaction.
- **transaction_qty**: Quantity of products purchased in a transaction.
- **store_id**: Unique identifier for each store location.
- **store_location**: Name of the store's physical location.
- **product_id**: Unique identifier for each product sold.
- **unit_price**: Price of a single unit of the product.
- **product_category**: General category of the product (e.g., Coffee, Tea, Bakery).
- **product_type**: Specific type or variant of the product.
- **product_detail**: Additional details about the product (e.g., size, blend).

## Methodology

The project followed a structured data analysis workflow:

1. **Data Loading & Initial Inspection**  
   The CSV file was loaded into Excel, and an initial review was performed to understand its structure and identify potential issues.

2. **Data Cleaning & Preparation**
   - **Missing Values**: Checked for and confirmed no missing values across critical columns.
   - **Data Types**: Converted `transaction_date` and `transaction_time` to appropriate date/time formats.
   - **Structural Consistency**: Verified consistency in categorical fields (`store_location`, `product_category`, `product_type`, `product_detail`) for uniform reporting.
   - **Duplicate Removal**: Confirmed no exact duplicate rows were present.
   - **Feature Engineering**: Created a Revenue column (`transaction_qty * unit_price`), and extracted Month, Day of Week, and Hour from date/time fields.

3. **Data Analysis with PivotTables**  
   Utilized Excel's PivotTable functionality to aggregate and summarize data by various dimensions (time, location, product).

4. **Dashboard Design & Visualization**  
   Created interactive Pivot Charts and organized them into a dynamic dashboard for easy interpretation of trends and performance metrics.

## Key Insights & Recommendations (Based on Dashboard)

### Key Performance Indicators (KPIs)
- **Total Revenue:** $230,057
- **Total Units Sold:** 71,742

### Sales Trends

#### Transactions by Hour of the Day
- Peak transaction hours are observed around **9 AM and 10 AM**, indicating high morning traffic.
- Another significant peak around **3 PM to 4 PM**.
- Sales significantly drop after **6 PM**.

**Recommendation:**  
Optimize staffing and promotions during peak hours (9–10 AM, 3–4 PM). Consider "happy hour" deals or special offerings to boost sales during slower evening hours (after 6 PM).

#### Transactions by Weekdays
- **Monday** appears to be the busiest day, followed closely by Thursday and Friday.
- **Weekend** sales (Saturday and Sunday) are consistent but slightly lower than weekdays.

**Recommendation:**  
Leverage Monday's high traffic with loyalty programs or special offers. Analyze reasons for slightly lower weekend sales and explore weekend-specific promotions or events.

#### Total Revenue by Month
- Revenue shows a steady upward trend from **January to June**, with June being the highest revenue month at **$54,646**.

**Recommendation:**  
Investigate factors contributing to the consistent growth and replicate successful strategies. Plan for potential seasonal dips in colder months (January, February) with targeted campaigns.

### Product Performance

#### Transactions by Product Category
- **Coffee** is by far the leading product category with over 16,000 transactions.
- **Tea** and **Bakery** are the next most popular categories.
- Categories like **Coffee beans**, **Loose Tea**, **Branded**, and **Packaged Chocolate** have significantly fewer transactions.

**Recommendation:**  
Continue to prioritize coffee offerings. Explore ways to boost sales for lower-performing categories, such as better display, promotions, or re-evaluating their product mix.

### Store Performance (from dashboard slicer)
- The dashboard allows filtering by `store_location` (Astoria, Hell's Kitchen, Lower Manhattan), enabling location-specific analysis.
- (Further insights would be derived by interacting with the dashboard to see individual store performance.)

## How to Use This Project

1. **Clone the Repository:**
   ```sh
   git clone [your-repository-url]
   ```

2. **Navigate to the Project Directory:**
   ```sh
   cd maven-coffee-shop-sales-analysis # or whatever your repo name is
   ```

3. **Open the Excel File:**
   - Locate and open the `Coffee Shop Sales.xlsx` file. This file should contain:
     - The original Transactions data (potentially with the added Revenue column and date/time features)
     - The PivotTables created for analysis
     - The interactive dashboard sheet

Feel free to explore the raw data, interact with the PivotTables, and use the slicers on the dashboard to filter and understand the sales trends in more detail.

## Technologies Used

- **Microsoft Excel** (for data preparation, PivotTables, Pivot Charts, and Dashboard)

## Author

Fouzia Ashfaq

## License
MIT License 
