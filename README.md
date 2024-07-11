# MBTA - Load on the bus prediction

## Project Overview
This project aims to predict the load on a Massachusetts Bay Transportation Authority (MBTA) bus at a given time and date. The goal is to assist in efficient resource allocation and improve service quality. By leveraging historical bus service data, we built a regression model to forecast passenger load, helping MBTA optimize operations and enhance rider experience.

## Team Members
- Praneith Ranganath (ranganth.p@northeastern.edu)
- Aditya Bharadwaj Shivapura Guruprasad (shivapuraguruprasa.a@northeastern.edu)

## Problem Statement
The MBTA faces challenges in meeting service demands due to a shortage of drivers and an increasing population. This project addresses the following questions:
1. What is the predicted load of a bus on a particular date and time?
2. How can bus driver utilization be optimized?
3. Which bus routes need additional resources?

## Dataset
The dataset is sourced from the MBTA Open Data Portal. It includes over 5 million records spanning 5 years, with both numerical and categorical attributes. Key columns include:
- `route_id`: Unique identifier for each bus route.
- `stop_name`: Name of the bus stop.
- `day_type`: Indicates whether the data corresponds to a Weekday, Saturday, or Sunday.
- `load_`: Number of passengers on the bus at a stop.

## Data Exploration and Processing
- **Average Load Analysis**: Identified peak hours and trends in passenger demand to suggest operational improvements.
- **Correlation Analysis**: Used to understand relationships between variables and ensure all attributes are considered in the model.
- **Visualization**: Scatter plots and bar graphs were used to identify patterns and insights from the data.

## Model Development
Several regression models were tested, including Linear Regression, K-Nearest Neighbors (KNN), Decision Tree, and Random Forest. Random Forest provided the best performance due to its ability to handle large datasets and capture complex relationships between variables.

## Key Findings
- The number of passengers boarding is the most significant predictor of bus load.
- Trip start time is also a crucial factor.
- Day of the week has a lesser impact on load prediction.

## Impact
The predictive model helps MBTA make informed decisions on scheduling and resource allocation, ultimately improving service efficiency and passenger satisfaction. It also aids in mitigating operational losses due to underutilized services.

## How to Use
1. Clone this repository.
2. Ensure you have Python and necessary libraries installed.
3. Follow the provided notebooks/scripts to preprocess the data and train the model.
4. Use the trained model to make predictions on bus load and optimize MBTA operations.
