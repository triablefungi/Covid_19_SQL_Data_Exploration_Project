# COVID-19 Data Exploration Using SQL

## Project Overview

This project explores global COVID-19 cases, deaths, population figures, and vaccination progress using Microsoft SQL Server.

The analysis examines how COVID-19 affected different countries and continents, compares reported cases with deaths and population figures, and tracks vaccination progress over time.

The dataset covers the period from **1 January 2020 to 30 April 2021** and contains information for **219 locations**.

## Project Objectives

The main objectives of this project were to:

- Compare total COVID-19 cases with total deaths
- Calculate the percentage of the population infected
- Identify countries with the highest infection rates
- Identify countries with the highest reported death counts
- Compare COVID-19 deaths across continents
- Calculate global case and death figures
- Track cumulative vaccinations by country
- Calculate the percentage of each country's population vaccinated

## Dataset

The project uses two datasets:

- `covid_deaths.csv` — COVID-19 cases, deaths, population, hospitalisation, and location data
- `covid_vaccinations.csv` — COVID-19 testing, vaccination, demographic, economic, and healthcare data

The files contain approximately 85,000 records each.

Original data source: [Our World in Data COVID-19 Dataset](https://ourworldindata.org/covid-deaths)

## Tools Used

- Microsoft SQL Server
- SQL Server Management Studio
- Microsoft Excel
- GitHub

## SQL Skills Demonstrated

This project demonstrates the use of:

- Joins
- Common Table Expressions
- Temporary tables
- Window functions
- Aggregate functions
- Data type conversion
- Views
- Filtering and sorting
- Grouping data
- Percentage calculations

## Analysis Performed

### 1. Total Cases vs Total Deaths

Calculated the percentage of reported COVID-19 cases that resulted in recorded deaths.

### 2. Total Cases vs Population

Calculated the percentage of each country's population that had recorded COVID-19 infections.

### 3. Countries with the Highest Infection Rates

Compared each country's highest recorded case count against its population.

### 4. Countries with the Highest Death Counts

Identified the countries with the highest cumulative reported COVID-19 deaths.

### 5. Death Counts by Continent

Compared the highest reported death totals across continents.

### 6. Global COVID-19 Figures

Calculated total reported cases, total reported deaths, and the global death percentage.

### 7. Population vs Vaccinations

Joined the deaths and vaccination datasets using location and date.

A window function was used to calculate cumulative vaccinations for each country.

### 8. Vaccination Percentage

Used a Common Table Expression and temporary table to calculate the percentage of each country's population that had received vaccinations.

### 9. SQL View

Created the `PercentPopulationVaccinated` view to store vaccination data for future visualisation and dashboard projects.

## Key Findings

Based on the dataset through 30 April 2021:

- Approximately **150.6 million reported COVID-19 cases** were recorded globally
- Approximately **3.18 million reported deaths** were recorded globally
- Recorded deaths represented approximately **2.11% of reported cases**
- The United States had the highest recorded death count in the dataset
- Andorra had one of the highest recorded infection rates relative to population
- Vaccination progress varied significantly between countries

These figures reflect reported data available in the dataset and should not be interpreted as current COVID-19 statistics.

## Repository Structure

```text
covid-19-sql-data-exploration/
│
├── README.md
├── SQL/
│   └── covid_19_data_exploration.sql
└── Data/
    ├── covid_deaths.csv
    └── covid_vaccinations.csv
