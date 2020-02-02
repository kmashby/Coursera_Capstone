# Coursera_Capstone
This repository was created to store projects for the Coursera Applied Data Science Capstone course.

# Introduction
  
A client wants to open a new pet store in Chicago, IL and approached our company to find the best location. There are already four existing pet stores in Chicago, although one recently closed, and another specializes in aquariums. Our goal is to identify neighborhoods that are similar to the other neighborhoods with the two pet stores as these may offer ideal locations for a new pet store. 
To accomplish this goal, I will use the Foursquare API to download venue data for each neighborhood in Chicago and then cluster the neighborhood data using k-means. Neighborhoods within the same cluster as those with existing pet stores could provide the best location for a new pet store.
 
#Data
The Foursquare API and the City of Chicago website were used to collect data for this project. 
  
Chicago neighborhood names and boundary data can be downloaded from the Chicago city website (https://data.cityofchicago.org/resource/igwz-8jzy.json). The boundaries information is provided as a multipolygon with multiple latitude and longitude points for each neighborhood. A centroid point can be calculated from the boundary points and the latitude and longitude of the centroid point can be used as the location for the neighborhood in the Foursquare API query. 
 
The Foursquare API explore venues query returns venue names, locations, and categories for venues within a certain radius of a given location. Venues are grouped into categories such as Pet Shop, Sandwich Place, Park, Bus Station, Bakery, and Mexican Restaurant. For example, the store “Family Dollar” is in the category “Discount Store” and “Subway” is in the “Sandwich Place” category. 
 
The venue information can be grouped by neighborhood and used to segment neighborhoods into clusters with similar frequencies of venue categories. 


