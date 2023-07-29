---
title: "TICKER-CHART API"
description: "An API to fetch historical chart data for the stocks in Indian National Stock Exchange. Hosted on pythonanywhere.com | Tech Stack: Flask, Python"
#dateString: Jan 2021 - May 2021
draft: false
tags: ["REST", "API", "Python", "Flask", "Postman", "Stocks"]
showToc: false
weight: 140
cover:
    image: "projects/tickerchart/cover.jpg"
--- 
### 🔗 [Github Repository](https://github.com/NehalH/TickerChart)

## Description
TickerChart is a Python-based API built using flask that provides historical stock market chart data for companies listed on the Indian National Stock Exchange (NSE). It leverages the popular Flask web framework and yfinance library to fetch and deliver stock market data in JSON format.

## Deployment

The TickerChart API is now deployed and accessible on PythonAnywhere. You can access the API using the following endpoint:

- **API Endpoint** : [http://nehalhosalikar.pythonanywhere.com/chart](http://nehalhosalikar.pythonanywhere.com/chart)

## How to Use

To use the TickerChart API, send a GET request to the `/chart` endpoint with the required query parameters.

### Parameters

- `ticker`: The stock ticker symbol of the company you want to retrieve data for.
- `period`: The time duration for which you want historical data. Valid periods are: `1d`, `5d`, `1mo`, `3mo`, `6mo`, `1y`, `2y`, `5y`, `10y`, `ytd`, `max`.
- `interval`: The time interval between data points. Valid intervals are: `1m`, `2m`, `5m`, `15m`, `30m`, `60m`, `1h`, `1d`, `1wk`, `1mo`, `3mo`.

### Response

The API will respond with JSON data containing historical stock market chart data for the requested company and period. The data will be presented in a list of records format.

## Example API Usage

To use the TickerChart API, make a GET request to the `/chart` endpoint with the required query parameters. Here's an example API call:

- **Example API Call** : http://nehalhosalikar.pythonanywhere.com/chart?ticker=TATASTEEL&period=1d&interval=1m
