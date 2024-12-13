# MercadoLibre Search Traffic and Stock Price Analysis

## Project Overview

This project analyzes Google search traffic data for MercadoLibre, the largest e-commerce platform in Latin America, and investigates its relationship with the company's stock price. The analysis aims to identify trends and patterns in search traffic, explore potential connections with financial events, and develop a time series model for forecasting future search traffic.

## Project Structure

The project consists of the following main steps:

1. **Finding Unusual Patterns in Hourly Google Search Traffic:**
    - Analyzing search traffic data for May 2020 (when MercadoLibre released its quarterly financial results).
    - Comparing the total search traffic for May 2020 to the monthly median across all months.

2. **Mining the Search Traffic Data for Seasonality:**
    - Grouping hourly search data to identify average traffic by the hour of day, day of the week, and week of the year.
    - Visualizing these patterns to determine predictable seasonal trends.

3. **Relating the Search Traffic to Stock Price Patterns:**
    - Reading in and plotting the MercadoLibre stock price data.
    - Concatenating the stock price data to the search data in a single DataFrame.
    - Slicing the data to the first half of 2020 and plotting it to identify any common trends.
    - Creating new columns for lagged search trends, stock volatility, and hourly stock return.
    - Analyzing the correlation between these variables to determine any predictable relationships.

4. **Creating a Time Series Model with Prophet:**
    - Setting up the Google search data for a Prophet forecasting model.
    - Estimating the model and plotting the forecast for near-term popularity.
    - Plotting individual time series components to identify the time of day, day of the week, and lowest point for search traffic.

## Dependencies

- pandas
- prophet
- datetime
- numpy
- matplotlib

## Installation

1. Install the required libraries:

 ## Usage

1. Run the Jupyter Notebook containing the code for each step.
2. Follow the comments and instructions within the notebook to execute the analysis.
3. Analyze the generated plots and results to answer the questions posed in each section.

## Findings

- The analysis reveals that search traffic for MercadoLibre exhibits predictable patterns based on time of day, day of the week, and time of year.
- There is a potential correlation between lagged search traffic and stock volatility or stock price returns, indicating a possible relationship between search interest and financial performance.
- The Prophet model forecasts a general increase in search traffic for MercadoLibre in the near term, with some seasonal fluctuations.

## Future Work

- Further investigation into the relationship between search traffic and financial events.
- Refinement of the time series model to improve forecast accuracy.
- Incorporating external factors and data sources to enhance the analysis.

## Contributing

Contributions to this project are welcome. Please feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
