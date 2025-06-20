# COVID-19-Data-Exploration-Using-SQL

## 📝 Overview

This project focuses on analyzing global COVID-19 data using SQL. The dataset includes information on COVID-19 deaths, infections, population, and vaccinations across different countries and continents. The goal was to derive meaningful insights such as infection and death rates, population impact, and vaccination trends using raw data from [Our World in Data](https://ourworldindata.org/covid-deaths).

---

## 🔄 Steps and Process

### 1. View and Explore the Raw Tables

Two primary tables were used:
- `CovidDeaths`
- `CovidVaccinations`

Initial queries were written to inspect the structure and content of each table and identify relevant fields for analysis (e.g., location, date, total_cases, total_deaths, population).

---

### 2. Data Type Adjustment

To ensure accurate calculations, data types of key columns such as `total_cases` and `total_deaths` were altered to `FLOAT`.
---

### 3. Infection and Death Rate Analysis
Queries were created to evaluate:

The likelihood of death from COVID-19 per country.

Percentage of population infected.

Countries and continents with the highest infection or death rates.

---

### 4. Population vs COVID Impact
The percentage of population affected by COVID-19 was calculated and ranked across countries to understand its global spread.

---

### 5. Grouped and Aggregated Analysis
Highest infection counts were grouped by location.

Death counts were grouped by both country and continent.

Calculations for percent of population infected or deceased were done using aggregated max values.

---

### 6. Global Tracking Over Time
A time-series aggregation was performed to track total daily new cases and deaths globally.

---

### 7. Vaccination Impact Analysis
Using a JOIN between the CovidDeaths and CovidVaccinations tables, a rolling sum was calculated to track the total number of people vaccinated over time in each country.

 
---

###  Final Output
The analysis revealed:

Infection and death percentages by population.

Countries with the highest COVID-19 impact.

Global trends over time.

Progress of vaccination campaigns across nations.

---

###  Tools and Technologies
Database: SQL Server

Techniques Used:

Data exploration and transformation

Aggregation and grouping

Use of window functions

Joins for multi-table analysis

Data type conversion

