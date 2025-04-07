# The Test Instance of Irish Highway Network For Charging Station Location Problems

This repository contains datasets of the test instances of 25-node network by Simchi-Levi & Berman (1988) and our constructed Ireland's highway network, developed for electric vehicle (EV) charging station location Problems (CSLP) studies.

## Contents

The repository includes:

- `nodes.csv`: Node data including GIS coordinates, classification (e.g. city, town, junction), and population.
- `edges.csv`: Edge data representing links between nodes, including corresponding distances.
- `network_visualisation.png`: A graphical visualization of the constructed highway network.
- `import_network.py`: A Python script to import the dataset into a graph-based structure for further analysis or optimization.

## Description

This dataset was constructed to support research on the **Charging Station Location Problem (CSLP)** in Ireland. It provides a reasonably accurate, simplified representation of the Irish highway network that captures key travel corridors and urban centers.

### Key Features:
- Designed for optimization and network analysis
- Easy to integrate with Python tools such as NetworkX, Pandas, and Geopandas
- Suitable for testing location models like p-Median, FRLM, or KSP-based formulations

## 🔗 Download

You can download the data directly here:  
[📥 Click here to download](https://github.com/your-link)

## 📜 License

This dataset is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).  
You are free to use, modify, and share this data for any purpose, including commercial use, with appropriate attribution.

## 📖 Citation

If you use this dataset in your work, please cite it as:

References:
1. Simchi-Levi, D., & Berman, O. (1988). A Heuristic Algorithm for the Traveling Salesman Location Problem on Networks. Operations Research, 36(3), 478–484. http://www.jstor.org/stable/170990
