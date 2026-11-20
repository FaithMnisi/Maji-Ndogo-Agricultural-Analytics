# Maji Ndogo: Agricultural Data Exploration and Analysis

## Project Overview

Agricultural planning requires an understanding of the environmental conditions in which crops grow. In this project, I explored agricultural and environmental data from the fictional country of Maji Ndogo to investigate how rainfall, elevation, temperature and soil fertility vary across crop types.

Using Python, SQL and Pandas, I integrated data from multiple tables, corrected data quality issues and analysed growing conditions to identify patterns that could support crop selection and agricultural planning.

## The Objectives

- **Explore crop distribution:** Examine rainfall and elevation associated with different crop types to understand their growing environments.
- **Identify fertile soils:** Compare average soil fertility across soil types to identify soils with higher fertility scores.
- **Assess climate and geography:** Compare rainfall, temperature and elevation across crops to investigate differences in growing conditions.
- **Identify high-performing crops:** Determine which crop types are most frequently represented among fields with above-average standard yields.
- **Filter suitable growing conditions:** Identify fields meeting specific yield, temperature and pollution criteria.

## Tools Used

- Python
- Pandas
- SQL
- SQLite
- SQLAlchemy
- Jupyter Notebook

## Project Workflow

### 1. Data Integration

- Connected to an SQLite database containing four agricultural and environmental tables.
- Used SQL joins on `Field_ID` to combine geographic, weather, soil and crop, and farm management data into a single dataset.
- Loaded the integrated data into a Pandas DataFrame for analysis.

### 2. Data Cleaning and Preparation

Addressed data inconsistencies before analysis:

- Corrected swapped column names.
- Standardised crop names and corrected spelling errors.
- Corrected negative elevation values.
- Removed unnecessary field identifiers.
- Verified crop categories, elevation values and data types.

### 3. Agricultural Analysis

**Crop distribution**

Developed a reusable Python function to calculate average rainfall and elevation for a selected crop, allowing growing environments to be compared across crop types.

**Soil fertility**

Grouped the data by soil type and calculated average fertility scores to compare soil fertility across six soil categories.

**Climate and geographical conditions**

Aggregated elevation, minimum temperature, maximum temperature and rainfall by crop type to compare environmental conditions across eight crop categories.

**Yield performance**

Filtered fields with above-average standard yields, grouped them by crop type and ranked crop categories according to the number of qualifying fields to identify the most frequently represented crop.

**Growing conditions**

Applied multiple filtering criteria to identify fields for a selected crop that had above-average standard yields, average temperatures between 12°C and 15°C, and pollution levels below 0.0001.

### 4. Data Exploration and Visualisation

Used Pandas to create visualisations to support exploratory analysis:

- Bar chart comparing average standard yields across crop types.
- Histogram examining the distribution of standard yields.
- Scatter plot exploring the relationship between pollution levels and standard yields.

Also explored the use of `DataFrame.query()` to simplify filtering and improve readability when applying multiple conditions.

## How the Analysis Can Support Agricultural Planning

The analysis provides a starting point for agricultural decision-making by helping planners:

- Compare environmental conditions across crops when evaluating potential cultivation areas.
- Examine soil fertility differences when assessing agricultural land.
- Explore climate and geographical characteristics associated with different crops.
- Narrow down fields based on selected yield and environmental criteria.
- Identify patterns that could inform the placement and planning of agricultural automation systems.

## Skills Demonstrated

SQL joins and data extraction, Python programming, Pandas data manipulation, data cleaning, exploratory data analysis, aggregation, conditional filtering, data visualisation and reusable functions.
