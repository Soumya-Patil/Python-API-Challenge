Part I - WeatherPy
Created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this,  a Python library CitiPy and  the OpenWeatherMap API was Utilized , and finally representative model of weather across world cities was created.

The Following Relationships were Showcased - 

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

Also ran a  linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude) :

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

To optimize the code,  a function was created for the  linear regression plots.

Randomly selected at least 500 unique (non-repeat) cities based on latitude and longitude.
Performed a weather check on each of the cities using a series of successive API calls.
Included a print log of each city as it's being processed with the city number and city name.
Saved a CSV of all retrieved data and a PNG image for each scatter plot.


Part II - VacationPy
A fun exploration  with weather data to plan future vacations. Used jupyter-gmaps and the Google Places API for this part.



Created a heat map that displays the humidity for every city from the part I of the homework.

Narrowed down the DataFrame to find your ideal weather condition. For example:


A max temperature lower than 80 degrees but higher than 70.


Wind speed less than 10 mph.


Zero cloudiness.


Dropped any rows that don't contain all three conditions. You want to be sure the weather is ideal.

Used Google Places API to find the first hotel for each city located within 5000 meters of the coordinates.

Plotted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

