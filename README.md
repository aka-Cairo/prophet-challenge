# MercadoLibre Google Search Trends Forecasting with Prophet

## Overview
This repository contains Python code to forecast Google search trends for MercadoLibre using Facebook's Prophet library. Prophet is a robust tool for time series forecasting, capable of capturing trends, seasonality, and holiday effects in the data.

## Steps Covered
1. **Data Preparation**: 
   - We loaded hourly Google search trends data for MercadoLibre using Pandas DataFrame.
   - Cleaned the data by setting the 'Date' column as the Datetime Index and handling any missing values.

2. **Time Series Analysis**:
   - Calculated the total search traffic for May 2020 and the monthly median search traffic across all months.
   - Analyzed the relationship between search trends and MercadoLibre's financial results release.

3. **Prophet Model Implementation**:
   - Set up a Prophet model to forecast search trends.
   - Prepared future data for predictions extending up to 2000 hours (approximately 80 days) using `make_future_dataframe()`.

4. **Visualization**:
   - Visualized Prophet predictions using Matplotlib.
   - Plotted the forecasted trends (`yhat`), along with uncertainty intervals (`yhat_lower` and `yhat_upper`), over the last 2000 hours.

5. **Forecast Components**:
   - Used Prophet's `plot_components()` function to visualize forecast components such as trend, yearly seasonality, and weekly seasonality.

## Files Included or Linked
- **forecasting_net_prophet.ipynb**: Jupyter notebook containing Python code for data loading, analysis, Prophet modeling, and visualization.
- **df_mercado_stock**: Dataset containing MercadoLibre's historical stock prices. (linked)
- **df_mercado_trends.csv**: Dataset containing hourly Google search trends for MercadoLibre. (linked)

## Dependencies
- Python 3.x
- Pandas
- Prophet
- Matplotlib

## Usage
1. Clone the repository:
   ```bash
   git clone <repository-url>
