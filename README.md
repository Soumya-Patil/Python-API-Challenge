## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)

## General info
#### Part I - WeatherPy
This Project runs a Python Script which  Visualizes the weather of 500+ cities across the world of varying distance from the equator; 
Randomly selects  at least 500 unique (non-repeat) cities based on latitude and longitude.
Performs a weather check on each of the cities using a series of successive API calls.
Includes a print log of each city as it's being processed with the city number and city name.
Saves a CSV of all retrieved data and a PNG image for each scatter plot.


Also it looks into a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

A run on  linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

#### Part II - VacationPy

From the Weather Data gathered in Part I , here's a fun exploration to plan future vacations . 
A heat map that displays the humidity for every city from the part I above.
A narrowed down DataFrame to find your ideal weather condition. 
For example:

A max temperature lower than 80 degrees but higher than 70.
Wind speed less than 10 mph.
Zero cloudiness.

A Plot of  hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country

## Technologies
Project is created with:
* Jupyter Notebook
* Python
* CitiPy
* MatPlotlib
* OpenWeatherMap API
* Jupyter-gmaps
* Google Places API 

## Setup
To run this project, Download both the folders locally and have the dependencies installed using Conda .

