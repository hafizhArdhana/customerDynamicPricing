# ✈️ Clustering & Time Series Analyst – Customer Dynamic Pricing

## 📅 Project Period
May 2025

## 📘 Project Description
This project focuses on analyzing and forecasting flight ticket prices using a combination of **unsupervised learning (clustering)** and **time series modeling**. The dataset contains **452,088 records** of flight bookings, consisting of 8 main features:

- `Date of Booking`
- `Date of Journey`
- `Airline-Class` (including airline name, flight number, and class)
- `Departure Time` and `Arrival Time` (including departure and arrival cities)
- `Duration`
- `Total Stops`
- `Price`

All columns were initially of object type and required extensive data cleaning due to mixed-format entries (e.g., combined city names and times, thousands separators in price).

The objective of this project is to:
- Understand patterns in pricing and flight behavior.
- Cluster similar bookings based on flight characteristics.
- Forecast future ticket prices for specific customer segments.

## 🔍 Exploratory Data Analysis (EDA)
- Inspected column types and performed conversion (e.g., dates, price to numeric).
- Visualized distribution of durations, prices, and class imbalance in flight routes.
- Analyzed popular airlines, time patterns, and route frequency.

## 🧹 Data Cleaning
- Parsed and split complex string entries (e.g., separate airline names and flight numbers).
- Standardized city names and time formats.
- Removed or imputed inconsistent entries and outliers.

## 🛠️ Feature Engineering
- Extracted new features such as:
  - Day of week and month from journey date
  - Time of day from departure/arrival time
  - Flight duration in minutes
- Created price per minute and price per stop as engineered metrics.

## 🔗 Clustering
- Applied **K-Means** clustering to group bookings based on:
  - Duration
  - Stops
  - Airline
  - Time features
- Purpose: to segment customers/flights for more accurate pricing strategies.

## ⏳ Time Series Analysis
- Conducted **stationarity tests** (ADF Test) on ticket price series to ensure model assumptions.
- Implemented:
  - **ARIMA**: for univariate forecasting of ticket prices per cluster.
  - **ARIMAX**: included external regressors like duration, stops, and airline to improve predictions.

## 📈 Results
- Identified clusters of similar flight characteristics that show distinct pricing trends.
- Successfully forecasted ticket prices with ARIMA/ARIMAX per cluster segment.
- Demonstrated potential for dynamic pricing models tailored to customer segments.

## 📁 Dataset
The dataset was sourced from internal simulation (CSV format) and includes real-world-like booking behavior across multiple flight routes.

---

> ✨ *This project demonstrates my capability to combine clustering and time series forecasting to uncover insights and build predictive models in the domain of dynamic pricing.*

