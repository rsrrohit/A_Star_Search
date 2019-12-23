# A_Star_Search
Implemented A start search algorithm for finding a shortest path between any two US cities.

program should be run on the command line like this:

./route.py [start-city] [end-city] [cost-function]
where:

• start-city and end-city are the cities we need a route between (format given in road-segments.txt). e.g. New_York,_New_York and Los_Angeles,_California

• cost-function is one of following:

segments - It tries to find a route with the fewest number of "turns" (i.e. edges of the graph)
distance - It tries to find a route with the shortest total distance
time - It tries to find the fastest route, for a car that always travels at the speed limit
mpg - It tries to find the most economical route, for a car that always travels at the speed limit and
whose mileage per gallon (MPG) is a function of its velocity (in miles per hour), as follows:
MPG(v) = 400 * v/150 * (1 − v/150)^4

The output of the program is a nicely-formatted, human-readable list of directions, including travel
times, distances, intermediate cities, and highway names, similar to what Google Maps or another site might
produce. In addition, the last line of output has the following output about the route:
[total-segments] [total-miles] [total-hours] [total-gas-gallons] [start-city] [city-1] [city-2] ... [end-city]

Extra files:-
This is a simple dataset of North American (though mostly U.S.) major roads.

city-gps.txt contains one line per city, with three fields per line, 
delimited by spaces. The first field is the city, followed by the latitude,
followed by the longitude.

road-segments.txt has one line per road segment connecting two cities.
The space delimited fields are:
- first city
- second city
- length (in miles)
- speed limit (in miles per hour)
- name of highway
