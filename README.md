# Climate Analysis for Honolulu, Hawaii

## Overview

This project involves analyzing climate data for Honolulu, Hawaii. The analysis focuses on precipitation and temperature data, and an API is created to provide access to this data.

## Project Structure

### Data Analysis

The analysis covers the last 12 months of available climate data, using Python libraries such as SQLAlchemy, Pandas, and Matplotlib.

### Flask API

A Flask API is provided to access the climate data. The API allows users to query precipitation data, station information, temperature observations, and temperature statistics over specific date ranges.

## Files

- **`climate_analysis.ipynb`**: Jupyter notebook containing the climate data analysis.
- **`app.py`**: Flask application providing API endpoints.
- **`hawaii.sqlite`**: SQLite database containing the climate data.
- **`README.md`**: This file.

## API Endpoints

- **`/api/v1.0/precipitation`**: Returns precipitation data for the last 12 months.
- **`/api/v1.0/stations`**: Returns a list of weather stations.
- **`/api/v1.0/tobs`**: Returns temperature observations for the most active station over the last 12 months.
- **`/api/v1.0/<start>`**: Returns minimum, average, and maximum temperatures from the start date onwards.
- **`/api/v1.0/<start>/<end>`**: Returns minimum, average, and maximum temperatures for the specified date range.

## Data Source

The project uses an SQLite database (`hawaii.sqlite`) that contains two tables:
- **`Measurement`**: Contains daily precipitation and temperature observations.
- **`Station`**: Contains information about the weather stations.
