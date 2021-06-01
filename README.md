# WeatherPy
Utilize a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities

# My Analysis
I created a series of scatter plots to showcase multiple relationships. An example is shown below. I created plots and stated my observations for multiple comparisons such as Humidity vs Latitude, Cloudiness vs Latitude, Wind Speed vs Latitiude. 

Temperature (F) vs. Latitude
Observation: This scatter plot used displays the temperature around the world from -60 latitude to 80 latitude and shows how temperature rises as the latitude gets closer to the equator (0 latitude)
     
I then ran linear regression on each relationship. Although, this time, separating the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). An example is shown below:

Northern Hemisphere - Temperature (F) vs. Latitude
Observation: The r-value of .774 indicates that there is a fairly positive correlation between the latitude coordinates and equator. In other words, the further away the latitude point is from 0, the more likely the max temp will be a lower value.

Southern Hemisphere - Temperature (F) vs. Latitude
Observation: The r-value of .484 indicates that there is a lower positive correlation between the latitude coordinates and equator in the southern hemisphere than the northern hemisphere. In other words, as we keep going south from the equator max temp drops but not as consistently. 


# VacationPy
Use jupyter-gmaps and the Google Places API to create a heat map that displays the humidity levels. 

<img src="https://github.com/Bandelero/python-api-challenge/blob/main/VacationPy/HeatMapwithMarker.png" alt="map" width="600"/>

I then narrowed down my DataFrame to find the ideal weather condition shown below and found the first hotel for each city located within 5000 meters of my coordinates:

- A max temperature lower than 80 degrees but higher than 70.

- Wind speed less than 10 mph.

- Zero cloudiness.

<img src="https://github.com/Bandelero/python-api-challenge/blob/main/VacationPy/InfoBoxTemplate.png" alt="map" width="600"/>


# Conclusion

This was a great learning experience where I had to do an api call on https://api.openweathermap.org/ and also https://maps.googleapis.com/maps/api/place/nearbysearch/json to hit the Google Places API for each city's coordinates.



