# Brazilian-air-traffic-network

This is a study on brazilian air traffic, in order to analyze the data in graphs, using networkx, we will verify the assortativity of the graph using the attribute "region", analyze the assortativity related to degree, both in Brazil and their regions, analyze the connected components of both Brazil and their regions and create a travel scenario to determine the shortest path of a route of five cities.

# Preparing the Data

The dataset used in this study has all flights in Brazil registered by ANAC, nationally and internationally: https://github.com/alvarofpp/dataset-flights-brazil/tree/main/data

For the study, we treat the data to use only the nacinal brazilian air network, due to the fact that, as the main node attribute for the study is "region", national regions, international airports do not have this attribute defined, causing a filling of empty data, which corresponds to 60% of the data.

# Part 1: Assortativity Graph

For the first part, we will conduct a study on the network assortativity considering as an attribute the REGION where the airport.



Then, we will generate a similar graph considering as a group the AIRPORT REGION.

<img src="/images/assortativity.png" height="500" width="620">

# Part 2: Degree Assortativity



# Part 3: Connected Components



# Part 4: Walks, Paths and Distances
