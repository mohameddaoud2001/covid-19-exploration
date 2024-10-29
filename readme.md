# COVID-19 Data Exploration

This project explores and analyzes COVID-19 data, providing insights into infection and death rates, population impact, and vaccination progress across countries and continents. The analysis demonstrates SQL skills such as joins, common table expressions (CTEs), temporary tables, window functions, aggregate functions, views, and data type conversions.

## Project Structure

This project is structured to investigate key aspects of COVID-19's global impact, including infection rates, death percentages, and vaccination progress.

### Data Sources

- **PortfolioProject..CovidDeaths**: Contains data on COVID-19 cases, deaths, and population.
- **PortfolioProject..CovidVaccinations**: Contains vaccination data.

### Skills Used

- **SQL Techniques**: Joins, CTEs, Temporary Tables, Window Functions, Aggregate Functions, Views.
- **Data Processing**: Converting data types, handling NULL values, managing indexes.

---

## SQL Queries Overview

1. **Basic Data Extraction**
   - Extracts initial data for exploration and applies filters to refine focus by continent.

2. **Infection and Death Analysis**
   - Calculates the death percentage for COVID-19 cases to show the likelihood of mortality for each country.
   - Assesses infection rates as a percentage of the total population.

3. **Country and Continent Analysis**
   - **Highest Infection Rates**: Identifies countries with the highest infection rate as a percentage of the population.
   - **Highest Death Counts**: Shows countries with the most deaths as a total and by population ratio.
   - **Continent Comparison**: Aggregates death data by continent to identify which regions were most impacted.

4. **Global Summary**
   - Summarizes global case and death totals, as well as the global death percentage.

5. **Vaccination Analysis**
   - **Vaccination Progress**: Shows the cumulative number of people vaccinated and percentage of the population vaccinated per location.
   - **CTE Calculation**: Uses CTEs to calculate rolling vaccination totals and population percentages.
   - **Temporary Table**: Creates a temporary table to hold population vaccination percentage data for further analysis.
   - **View Creation**: Defines a view to store rolling vaccination data for future visualizations and reporting.

---

## Project Queries

The primary SQL queries cover various aspects of COVID-19 data analysis:

1. **Data Filtering and Sorting**: Retrieves initial data by location, date, and case count.
2. **Total Cases vs. Death Rate**: Shows the percentage of deaths among total cases per country.
3. **Infection Rate by Population**: Calculates infection rates as a proportion of the population.
4. **Highest Infection and Death Rates**: Identifies the countries with the highest infection and death rates relative to population.
5. **Continental Death Rates**: Compares continents by their maximum death counts.
6. **Global Aggregation**: Summarizes total global cases, deaths, and calculates the global death rate.
7. **Vaccination Data**: Analyzes vaccination rates and calculates the percentage of the vaccinated population using CTEs and temporary tables.
8. **View for Visualization**: Creates a view (`PercentPopulationVaccinated`) for storing cumulative vaccination data.

---

## Requirements

- **SQL Server Management Studio** (SSMS) or any compatible SQL environment.
- Data tables `PortfolioProject..CovidDeaths` and `PortfolioProject..CovidVaccinations` with required fields: `Location`, `Date`, `Total_cases`, `New_cases`, `Total_deaths`, `Population`, `New_vaccinations`, `Continent`.

## Usage

1. Run each SQL query in sequence to explore and analyze the COVID-19 dataset.
2. Utilize the `PercentPopulationVaccinated` view to retrieve cumulative vaccination data for visualization or further analysis.

## Potential Improvements

- **Indexing**: Add indexes on frequently used columns to optimize performance on large datasets.
- **Error Handling**: Include `CASE` statements to manage division by zero errors.
- **Time-based Aggregation**: Group data by time intervals (e.g., months) for trend analysis.
- **Vaccination-Death Correlation**: Explore correlations between vaccination rates and death rates to gain deeper insights.

---
