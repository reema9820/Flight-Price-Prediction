# Airline Data Analysis

This repository contains a detailed analysis of airline pricing data, focusing on various aspects such as feature engineering, data preprocessing, exploratory data analysis (EDA), and preparation for a machine learning model.

## Project Overview

The objective of this project is to explore and analyze airline pricing data to uncover patterns and insights. The dataset includes information such as airlines, source, destination, total stops, price, date, month, year, departure and arrival times, and duration.

## Table of Contents

- [Dataset](#dataset)
- [Feature Engineering](#feature-engineering)
- [Handling Missing Values](#handling-missing-values)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Outlier Detection](#outlier-detection)
- [Skewness Treatment](#skewness-treatment)
- [Assumption of Linear Regression](#assumption-of-linear-regression)
- [Encoding Categorical Variables](#encoding-categorical-variables)
- [Conclusion](#conclusion)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Dataset

The dataset used in this project contains the following columns:

- **Airline:** The name of the airline.
- **Source:** The departure city.
- **Destination:** The arrival city.
- **Total Stops:** The number of stops between source and destination.
- **Price:** The ticket price.
- **Date:** The date of travel.
- **Month:** The month of travel.
- **Year:** The year of travel.
- **Dep_hour:** The hour of departure.
- **Dep_minutes:** The minute of departure.
- **Arrival_hour:** The hour of arrival.
- **Arrival_minutes:** The minute of arrival.
- **Duration_hours:** The duration of the flight in hours.
- **Duration_mins:** The duration of the flight in minutes.

## Feature Engineering

- Extracted day, month, and year from the date column.
- Created separate columns for the hour and minute of departure and arrival times.
- Converted the `Total_Stops` column into a numerical ordinal categorical type using Label Encoding.

## Handling Missing Values

- Checked for missing values in the `Total_Stops` column.
- Imputed missing values based on similar entries within the dataset.

## Exploratory Data Analysis (EDA)

- Analyzed the distribution of prices based on the number of stops, travel duration, and the month of travel.
- Visualized the relationships between different numerical features and the target variable (Price).

## Outlier Detection

- Identified and discussed outliers in features such as `Total_Stops`, `Duration_hours`, and `Price`.
- Dropped data entries that contained incorrect flight durations.

## Skewness Treatment

- Applied log transformation to the `Duration_hours` column to correct skewness.
- Ensured that the skewness of other numerical columns was within acceptable thresholds.

## Assumption of Linear Regression

- Visualized the relationships between the independent variables and the target variable using scatter plots.
- Identified correlations between the variables using a heatmap.

## Encoding Categorical Variables

- Applied One-Hot Encoding to categorical variables to convert them into numerical columns.
- Verified the shape of the dataset after encoding.

## Conclusion

This project provides a thorough analysis of airline data, laying the groundwork for further model development and prediction tasks.

## Dependencies

- Python 3.x
- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/reema9820/Flight-Price-Prediction.git
    ```
2. Navigate to the project directory:
    ```bash
    cd airline-data-analysis
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

Run the main analysis script to perform data processing and visualization


## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.


