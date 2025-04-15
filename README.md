# 🌴 Climate Data Exploration & API - SurfsUp

This project analyzes weather data from Honolulu, Hawaii and builds a simple API to serve temperature and precipitation records using Flask and SQLAlchemy.

## 📊 Project Overview

The project is split into two main parts:

### Part 1: Data Analysis in Jupyter Notebook
- Connect to a local SQLite database
- Explore historical weather patterns using Pandas, SQLAlchemy, and Matplotlib
- Analyze precipitation trends and temperature records over the last 12 months
- Identify the most active weather station
- Visualize data including precipitation line plots and temperature histograms

### Part 2: Flask API
- Create multiple API endpoints to serve weather data
- Return JSON responses for precipitation, temperature, and station info
- Accept date ranges via dynamic routes and return summary statistics

## 🔧 Tools Used
- Python
- SQLite
- SQLAlchemy
- Pandas
- Matplotlib
- Flask

## 🗂 File Descriptions
- `climate_analysis.ipynb`: Notebook for running and visualizing all data queries
- `app.py`: Flask app with all API routes
- `hawaii.sqlite`: SQLite database containing climate measurements and station data
- `.gitignore`: Prevents sensitive files like `.env` or keys from being pushed
- `Resources/`: Folder containing source database

## 🔗 Example API Routes

| Route | Description |
|-------|-------------|
| `/` | Welcome page listing all routes |
| `/api/v1.0/precipitation` | Precipitation data for the last year |
| `/api/v1.0/stations` | All station IDs |
| `/api/v1.0/tobs` | Temps from the most active station (last 12 months) |
| `/api/v1.0/<start>` | Temp summary from start date to end of dataset |
| `/api/v1.0/<start>/<end>` | Temp summary for specific date range |
