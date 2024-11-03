# Discharge-Stage Data

This repository contains discharge and stage measurements from 180 stream gauges across Iceland, Sweden, and the United States. The data was used in the analysis presented in [paper citation to be added upon publication].

## Data Description

The repository contains stage-discharge measurements from:
- Iceland: 60 stations
- Sweden: 60 stations
- United States: 60 stations

Each data file contains the following variables:
- `meas_nu`: Measurement number/ID
- `station_number`: Unique station identifier
- `station_name`: Name of the station
- `date`: Date of measurement (YYYY-MM-DD)
- `W`: Stage/water level (m)
- `Q`: Discharge (m³/s)
- `country`: Country of station location

## Data Structure

The data is organized in three CSV files under the `data/` directory:
- `iceland.csv`: Measurements from Icelandic stations
- `sweden.csv`: Measurements from Swedish stations
- `usa.csv`: Measurements from United States stations

## Usage

The data can be easily loaded in R:
```R
iceland_data <- read.csv("data/iceland.csv")
sweden_data <- read.csv("data/sweden.csv")
usa_data <- read.csv("data/usa.csv")