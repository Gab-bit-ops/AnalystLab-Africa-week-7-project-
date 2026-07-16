# 🌦️ Weather Data ETL Pipeline

A basic ETL (Extract, Transform, Load) pipeline built in Python that retrieves live weather data for multiple Nigerian cities using the OpenWeather API, cleans and structures it with Pandas, and performs basic analysis on the results.

## 📌 Project Overview

This project was built as part of the AnalystLab Africa Data Analyst Intern Program. It demonstrates a complete, real-world data workflow — from pulling live data off a public API, to transforming it into a clean dataset to drawing basic insights from it.

## 📊 Data Source

Weather data was retrieved from the [OpenWeather API](https://openweathermap.org/api) for six Nigerian cities:
- Abuja
- Lagos
- Kano
- Lokoja
- Benue
- Oyo

## 🛠️ Tools Used

- **Python** — core programming language
- **Jupyter Notebook** (via Anaconda) — development environment
- **Requests** — for connecting to and pulling data from the API
- **Pandas** — for data cleaning, transformation, and analysis
- **CSV** — for storing the final dataset

## 🔄 ETL Process

**1. Extract**
Live weather data was pulled from the OpenWeather API for each city using Python's `requests` library, returning raw JSON data.

**2. Transform**
The raw JSON was cleaned and structured into a Pandas DataFrame. Key fields — city, temperature, humidity, weather condition, wind speed, and date/time — were extracted, columns were renamed for clarity, and data types were verified.

**3. Load**
The cleaned dataset was saved as `weather_data.csv`, ready for analysis and reuse.

## 📈 Key Findings

- **Highest temperature:** Kano — 35.44°C
- **Lowest temperature:** Oyo — 24.56°C
- **Highest humidity:** Oyo — 91%
- **Lowest humidity:** Kano
- Weather conditions varied across cities, showing a mix of *broken clouds* and *overcast clouds*
- Notably, the city with the lowest temperature (Oyo) had the highest humidity, while the hottest city (Kano) had the lowest — suggesting an inverse relationship between temperature and humidity in this dataset


