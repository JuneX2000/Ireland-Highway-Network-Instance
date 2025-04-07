# The Test Instances For Charging Station Location Problems

This repository contains datasets of test instances of the 25-node network by Simchi-Levi & Berman (1988) and our constructed Irish highway network developed for electric vehicle (EV) charging station location Problems (CSLP) studies.

1. **25-Node Network Instance** – A simplified benchmark instance often used in CSLP literature.
2. **Irish Highway Network** – A realistic representation of Ireland's highway network constructed for solving the CSLP on Irish highway roads.

## Contents

For each instance, the repository includes:
  `Nodes.csv`: Data of nodes.
  `Edges.csv`: Data of edges representing links between nodes.
  `Traffic_Flow.csv`: EV Traffic flow volumes in Origin-Destination matrix.
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
The functional category of the node. For example:
- `"Center"` – nodes that can generate and attract significant travel demand (e.g., cities or towns).  
- `"Connection"` – nodes that serve as intersections or highway junctions.
    
**Note:** Columns with missing data are not included in the dataset

   
### 2. `Edges.csv`

#### 2.1 `Origin` : `<integer>`
The index of starting node of the edge in the graph.
#### 2.2 `Destination` : `<integer>`
The index of ending node of the edge.
#### 2.3 `Edge Length` : `<real>`
The distance required to travel from the origin to the destination.

### 3. `Traffic_Flow.csv`

This CSV file contains the estimated traffic volumes between selected origin-destination (O-D) node pairs in the network.

#### Key Features:
The label of each row represents the origin node index, and label of each column corresponds to destination node index. The value at each cell `(i, j)` indicates the traffic flow volume from node `i` to node `j`.

**Note:** This matrix may be symmetric or asymmetric depending on the method of traffic estimation.

### 4. `Network_Visualisation.pdf`

This pdf file provides a visual representation of the network instance, serves as a quick and intuitive reference for the topology, geographic spread, and structure of the instance.

#### 4.1 Nodes
- In the representation of the Irish highway network, round nodes represent "centers", which serve as demand generators and attractors. Triangle nodes represent highway "connections" (e.g., junctions and intersections).
- In the 25-node network, The size of nodes are propotional to the population weights assigned to each node.
#### 4.2 Edges 
The edges represent undirect connections between nodes.


### 5. `Network_Import.py`

This Python script is used to build the graph-based structure for each test instance and import the traffic flow data file into constructed network structure.

**Create a dictionary-based adjacency list:**
- Each **key** represents a node (as a string).
- Each **value** is another dictionary containing:
  - Keys are indices of neighboring nodes
  - Values are edge lengths

**Import the traffic flow data from `Traffic_Flow.csv` files.**


## References:
1. Simchi-Levi, D., & Berman, O. (1988). A Heuristic Algorithm for the Traveling Salesman Location Problem on Networks. Operations Research, 36(3), 478–484. http://www.jstor.org/stable/170990
