# The Test Instance of Irish Highway Network For Charging Station Location Problems

This repository contains datasets and supporting tools for modeling Ireland's highway network, developed for use in electric vehicle (EV) charging station location optimization studies.

## 📦 Contents

The repository includes:

- `nodes.csv`: Node data including GIS coordinates, classification (e.g. city, town, junction), and population.
- `edges.csv`: Edge data representing links between nodes, including corresponding distances.
- `network_visualisation.png`: A graphical visualization of the constructed highway network.
- `import_network.py`: A Python script to import the dataset into a graph-based structure for further analysis or optimization.

## 📍 Description

This dataset was constructed to support research on the **Charging Station Location Problem (CSLP)** in Ireland. It provides a reasonably accurate, simplified representation of the Irish highway network that captures key travel corridors and urban centers.

### Key Features:
- Designed for optimization and network analysis
- Easy to integrate with Python tools such as NetworkX, Pandas, and Geopandas
- Suitable for testing location models like p-Median, FRLM, or KSP-based formulations
