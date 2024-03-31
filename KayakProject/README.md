# Project 🚧

The team discovered that 70% of their users who are planning a trip would like to have more information about the destination they are going to.

## Objective
The objective of this project is to recommend where people should plan their next holidays. The application should be based on real data about:

- Weather
- Hotels in the area

The application should then be able to recommend the best destinations and hotels based on the above variables at any given time.

## Goals 🎯
As the project has just started, your team doesn't have any data that can be used to create this application. Therefore, your job will be to:

1. Scrape data from destinations.
2. Get weather data from each destination.
3. Get hotels' info about each destination.
4. Store all the information above in a data lake.
5. Creating Maps: Creating two maps, one showcasing the top 5 destinations and another highlighting the top 20 hotels in the area.
6. Extract, transform, and load cleaned data from your data lake to a data warehouse.

## City List
- Mont Saint Michel
- St Malo
- Bayeux
- Le Havre
- Rouen
- Paris
- Amiens
- Lille
- Strasbourg
- Chateau du Haut Koenigsbourg
- Colmar
- Eguisheim
- Besancon
- Dijon
- Annecy
- Grenoble
- Lyon
- Gorges du Verdon
- Bormes les Mimosas
- Cassis
- Marseille
- Aix en Provence
- Avignon
- Uzes
- Nimes
- Aigues Mortes
- Saintes Maries de la mer
- Collioure
- Carcassonne
- Ariege
- Toulouse
- Montauban
- Biarritz
- Bayonne
- La Rochelle

## Data Sources
- Use [Nominatim](https://nominatim.org/) to get the GPS coordinates of all the cities (no subscription required). Documentation: [Nominatim API](https://nominatim.org/release-docs/develop/api/Search/)
- Use [OpenWeatherMap](https://openweathermap.org/appid) (you have to subscribe to get a free API key) and [One Call API](https://openweathermap.org/api/one-call-api) to get some information about the weather for the 35 cities and put it in a DataFrame.
- Scrape Booking.com for hotel data. Since Booking Holdings doesn't have aggregated databases, it will be much faster to scrape data directly from booking.com. You can scrape as much information as you want, but we suggest that you get at least:
  - Hotel name
  - URL to its booking.com page
  - Coordinates (latitude and longitude)
  - Score given by the website users
  - Text description of the hotel

## ETL
Once you upload your data onto S3, it will be better for the next data analysis team to extract clean data directly from a Data Warehouse. Therefore, create a SQL Database using AWS RDS, extract your data from S3, and store it in your newly created DB.


