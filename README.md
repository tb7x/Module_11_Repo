# Module_11_Repo

## Description

# This project is supposed to be able to find ways for the company to grow by analyzing the financial and user data. The project essentially predicts the search traffic for the company and if the stock is successfully traded. Graphs were made to visualize the findings.

## Technologies

# This project is written with the programming language Python. It also uses the libraries Pandas, Prophet, hvplot, datetime, matplotlib, numpy, and Path. The project was written on the Windows operating system.
---

## Installation Guide

```

from google.colab import files
uploaded = files.upload()

df_mercado_trends = pd.read_csv('google_hourly_search_trends.csv', index_col = 'Date', parse_dates=True, infer_datetime_format=True)
```

```
from google.colab import files
uploaded = files.upload()

df_mercado_stock = pd.read_csv('mercado_stock_price.csv', index_col = 'date', parse_dates=True, infer_datetime_format=True)
```

## Usage

```
first_half_2020 = mercado_stock_trends_df.loc['2020-01' : '2020-06']

hv.extension('bokeh')
    
first_half_2020.hvplot(shared_axes=False, subplots=True).cols(1)

forecast_mercado_trends = mercado_prophet_df.predict(future_mercado_trends)

mercado_prophet_df.plot(forecast_mercado_trends)

future_mercado_trends = mercado_prophet_df.make_future_dataframe(periods=2000, freq='D')
)

---

## Contributors


# Creator of this project is Thomas Burns
# Email is burns235577@gmail.com
---