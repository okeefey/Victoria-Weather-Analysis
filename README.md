# Victoria Weather Analysis

This project performs a comprehensive analysis of historical weather data for Victoria, British Columbia, covering multiple time periods. The analysis includes data cleaning, visualization, statistical modeling, and comparison of temperature trends over several decades.

---

## Project Overview

The purpose of this project is to investigate monthly and daily temperature trends in Victoria from different time periods (1974–1979, 1984–1989, 2009–2014, and 2019–2024). The project analyzes average and maximum temperatures, examines seasonality effects, conducts hypothesis testing, and predicts future temperature trends.

---

## Data

- The data consists of daily climate CSV files obtained from Environment Canada.
- Files are named by station ID and year, e.g., `en_climate_daily_BC_1018611_2009_P1D.csv`.
- Multiple years' data from several stations are combined and summarized.

---

## Analysis

Key steps and analyses performed in the R Markdown include:

- Data loading and cleaning with custom functions.
- Calculation of monthly average and maximum temperatures.
- Visualization of temperature trends using line plots, boxplots, and heatmaps.
- Linear regression modeling of temperature trends, including seasonality adjustments.
- Two-sample t-tests comparing temperature distributions between different years and periods.
- Checking for heteroskedasticity in regression models.
- Identification of temperature anomalies using z-scores.
- Extrapolation of temperature trends to predict future values.

---

## Usage

To run the analysis:

1. Ensure all CSV data files are placed in the project directory.
2. Open the R Markdown file `Victoria_Weather_Analysis.Rmd` in RStudio.
3. Install required packages if not already installed:

   ```r
   install.packages(c("tidyverse", "ggplot2", "lubridate", "lmtest"))
