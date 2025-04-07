# The Test Instance of Irish Highway Network For Charging Station Location Problems

This repository contains datasets of the test instances of the 25-node network by Simchi-Levi & Berman (1988) and our constructed Irish highway network instance, developed for electric vehicle (EV) charging station location Problems (CSLP) studies.

## Contents

The repository includes two folders sepratedly for the 25-node network instance and the Irish highway network instance:

1. **25-Node Network Instance** – A simplified benchmark instance often used in CSLP literature.
2. **Irish Highway Network** – A realistic representation of Ireland's highway network constructed for solving the CSLP on Irish highway roads.

---

## 📂 Repository Structure

```text
├── 25-node network/
│   ├── nodes_25.csv
│   ├── edges_25.csv
│   ├── network_visualisation_25.png
│   └── import_25_node_network.py

├── Irish highway network/
│   ├── nodes_ireland.csv
│   ├── edges_ireland.csv
│   ├── network_visualisation_ireland.png
│   └── import_ireland_network.py





- `nodes.csv`: Node data including GIS coordinates, classification (e.g. city, town, junction), and population.
- `edges.csv`: Edge data representing links between nodes, including corresponding distances.
- `network_visualisation.png`: A graphical visualization of the constructed highway network.
- `import_network.py`: A Python script to import the dataset into a graph-based structure for further analysis or optimization.

## References:
1. Simchi-Levi, D., & Berman, O. (1988). A Heuristic Algorithm for the Traveling Salesman Location Problem on Networks. Operations Research, 36(3), 478–484. http://www.jstor.org/stable/170990
