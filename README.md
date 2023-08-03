# **Python API - Weather Analysis**

**Background**

In this project, Python requests, APIs, and JSON traversals are being used to answer a fundamental question: "What's the weather like as we approach the equator?" The answer is obviously "hotter" but we have used the data to prove the answer.

**Part I – WeatherPy**

A Python script was created to visualize the weather of cities across the world of varying distance from the equator. To accomplish this, a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), were utilized to create a representative model of weather across world cities.

A series of scatter plots to showcase the following relationships:

- Latitude vs. Temperature
- Latitude vs. Humidity
- Latitude vs. Cloudiness
- Latitude vs. Wind Speed

A linear regression on each relationship is shown into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

- Northern Hemisphere - Temperature vs. Latitude
- Southern Hemisphere - Temperature vs. Latitude
- Northern Hemisphere - Humidity vs. Latitude
- Southern Hemisphere - Humidity vs. Latitude
- Northern Hemisphere - Cloudiness vs. Latitude
- Southern Hemisphere - Cloudiness vs. Latitude
- Northern Hemisphere - Wind Speed vs. Latitude
- Southern Hemisphere - Wind Speed vs. Latitude

**Part II - VacationPy**

- Created a heat map that displays the humidity for every city from the part I.
- Narrowed down the DataFrame to find the ideal weather condition. For example:
  - A max temperature lower than 80.6 degrees but higher than 70.
  - Wind speed less than 10 mph.
  - Zero cloudiness.
- Used Google Maps API to find the first hotel for each city located within 5000 meters radius of the coordinates.
- Plotted the hotels on top of the humidity heatmap with each pin containing the  **Hotel Name** ,  **City** , and  **Country**.
