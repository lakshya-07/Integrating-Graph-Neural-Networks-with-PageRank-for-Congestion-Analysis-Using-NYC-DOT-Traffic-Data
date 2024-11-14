# Integrating-Graph-Neural-Networks-with-PageRank-for-Congestion-Analysis-Using-NYC-DOT-Traffic-Data

## Table of Contents
- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset Description](#dataset-description)
- [Data Preprocessing](#Data-Preprocessing)
- [Integration of Graph Neural Networks](#Integration-of-Graph-Neural-Networks)
- [Results and Visualizations](#results-and-visualizations)
- [Conclusions](#conclusions)
- [Requirements](#requirements)
- [Installation](#installation)

## Project Overview
This project presents an innovative approach to traffic congestion analysis in urban environments by enhancing the traditional PageRank algorithm with Graph Neural Networks (GNNs). The aim is to evaluate and rank road network intersections based on their importance and traffic congestion levels, providing data-driven insights for better urban traffic management.

## Objectives
The main objectives of this research are:
1. To incorporate GNNs for learning node embeddings that capture topological and dynamic features of road networks.
2. To apply the enhanced PageRank algorithm to identify key intersections with significant traffic impact.
3. To visualize the influence of congestion on the relative importance of junctions using traffic volume data.

## Dataset Description
The dataset used in this research comes from the **New York City Department of Transportation (NYC DOT)**. It includes traffic sample volume counts at various bridge crossings and roadways. Key features of the dataset:
- **Columns**:
  - `RequestID`: Unique identifier for each traffic count request.
  - `boro`: Borough where the traffic count was conducted.
  - `yr`, `m`, `d`, `HH`, `mm`: Date and time information.
  - `vol`: Total traffic volume counted in 15-minute increments.
  - `SegmentId`: Identifier for each street segment.
  - `WktGeom`: Geometry data representing the road segment.
- The dataset provides crucial information for simulating traffic loads and integrating them with network graphs.

## Basic Methodology
## Data Preprocessing
- Loading and cleaning the dataset.
- Converting `WktGeom` into `shapely` geometries for spatial operations.

## Integration of Graph Neural Networks
- Using GNNs to learn node embeddings that incorporate both static topological features and dynamic traffic volume.
- Modifying the PageRank algorithm to account for learned GNN node representations.

## Results and Visualizations
- Nodes with higher PageRank values under congested conditions were ranked.
- Visual maps displaying the most congested routes and intersections with time.

## Conclusions
- Incorporating GNNs into the PageRank algorithm improved the accuracy of traffic congestion prediction.
- The results demonstrate that the dynamic adjustment of PageRank values based on node embeddings offers better insights into traffic management.

## Requirements
- Python 3.8 or higher
- Libraries:
  - `numpy`
  - `pandas`
  - `networkx`
  - `osmnx`
  - `folium`
  - `matplotlib`
  - `shapely`
  - `geopandas`
  - `scikit-learn`
  - `torch`
  - `torch-geometric`

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/lakshya-07/Integrating-Graph-Neural-Networks-with-PageRank-for-Congestion-Analysis-Using-NYC-DOT-Traffic-Data.git
   cd Integrating-Graph-Neural-Networks-with-PageRank-for-Congestion-Analysis-Using-NYC-DOT-Traffic-Data
