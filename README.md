# COVID-19 Data Analysis and Visualization

## Project Overview
This project combines data analysis and visualization skills to explore the impact of the COVID-19 pandemic. Using SQL Server and Tableau, we perform data cleaning, querying, and advanced analysis to uncover trends and insights, which are then visualized through interactive dashboards. This comprehensive project demonstrates essential data analyst skills, including ETL (Extract, Transform, Load), data manipulation, and effective data presentation.

## Project Outline
The project consists of two main phases:
1. **SQL Data Analysis**: Creating a SQL Server database, importing data, cleaning it, and performing complex queries.
2. **Tableau Visualization**: Building insightful visualizations from the cleaned data and assembling them into a dashboard for interactive exploration.

---

## Phase 1: SQL Data Analysis

### 1. Data Preparation
- **Data Sources**: Use two Excel files:
  - `covid_deaths.xlsx`
  - `covid_vaccinations.xlsx`
- **Important**: Ensure the Excel files are saved as workbooks, not CSV files, to prevent import errors.

### 2. Creating the SQL Database
1. **Set Up SQL Server**: Open SQL Server and use the Import and Export wizard.
2. **Data Source Selection**: Choose the Excel files as the source.
3. **Database Configuration**: Set up a new SQL Server database as the destination.
4. **Verify Server Name**: Ensure it matches your SQL Server instance to avoid import issues.
5. **Data Import**: Complete the import to create tables for deaths and vaccinations data.

### 3. Data Validation and Basic Queries
- **Initial Queries**: Run SELECT statements to confirm data import.
- **Filtering and Sorting**: Use WHERE and ORDER BY clauses to filter data by location and date.
- **Use of Comments**: Add comments in SQL scripts to document your code.

### 4. Advanced SQL Analysis
- **Data Joins**: Join tables to combine deaths and vaccination data for deeper analysis.
- **Grouping and Aggregation**: Use GROUP BY to analyze data by continent and calculate global statistics.
- **CTEs and Temporary Tables**: Simplify complex queries and improve performance.
- **Creating Views**: Store results in views for easy access during visualization.

### 5. ETL and Data Cleaning
- **Handling Null Values**: Address inconsistencies and ensure data integrity.
- **Global Metrics Calculation**: Compute total cases, death percentages, and other key figures using SQL aggregate functions.
- **Data Preparation for Visualization**: Create structured data outputs for Tableau.

---

## Phase 2: Tableau Visualization

### 1. Preparing Data for Tableau
- **Cleaning Data**: Ensure there are no null values in the Excel sheets. Convert nulls to zeros to maintain numeric data types.
- **Separate Data Sources**: Import each Excel sheet into Tableau as a separate data source. This allows for more flexibility in visualization.

### 2. Building Visualizations
- **Global Summary Table**: 
  - **Description**: A table showing total cases, total deaths, and average death percentage.
  - **Formatting**: Customize with color changes, size adjustments, and gridlines for clarity.
  - **Number Formatting**: Ensure precise representation with two decimal places for percentages.

- **Bar Graph of Global Death Counts by Continent**: 
  - **Steps**: Drag "Continent" to Rows and "Total Deaths" to Columns.
  - **Customization**: Sort bars in descending order, adjust axis labels, and rename fields for clarity.

- **Map Visualization**:
  - **Setup**: Convert "Location" to a geographic role (Country/Region) to generate longitude and latitude.
  - **Enhancements**: Add infection rates, customize colors, adjust map backgrounds, and label countries.
  - **Data Representation**: Ensure colors are intuitive and convey data effectively.

- **Time-Series Chart**:
  - **Objective**: Track the percentage of the population infected over time.
  - **Implementation**: Add "Date" to Columns and "Infection Percentage" to Rows. Modify the date display to show yearly data.
  - **Forecasting**: Add predictive elements to estimate future infection trends based on historical data.

### 3. Creating the Tableau Dashboard
- **Combining Visualizations**: Arrange the bar graph, map, and time-series chart on a single dashboard.
- **Interactive Elements**: Add filters and legends to enable users to explore the data dynamically.
- **Design Considerations**: Optimize layout and colors to enhance user experience and data comprehension.

---

## Key Concepts and Techniques
- **SQL**: Master data querying, joins, CTEs, and views for efficient data manipulation.
- **Data Cleaning**: Handle null values and inconsistencies for accurate analysis.
- **Tableau**: Create interactive and visually appealing dashboards that communicate insights effectively.
- **ETL Process**: Import and transform data, ensuring it is analysis-ready.

---

## Best Practices
- **SQL Queries**: Write clean and efficient queries, adding comments for documentation.
- **Data Validation**: Always check for accuracy after each transformation step.
- **Visualization**: Choose colors and formats that enhance data interpretation.

## Future Enhancements
- **Automate Data Cleaning**: Use Python and pandas for more efficient data processing.
- **Machine Learning**: Incorporate predictive models for deeper insights.
- **Expand Analysis**: Include additional datasets for a broader perspective.

## Conclusion
This project illustrates how to leverage SQL and Tableau to analyze and visualize real-world data. It highlights the entire data analysis workflow, from data import and cleaning to creating interactive dashboards, demonstrating essential data analyst skills.
