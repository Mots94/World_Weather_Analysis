# World_Weather_Analysis
Using Python and APIs to visualize weather data for vacationing

## Purpose
When picking a vacation destination, there are a few key factors that often determine the location.  Some examples of those factors are the weather, availability of lodging, and ability to travel between different cities.  In this analysis, weather information and lodging were gathered using the Open Weather API and Google Places API.  This information was visualized using the Google Maps API, along with directions between locations.  

## Overview
Two thousand random latitudes and longitudes were generated, which were then joined together to create a list of latitude and longitude pairs. This list was interated over and the citipy module was used to determine the nearest city to each coordinate pair.  This yielded a list of 742 cities, which was also interated over to collect current weather data. The Open Weather API was used to collect information such as maximum temperature, humidity, and wind speed.  A user input was created for the minimum and maximum preferable temperature so city information could be further filtered to include only cities that an individual would want to visit.  This filtered array of cities was interated over to collect the nearest hotel for each city using the Google Places API.  City, weather, and hotel information were then visualized on a marker map using the Google Maps API.  
