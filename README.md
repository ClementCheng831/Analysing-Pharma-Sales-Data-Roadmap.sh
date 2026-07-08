# Pharmaceutical Sales Data Analysis

This repository contains a data analysis workflow that explores hourly pharmaceutical sales data to uncover purchasing patterns across various drug categories and brands.

This project is inspired by the challenge hosted on [roadmap.sh/projects/pharmaceutical-sales-data](https://roadmap.sh/projects/pharmaceutical-sales-data).

## Project Overview

The objective of this analysis is to process historical sales information and answer key business questions regarding drug distribution and seasonal demand. 

### Key Questions Answered
* **Total Sales Quantities:** What are the total sales quantities for each drug category (ATC code)?
* **Top Drug Brands:** Which individual drug brands have the highest total sales?
* **High Sales Anomalies:** Which three drugs had the highest sales specifically in January 2015, July 2016, and September 2017?
* **Yearly Volumetrics:** Which drug sold the most often throughout the entire year of 2017?
* **Average Daily Velocity:** Which drug category yields the highest average daily sales?
* **Seasonality Trends:** Are respiratory drugs (ATC code: R03) sold more frequently during specific months of the year?

## Dataset Information

The analysis expects an input data file named `saleshourly.csv`. The schema contains the following layout:
* **datum:** Date and hour string representing the data collection window.
* **ATC Codes (M01AB, M01AE, N02BA, N02BE, N05B, N05C, R03, R06):** Columns containing numerical values representing the volume or quantity sold for that specific drug category.
* **Time-Series Meta Columns:** Extracted markers including `Year`, `Month`, `Hour`, and `Weekday Name`.

## Requirements

The analysis relies on standard Python data science libraries. Ensure you have the following installed:

```bash
pip install pandas numpy matplotlib
