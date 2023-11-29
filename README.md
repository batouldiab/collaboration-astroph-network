# Project: Network Analysis and Link Prediction with Python

This project utilizes Python for network analysis using the NetworkX library. It involves various network analysis tasks, visualizations and link prediction model.

## Overview

This project analyzes a given dataset ( [Astro Physics collaboration network](https://snap.stanford.edu/data/ca-AstroPh.html) ) representing connections (scientific collaborations) between nodes (authors papers submitted to Astro Physics category), constructing a network graph based on this data. It conducts various analyses and visualizations to understand the network's structure and characteristics.

## Libraries Used

- `networkx` for constructing and analyzing the network
- `datetime` for timestamp operations
- `nxviz` for network visualizations
- `matplotlib` for plotting graphs
- `pandas` for data manipulation
- `sklearn` for machine learning functionalities
- `torch` for building neural networks
- `torch_geometric` for handling geometric deep learning operations

## Workflow

### Importing Libraries and Dataset
The script begins by importing necessary libraries, including NetworkX, datetime, nxviz, collections, and matplotlib. It then imports the dataset ('astrophy.txt') and creates a network from it.

### Network Analysis and Visualization

#### Network Graph Visualization
It visualizes the network graph using matplotlib, showcasing node connections and networkx layout.

#### Analysis of Network Characteristics
- Calculates the average shortest path diameter.
- Determines the degree distribution of the network and saves the most important nodes based on their degrees.
- Calculates various centrality measures like degree centrality, betweenness centrality, load centrality, and closeness centrality and saves the most important nodes based on the scores.

#### Giant Component Analysis
Identifies the giant component in the network and assesses its size.

#### Node Deletion Experiment
Simulates node removal experiments (10%, 20%, 30%) and measures their impact on the network's structure, visualizing the resultant graphs, and evaluating the giant component's size changes.

### Predicting Future Collaborations
Utilizes machine learning models (Logistic Regression and Graph Convolutional Neural Network) to predict future collaborations in the network based on edge data.

## Usage
Ensure the necessary libraries are installed before running the script. The dataset ('astrophy.txt') is present in the same directory; it is also downloadable from [Astro Physics collaboration network](https://snap.stanford.edu/data/ca-AstroPh.html).

### Running the Script
- Environment Setup: Ensure you have Jupyter Notebook installed or vscode that supports running IPython Notebooks.
- Run the cells within the notebook either individually or by selecting "Run All" from the menu.
  
## Note
- Certain operations in the script may be time-consuming (check the date-time information in the output of the cells). Adjust them based on computational resources.
