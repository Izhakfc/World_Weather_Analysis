# World_Weather_Analysis

## Overview 
Design a user_interface program that allows users input their desired min and max temperatures in order to filter through a set of cities that fulfill those requirements. Afterwards, the program will perform requests on the OpenWeather API to get other weather characteristics from each filtered city. Then using GOOGLE APIs display the location and info of each city and design a travel itinerary for the user.

## Get the weather characteristics for each city
Using the np.random.uniform function we obtained 2,000 random latitude and longitude locations to obtain city names using the citipy module. After obtaining the cities, requests in the OpenWather API were made in order to get weather characteristics for each of this cities and added them into a dataframe and then stored the dataframe into a csv file. The dataframe structure is shown below:

-- Figure --

## User-interface to get users narrow their travel searches based on temperature
The customer was asked for information to narrow down the search like based on the desired min and max temperature. After filtering the cities by the temperature parameters, a new column was added in order to store hotel names for each of the cities from GOOGLE MAP API, cities with no hotel names where deleted from the dataframe as shown below.
--Figure--
Using the new data frame an info box and a gmaps marker layer was created to display the location of each of the hotels.
--Figure--

## Create a travel itinerary and display the route
Using the information collected from the previous step the customer was asked to chose 4 destination cities that he desires to travel. The  suser defined the start of his travel and enumerated the stops for each city, finally, a gmaps direction layer was created showing the route to follow with the DRIVING option.
--Figure--
