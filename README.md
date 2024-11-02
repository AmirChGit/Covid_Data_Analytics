# COVID Data Analysis Project

## Description
This project demonstrates a comprehensive approach to building a data analysis portfolio, focusing on analyzing COVID-19 data using SQL, Tableau, and Python (pandas). It walks through the process of creating a database, importing data from Excel files, cleaning and querying the data using SQL, and visualizing it in Tableau. The project showcases skills essential for a data analyst, including ETL (Extract, Transform, Load) processes and data visualization techniques.

## Project Outline
The goal of this project is to import COVID-19 data into a SQL Server database, perform data analysis using SQL, and create visualizations in Tableau to extract meaningful insights. It also covers advanced techniques for handling and preparing data for analysis.

## Steps Involved

### 1. Data Preparation
- **Data Sources**: Use two Excel files:
  - `covid_deaths.xlsx`
  - `covid_vaccinations.xlsx`
- **Important**: The files should be saved as Excel workbooks, not CSV files, to avoid errors during import.

### 2. Creating the SQL Database
1. **Set Up SQL Server**: Open Microsoft SQL Server and launch the Import and Export wizard.
2. **Select Data Source**: Choose the Excel files as the data source.
3. **Destination Configuration**: Set the SQL Server database as the destination.
4. **Verify Server Name**: Ensure the server name matches the SQL Server instance to avoid import errors.
5. **Import Data**: Follow the wizard's steps to import the data into new tables.

### 3. Basic SQL Queries
- **Validate Data**: Perform simple SELECT queries to ensure the data has been imported correctly.
- **Filtering**: Use queries to filter data by location and date.
- **Using Comments**: Add comments in SQL queries for better understanding and maintainability.

### 4. Data Analysis Using SQL
- **Select Specific Columns**: Query the tables to retrieve only the necessary columns.
- **Filter and Sort Data**: Use WHERE clauses and ORDER BY to sort and filter data efficiently.
- **Grouping Data**: Use GROUP BY to summarize data by continent or country.

### 5. Advanced SQL Techniques
- **Data Joins**: Combine tables (e.g., deaths and vaccinations) to create a comprehensive dataset.
- **Common Table Expressions (CTEs)**: Simplify complex queries and improve readability.
- **Temporary Tables**: Store and manipulate intermediate data for further analysis.
- **Views**: Create views to save frequently used queries for future reference.

### 6. ETL Process and Data Cleaning
- **Address Data Inconsistencies**: Filter out or adjust inaccurate data, such as entries labeled "world" or "continent".
- **Calculate Global Metrics**: Use aggregate functions to calculate total cases, death percentages, and other key metrics.
- **Join and Merge Data**: Integrate vaccination data with death counts to analyze correlations.

### 7. Calculating Vaccination Metrics
- **Rolling Count**: Define a new column for "new vaccinations per day" and use the `SUM` function with the `PARTITION BY` clause to calculate a rolling total.
- **Percentage Vaccinated**: Calculate the percentage of the population vaccinated by dividing the rolling count by the total population and multiplying by 100.
- **Methods**: Implement both CTEs and temporary tables for calculating metrics, exploring their advantages.

### 8. Visualization in Tableau
- **Import Data**: Load the cleaned and processed data into Tableau.
- **Create Dashboards**: Develop interactive visualizations to explore data trends, such as vaccination rates and death statistics.
- **Drill-Down Analysis**: Break down data from global to country-specific insights.
- **Highlight Key Metrics**: Use calculated fields to display essential information clearly.

## Key Concepts and Techniques
- **SQL**: Master basic and advanced SQL concepts, including SELECT, WHERE, JOIN, GROUP BY, CTEs, and views.
- **ETL**: Perform data cleaning and transformation efficiently.
- **Data Visualization**: Use Tableau to present data insights effectively.
- **Python (pandas)**: Automate data cleaning and analysis for efficiency (future scope).

## Best Practices
- **Commenting Code**: Use comments in SQL scripts to explain the purpose of each query.
- **Data Validation**: Always validate data after import and transformation.
- **Optimized Queries**: Write efficient queries to handle large datasets.

## Troubleshooting Tips
- **Import Issues**: Double-check the server name and data source format if errors occur.
- **Data Inconsistencies**: Use filters to correct or exclude problematic records.
- **Efficient SQL**: Refactor complex queries to improve performance.

## Future Enhancements
- **Automate with Python**: Use pandas to automate the data cleaning process.
- **Machine Learning**: Apply machine learning models to predict future trends.
- **Broader Analysis**: Expand the dataset to include more variables for comprehensive analysis.

## Conclusion
This project illustrates the end-to-end process of analyzing real-world data using SQL, Tableau, and Python. It highlights the importance of data cleaning, querying, and visualization in deriving actionable insights from complex datasets.
