# Investigating COVID-19 Virus Trends
 R Project - exploring data structures

 # COVID-19 Virus Trends Analysis

## Project Overview

This project investigates COVID-19 virus trends with a focus on analyzing the relationship between the number of positive cases and the number of tests conducted across various countries. By examining these trends, we aim to provide insights into the pandemic's impact and identify countries with significant transmission rates relative to testing efforts.

## Data Source

The analysis uses a [dataset from Kaggle](https://www.kaggle.com/datasets/lin0li/covid19testing) that contains COVID-19 data, including testing, positive cases, hospitalizations, recoveries, and deaths.

### Dataset Columns:

- **`Date`**: Date of the data entry.
- **`Continent_Name`**: Name of the continent.
- **`Two_Letter_Country_Code`**: ISO country codes.
- **`Country_Region`**: Names of countries.
- **`Province_State`**: Names of provinces or states; marked as `All States` if not available.
- **`positive`**: Cumulative number of positive cases.
- **`active`**: Number of active cases on the specified date.
- **`hospitalized`**: Cumulative number of hospitalizations.
- **`hospitalizedCurr`**: Number of actively hospitalized cases on the specified date.
- **`recovered`**: Cumulative number of recovered cases.
- **`death`**: Cumulative number of deaths.
- **`total_tested`**: Cumulative number of tests conducted.
- **`daily_tested`**: Number of tests conducted on the specified date.

## Objectives

The main objective of this project is to answer the question:

- **Which countries have reported the highest number of positive cases in relation to the number of tests conducted?**

## Methodology

- **Data Processing**: The data was processed using R and the `dplyr` package for data manipulation.
- **Summarization**: We grouped the data by country and calculated the total number of tests, positive cases, active cases, and hospitalizations.
- **Analysis**: The project focused on identifying the top countries with the highest ratio of positive cases to tests conducted.
- **Visualization**: Results were visualized to highlight trends and differences across countries.

## Key Findings

- **High Positive-to-Test Ratios**: The analysis identified countries such as the United States, United Kingdom, and Turkey as having high ratios of positive cases relative to the number of tests conducted.
- **Healthcare System Impact**: Data on active and hospitalized cases provided insights into how different countries' healthcare systems managed COVID-19 patients.
- **Ongoing Monitoring**: The findings emphasize the need for continuous monitoring and data analysis to understand the pandemic's evolving dynamics.

## Recommendations

- **Enhance Testing Capabilities**: Increase testing efforts in countries with high positive-to-test ratios to better identify and isolate cases.
- **Targeted Public Health Interventions**: Focus resources on regions with high transmission rates to effectively control outbreaks.
- **Data-Driven Decision Making**: Use data analytics to inform public health strategies, including lockdown measures and vaccination campaigns.

## Project Structure

- **Dataframes**: `covid_df`, `covid_df_all_states`, `covid_df_all_states_daily`, and `covid_top_10`.
- **Matrix**: `covid_mat`.
- **Vectors**: `vector_cols` and `countries`.

## How to Run

1. **Clone the Repository**: `git clone <repository_url>`
2. **Install Required Packages**: Ensure you have R and necessary packages (like `dplyr`) installed.
3. **Run the R Markdown File**: Open and execute `COVID19 Project.Rmd` to reproduce the analysis.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request if you'd like to improve the project.

