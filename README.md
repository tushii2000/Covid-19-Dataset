# COVID-19 Data for India

This repository contains COVID-19 data for India in JSON format. The data includes information about daily cases, deaths, testing, and more.

## Data Source

The data is sourced from [data.covid19india.org](https://data.covid19india.org/v4/min/timeseries.min.json).

## Overview

The JSON file contains a time series of COVID-19 data, including daily counts of cases, deaths, and testing. Below is a brief overview of the data structure:

- `dates`: Contains daily data entries.
- `delta`: Provides the daily changes in cases, deaths, testing, etc.
- `total`: Represents the cumulative totals up to each date.

For more detailed information about the data structure, please refer to the [data dictionary](https://data.covid19india.org/v4/min/timeseries.min.json).

## Usage

To use this data, you can download the JSON file from the provided link or clone this repository. You can then parse the JSON file using your preferred programming language (e.g., Python, JavaScript) and extract the relevant data for analysis or visualization.

Here's an example of how to load the data in Python:

import requests
url="https://data.covid19india.org/v4/min/timeseries.min.json"
data=requests.get(url)
d1=data.json()
print(d1)

