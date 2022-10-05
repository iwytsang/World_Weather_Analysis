# World Weather Analysis
## Overview
### Purpose
The purpose of the analysis is to enhance the PlanMyTrip app so that it can identify potential travel destinations and nearby hotels based on inputs for weather preferences. In order to create a travel itinterary, four cities were chosen from the same country and the app creates a travel route between the cities and a marker layer map with information about the hotel, city, country, and current weather.

### Analysis

We first created a set of 2,000 random latitudes and longitudes in order to get the nearest city for each latitude and longitude combination. We then retrieved the information from OpenWeatherMap API and created a dataframe to include City Name, Country, Latitude, Longitude, Max Temperature, Humidity, Cloudiness, Wind Speed and Current Weather Description.

As per the below, image, we then prompted the user to enter the minimum and maximum temperatures they would like on their vacation. For our analysis, we chose minimum temperature as 10 degrees F and maximum temperature as 50 degrees F.

![image](https://user-images.githubusercontent.com/108503112/193958943-f3fb1802-a9f5-495e-86bd-47feaae6e7aa.png)

Once the temperatures were filtered out, we then created a marker layer map to include the cities from our dataframe that met the temperature criteria.

![image](https://user-images.githubusercontent.com/108503112/193958292-ab6aca3b-cd83-4bce-9eeb-97332a373b46.png)

## Results

Four cities were chosen from the filtered marker layer map in Iceland, and we used the Google Maps Direction API to create a travel itinerary map of routes between the four cities: Selfoss, Olafsvik, Husavik, and Hofn.

![WeatherPy_travel_map](https://user-images.githubusercontent.com/108503112/193959251-32bd08d5-f39e-459a-a53f-f149c7de789d.png)

We also created a marker map with the information of the hotel name, city, country, and current weather temperature and description in the information box.
![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/108503112/193959257-f9b78ace-5ec0-48bd-beec-6ffc3219c5f1.png)
