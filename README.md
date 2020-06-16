# python-api-challenge
Repository for Python-API homework
Part I - WeatherPy



you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.
Your first requirement is to create a series of scatter plots to showcase the following relationships:

Temperature (F) vs. Latitude
Humidity (%) vs. Latitude
Cloudiness (%) vs. Latitude
Wind Speed (mph) vs. Latitude

After each plot add a sentence or two explaining what the code is and analyzing.
Your second requirement is to run linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
Northern Hemisphere - Wind Speed (mph) vs. Latitude
Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots explain what the linear regression is modeling such as any relationships you notice and any other analysis you may have.
Optional You will be creating multiple linear regression plots. To optimize your code, write a function that creates the linear regression plots.
Your final notebook must:

Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
Perform a weather check on each of the cities using a series of successive API calls.
Include a print log of each city as it's being processed with the city number and city name.
Save a CSV of all retrieved data and a PNG image for each scatter plot.




Part II - VacationPy
Now let's use your skills in working with weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.



Narrow down the DataFrame to find your ideal weather condition. For example:


A max temperature lower than 80 degrees but higher than 70.


Wind speed less than 10 mph.


Zero cloudiness.


Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.


Note: Feel free to adjust to your specifications but be sure to limit the number of rows returned by your API requests to a reasonable number.




Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.


Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.






Inferences from the WeatherPy Analysis:

•	Northern (NH) and Southern (SH) Hemispheres Comparison
o	In the NH there is negative correlation between latitude and temperature with higher temperature around locations closer to the equator, and decreases as you move up away from the equator
o	In the SH there is positive correlation between latitude and temperature with temperature increasing as you move closer to the equator 
o	With the other variables namely: humidity, cloudiness, and wind speed there is little or no correlation between them and latitude in both NH and SH. The effect of latitude on these other variables is statistically insignificant with all having a R-Square value of less than 1%. 
