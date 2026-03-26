# Milcom2026-VANET-CybORG

This repository contains data and visualizations for analyzing vehicular ad-hoc networks (VANET) in the Anglova scenario using CybORG.

## Repository Structure

- `data/`: Directory containing the data files.
  - `convoy_scenario.csv`
  - `subnetworks_over_time.yaml`
- `index.html`: Interactive scatter plot visualization.
- `README.md`: Project documentation.

## Files Description

- **data/convoy_scenario.csv**: This file contains traces extracted from the first 16 minutes of the Anglova scenario. These traces capture the movement data of vehicles during this period. The CSV format includes columns such as vehicle_id, y (latitude), x (longitude), t (timestamp), Company, Platoon, Vehicle Type, speed, acceleration, and other attributes describing the vehicles and their states.

- **data/subnetworks_over_time.yaml**: This YAML file describes the sub-networks formed by the vehicles based on the traces in the CSV file. Sub-networks are computed considering connections within a distance of up to 500 meters, and the data is calculated for each second of movement. The structure is a dictionary where keys are timestamps, and values are sub-networks (e.g., subnetwork_0, subnetwork_1) each containing a list of vehicle IDs belonging to that sub-network.

- **index.html**: This HTML file provides an interactive scatter plot that visualizes the movement of vehicles over time. Vehicles are colored according to their sub-network membership, allowing for easy identification of network dynamics. The plot is animated, showing positions at each second, with hover details including vehicle ID and sub-network ID.

To view the visualization, open `index.html` in a web browser or visit the [GitHub Pages site](https://edgarsoliveira1.github.io/Milcom2026-VANET-CybORG-/).