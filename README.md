# The Test Instance of Irish Highway Network For Charging Station Location Problems

This repository contains datasets of test instances of the 25-node network by Simchi-Levi & Berman (1988) and our constructed Irish highway network developed for electric vehicle (EV) charging station location Problems (CSLP) studies.

1. **25-Node Network Instance** – A simplified benchmark instance often used in CSLP literature.
2. **Irish Highway Network** – A realistic representation of Ireland's highway network constructed for solving the CSLP on Irish highway roads.

## Contents

For each instance, the repository includes:
  `Nodes.csv`: Data of nodes.
  `Edges.csv`: Data of edges representing links between nodes.
  `Network_Visualisation.pdf`: A graphical visualization of the network instance.
  `Network_Import.py`: A Python script to import the graph-based structure for further analysis or optimization.

## The file format

### 1. `Nodes.csv`
#### 1.1 `Node` : `<integer>` 
The index for each node in the network.
#### 1.2 `Latitude` : `<string>`  
Latitude of the node in degrees, minutes, and seconds format.
#### 1.3 `Longitude` : `<string>`
Longitude of the node in degrees, minutes, and seconds format.
#### 1.4 `Degree` : `<integer>`
The number of edges the node has in the network.
#### 1.5 `Settlement` : `<string>`  
The name of the town or city close to the node.
#### 1.6 `Population` / `Population Weight` : `<integer>` 
The population represents the number of residents in the settlement, used to determine the classification of the node.
A alternative representation is the assigned population weight, commonly used to estimate potential EV demand or origin-destination weights.
#### 1.7 `Classification` : `<string>`  
    The functional category of the node, such as "Center" that can generate and attract traveling demands or "Connection" that serves as intersections and junctions in the instance.
    
**Note:** Columns with missing data are not included in the dataset

   
### 2. `Edges.csv`
#### 2.1 Origin: <integer>
The index of starting node of the edge in the graph.
#### 2.2 Destination: <integer>
The index of ending node of the edge.
#### 2.3 Edge Length: <real>
The distance required to travel from the origin to the destination.




- `nodes.csv`: Node data including GIS coordinates, classification (e.g. city, town, junction), and population.
- `edges.csv`: Edge data representing links between nodes, including corresponding distances.
- `network_visualisation.png`: A graphical visualization of the constructed highway network.
- `import_network.py`: A Python script to import the dataset into a graph-based structure for further analysis or optimization.

## References:
1. Simchi-Levi, D., & Berman, O. (1988). A Heuristic Algorithm for the Traveling Salesman Location Problem on Networks. Operations Research, 36(3), 478–484. http://www.jstor.org/stable/170990
