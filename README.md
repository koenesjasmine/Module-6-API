# World Weather Analysis

## Project Overview
PlanMyTrip has requested a dataset that will allow them to reccomment ideal hotels based on weather preferences. We will manage several APIs to provide a map of locations that meet a set of parameters provided by the customer. This map will include city locations as well as hotels nearby and the local weather recently (max temp, humidity, description [cloudy, sunny, rain, etc.])

### expected steps
1. generate a large list (2000) of random longitude and latitude
2. use citipy to associate the nearest city to the pre-developed locations
3. use API from OpenWeather and import the current local weather from the cities determined in previous step
4. get input from customer on min and max temperature ranges they would like their vacation spot to have
5. use google maps API to find nearby hotels for this filtered list of cities. leverage offers for locations that do not return a hotel
6. use gmaps to present a map with the potential city locations and hotels within reccomended pins. 
7. select 4 cities from the list of vacation itinerary options
8. use gmaps to create a route between the selected offer cities, looping back to the starting city. display this map. 

## Challenges

One major challenge that was indirectly related to the project was that I could not get gmaps and widgets to perform correctly with my key. Eventually, what worked was to explicitly specify the version of ipywidgets in my environment to make it work. 

## Data Summary Results
- The WeatherPy_Database contains over 700 cities found from our 2000 lat/long pairs.
- WeatherPy_vacation contains 327 cities; most, but not all, of which have hotels (this is filtered based on user input of min 65 and max 85 degrees F).

![WeatherPy_Vacation_map](C:\Users\jasmi\Desktop\Class\Module-6-\Module-6-API\Vacation_Search\WeatherPyShot.PNG)

- Weather_Vacation_Map includes travel paths shown on the map

![WeatherPy_travel_map](C:\Users\jasmi\Desktop\Class\Module-6-\Module-6-API\Vacation_Itinerary\TavelMap.PNG)

![WeatherPy_travel_map_markers](insert url)

## Conclusion
APIs are a powerful skill to add to the toolbelt. access to data across the web enables so many possibilities for future data analysis and exploration. 
additionally gmaps and citipy are both very useful libraries for geographic data and ability to display. 