# Brazilian Air Traffic Network

This is a study on brazilian air traffic, in order to analyze the data in graphs, using networkx, we will verify the assortativity of the graph using the attribute "region", analyze the assortativity related to degree, for both in Brazil and their regions networks, analyze the connected components of both Brazil and their regions and create a travel scenario to determine the shortest path of a route of five cities.

# Preparing the Data

The dataset used in this study has all flights in Brazil registered by ANAC, nationally and internationally: https://github.com/alvarofpp/dataset-flights-brazil/tree/main/data

For the study, we treat the data to use only the nacinal brazilian air network, due to the fact that, as the main node attribute for the study is "region", national regions, international airports do not have this attribute defined, causing a filling of empty data, which corresponds to 60% of the data.

# Part 1: Assortativity Graph

For the first part, we will conduct a study on the network assortativity considering as an attribute the REGION where the airport.

To being, we will define the assortativity of this network based on attribute group, the value obtained was greater than zero, so the network is assortative.

After, we build a mixing matrix that refers to the relationship between the aerial lines of the regions of Brazil, where the intersection of the row with the column indicates the percentage of the relationship between the regions. Through it, it is seen that the central-west region is the region that has the busiest airline.

Then, we will generate a similar graph considering as a group the AIRPORT REGION.

<img src="/images/assortativity.png" height="550" width="650">

# Part 2: Degree Assortativity

For the second part, we will perform a bivariate analysis between the degree of the vertex and the average number of neighbors, generate a similar graph for both in Brazil and their regions networks.

- Brazil Network:

<img src="/images/degree_assortativity_brazil.png" height="500" width="750">

- North Region Network:

<img src="/images/degree_assortativity_N.png" height="500" width="750">

- Northeast Region Network:

<img src="/images/degree_assortativity_ND.png" height="500" width="750">

- Midwest Region Network:

<img src="/images/degree_assortativity_CO.png" height="500" width="750">

- Southeast Region Network:

<img src="/images/degree_assortativity_SD.png" height="500" width="750">

- South Region Network:

<img src="/images/degree_assortativity_S.png" height="500" width="750">

Through this analysis, it is evident that the Brazilian air traffic in the country as a whole, and in its regions, are disassortative networks by degrees.

# Part 3: Connected Components

For the third part, we will finding how many connected components are there in the Brazilian air network, characterize by amount and percentage per region.
Through all fire regions, the Brazil have 30 connected components, in percentage, they are separated in:
North: 16.67%, Northeast: 20%, Midwest: 23.33%, Southeast: 20% and South: 20%.

# Part 4: Walks, Paths and Distances

For the fourth and last part, we will create a simulated scenario going from city to city, through five cities (Boa vista, Florianopolis, Vera Cruz, Várzea Grande and Guarulhos), through that, we want the shortest path, describe the path taken and the number of trips taken.

The shortest path taken are Boa vista -> Florianopolis -> Salvador -> Vera Cruz -> Salvador -> Várzea Grande -> Guarulhos. Took 6 trips to reach the destination city.

<img src="/images/shortest_path_scenario.png" height="500" width="700">

## Author
- Luís Fernando Tavares
