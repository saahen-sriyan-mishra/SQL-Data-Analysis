# SQL DATA ANALYSIS
(All the findings and relationship are visualised into Tableau and Power BI repositories)
## Tools Used:
SQL server management studio 19
## SQL Functions Used:
Arithmetic operations,  conversion functions, Cast functions,  grouping, ordering, sorting, filtering, Aggregation functions, Using CTE and Temp Tables, View for data storage, Table manipulation (Feature Engineering) etc.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Covid 19 Data Exploration

### Introduction
This contains SQL queries and data exploration scripts for analyzing Covid-19 data, including death rates, vaccination statistics, infection rates, and population statistics.

### Data Source
The data used for this analysis is sourced from the "Covid Death & Vaccination" dataset.

### Queries Overview
#### Exploration Queries
 - **Select all Covid death and vaccination data with continents:** Retrieves all data from the "Covid Deaths" table where the continent is not null, ordered by columns 3 and 4.
 - **Select relevant data for exploration:** Selects specific columns for exploration from the "Covid Deaths" table where the continent is not null, ordered by location and date.

#### Country-wise Analysis
- **Total cases vs Total deaths:** Calculates the death percentage based on total cases for each country.
- **Total cases vs Population:** Calculates the percentage of the population infected with Covid-19 for each country.
- **Countries with highest infection rate compared to population:** Identifies countries with the highest infection rates compared to their populations.
- **Country with highest death count:** Identifies the country with the highest death count.
- **Country with highest death count for total population:** Identifies the country with the highest death count relative to its total population.

#### Continent-wise Analysis
- **Continent with highest death count:** Identifies the continent with the highest death count.

#### Worldwide Data
- **Worldwide Covid-19 data:** Provides a summary of worldwide Covid-19 cases and deaths.

#### Data Joins and Transformations
- **Joining Covid death and vaccination tables:** Joins the Covid death and vaccination tables based on location, date, and continent.
- **New data for analysis by joining tables:** Retrieves new data for analysis by joining the Covid death and vaccination tables.
- **Showing people vaccinated vs country on date basis:** Shows the number of people vaccinated per country on a specific date.

#### Using CTEs and Temporary Tables
- **Using CTE for people vaccinated percentage:** Calculates the percentage of people vaccinated using a Common Table Expression (CTE).
- **Temporary table for calculation of people vaccinated percentage:** Creates a temporary table to calculate the percentage of people vaccinated.

#### Views for Visualization
- **DeathTableStats View:** A view containing death statistics for visualization purposes.
- **PopulationVsVaccination View:** A view containing population and vaccination statistics for visualization.

### Visualization Data Queries
- **Total cases, total deaths, and death percentage:** Retrieves total cases, total deaths, and death percentage.
- **Total death count by location:** Retrieves the total death count by location.
- **Highest infection count and percentage:** Retrieves the highest infection count and percentage for each location.
- **Highest infection count and percentage by date:** Retrieves the highest infection count and percentage for each location by date.

**Dashboard link:** [Covid-19 Dashboard](https://github.com/saahen-sriyan-mishra/Tableau-Visualizations/blob/main/1.%20COVID%20DEATHS%20AND%20VACCINATIONS/Covid-19%20Dashboard.twbx)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------


## BikeStores Database Exploration

### Introduction
This repository contains SQL scripts for setting up the BikeStores sample database and performing various data exploration tasks.  The aim is to uncover insights into customer behavior, sales volumes, product performance, and revenue generation.

### Database Information
- **Link:** [BikeStores Sample Database](http://www.sqlservertutorial.net/load-sample-database/)

### SQL Queries

#### Schema Creation
- Two schemas are created: `production` and `sales`.

#### Table Creation
production.categories, production.brands, production.products, sales.customers, sales.stores, sales.staffs, sales.orders, sales.order_items, production.stocks

#### Data Population
- Data is populated into the tables for both the schemas.

#### Queries Overview
- **Customer Details** Retrieves customer details along with their orders.
- **Sales Volume & Total Revenue** Calculates the total units purchased and revenue generated by each customer.
- **Product Unit & Revenue by Customers** Analyzes individual product unit and revenue from different customers.
- **Final Dataset** Provides detailed insights into individual product unit and revenue by categories, store, and salesperson, from different customers.

**Dashboard link:** [Bike Store Sales Dashboard](https://github.com/saahen-sriyan-mishra/Tableau-Visualizations/blob/main/2.%20BIKE%20STORE%20SALES/Bike%20Sales%20Dashboard.twbx)

---------------------------------------------------------------------------------------------------------------------------------


## walmart Sales Data Exploration
This contains SQL queries and scripts for analyzing Walmart sales data stored in the database. The aim is to uncover insights into customer behavior, sales volumes, product performance, rating revenue etc.

### SQL Queries

#### Data Preparation
Before conducting any analysis, ensure that the data is properly processed and structured.
- **Test Before Feature Engineering:** Perform preliminary tests and feature engineering on the data to extract relevant information such as time of the day, day name, and month name.
- **Adding Columns into Temporary Table:** Create a temporary table #sales and insert data from the WalmartSalesData.csv file. This step involves adding additional columns like time_of_day, Day_Name, and Month_Name for enhanced analysis.

#### Analysis
The analysis covers various aspects including product-related metrics, customer insights, and sales performance. Here's a breakdown of the analysis sections:

#### Product Analysis
- **Unique Product Lines:** Identify the distinct product lines available in the dataset.
- **Most Common Payment Method:** Determine the most frequently used payment method.
- **Most Popular Selling Product:** Find the product line with the highest sales volume.
- **Revenue by Month:** Analyze revenue trends over different months.
- **Largest COGS:** Identify the month with the highest Cost of Goods Sold (COGS).
- **Product Line Revenue:** Determine the product line contributing the most to revenue.
- **City Revenue:** Find the city generating the highest revenue.
- **Product Line VAT Analysis:** Identify the product line with the largest VAT.

#### Customer Analysis
- **Unique Customer Types:** Determine the variety of customer types in the dataset.
- **Most Common Customer Type:** Find the most prevalent customer type.
- **Customer Buying Behavior:** Analyze the buying patterns of different customer types.
- **Gender Distribution:** Determine the gender distribution among customers.
- **Gender Distribution per Branch:** Analyze gender distribution across different branches.
- **Rating Analysis:** Explore customer ratings by time of the day, day of the week, and branch.

#### Sales Analysis
- **Sales by Time of the Day:** Analyze sales volume across different times of the day.
- **Revenue by Customer Type:** Determine which customer type contributes the most to revenue.
- **City Tax/VAT Analysis:** Identify the city with the highest tax/VAT percentage.
- **VAT by Customer Type:** Analyze VAT payments based on customer types.

**Dashboard link:** [Walmart Sales Dashboard](https://github.com/saahen-sriyan-mishra/Tableau-Visualizations/blob/main/3.%20WALMART%20SALES/Walmart%20Sales%20Dashboard.twbx)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


### Usage
To replicate the analysis, execute the provided SQL queries in a SQL environment connected to the required DB.
To view the dashboards, click on the link, download the file and exploare the interactive dashboards.

