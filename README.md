# Python API Challenge

## Overview

This project consists of two parts: **WeatherPy** and **VacationPy**. The purpose is to analyze weather patterns across various cities and use this data to plan potential vacation destinations.

## Part 1: WeatherPy

### Objective

WeatherPy utilizes Python, the Citipy library, and the OpenWeatherMap API to gather and visualize weather data for over 500 randomly selected cities worldwide.

### Requirements

1. **Generate Random City Data**

   - Use the Citipy library to identify cities based on random latitude and longitude values.
   - Retrieve weather data from the OpenWeatherMap API.

2. **Create Scatter Plots to Show Weather Relationships**

   - Latitude vs. Temperature
   - Latitude vs. Humidity
   - Latitude vs. Cloudiness
   - Latitude vs. Wind Speed

3. **Compute Linear Regression for Weather Relationships**

   - Separate data into Northern Hemisphere and Southern Hemisphere categories.
   - Perform linear regression for:
     - Temperature vs. Latitude
     - Humidity vs. Latitude
     - Cloudiness vs. Latitude
     - Wind Speed vs. Latitude
   - Display regression lines, equations, and R-squared values.

4. **Analyze Findings**

   - Summarize relationships between latitude and weather variables.
   - Explain key insights derived from the regression analysis.

## Part 2: VacationPy

### Objective

VacationPy leverages weather data to identify ideal vacation destinations based on temperature and visualizes these locations using mapping tools.

### Requirements

1. **Map City Locations**

   - Display all cities from the dataset using Hvplot and Geoapify APIs.
   - Scale point sizes based on humidity levels.

2. **Find Nearby Hotels**

   - Use the Geoapify API to locate the nearest hotel within a 10,000-meter radius of each city.
   - Create a DataFrame to store city name, country, coordinates, humidity, and hotel name.

3. **Generate Vacation Map**

   - Display a map with markers for cities.
   - Include hover messages with city name, country, and hotel information.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- SciPy
- OpenWeatherMap API
- Geoapify API
- Citipy Library
- Hvplot

## Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/dagimg16/python-api-challenge.git
   ```
2. Install the required libraries:
   ```sh
   pip install pandas numpy matplotlib scipy hvplot requests citipy 
   ```
3. Obtain API Keys:
   - OpenWeatherMap API Key
   - Geoapify API Key
4. Create a `api_keys.py` file and store your API keys:
   ```
   weather_api_key =your_openweather_api_key
   geoapify_key =your_geoapify_api_key
   ```
5. Run the Jupyter Notebooks `WeatherPy.ipynb` and `VacationPy.ipynb` step by step.

## Results

The project successfully visualizes weather trends and identifies optimal vacation locations based on weather preferences.

## Resources & Acknowledgments
  - OpenWeather API: https://openweathermap.org/api
    - Usage: Used for retrieving weather data for data analysis.
    - License: Free tier for non-commercial use, with limitations on the number of requests.  
  - Geoapify API: https://www.geoapify.com/
    - API Documentation: https://apidocs.geoapify.com/
    - Usage: Used for geospatial data processing and mapping in the project.
    - License: Free tier available with limitations on the number of requests.   
    
## License
  - Feel free to use and modify this script for your own learning.
