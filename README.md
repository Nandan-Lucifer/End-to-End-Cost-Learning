# Deep Graph Edit Distance (Deep-GED)

Deep Graph Edit Distance (Deep-GED) is a Python-based tool for calculating the graph edit distance (GED) between two graphs. It's designed to work with molecular graphs where nodes represent atoms and edges represent bonds. The GED is a measure of the similarity between two graphs, and it quantifies the minimum cost of transforming one graph into another through a sequence of node and edge operations (substitution, insertion, and deletion).

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Usage](#usage)
- [Installation](#installation)

## Overview

Deep-GED provides a framework for computing the GED between two graphs based on a neural network model. It includes various functions for graph manipulation, cost matrix computation, and an end-to-end neural network model to predict GED.

## Features

- Graph edit distance (GED) computation for molecular graphs.
- Neural network model for Boiling Point prediction.
- Customizable node and edge costs.
- Example datasets for training.
- Detailed documentation and examples for usage.

## Usage

You can use Deep-GED by following the code provided in the repository. Make sure you have the required dependencies installed. Here's a brief overview of the code structure:

- `label_to_color`: A function to map node labels to colors.
- `nodes_to_color_sequence`: Generates a color sequence for nodes in a graph.
- `compute_star`: Calculates an extended label for a node based on its neighbors.
- `compute_extended_labels`: Computes extended labels for all nodes in a graph.
- `extract_edge_labels`: Extracts edge labels from a list of graphs.
- `extract_node_labels`: Extracts node labels from a list of graphs.
- `build_node_dictionary`: Builds a dictionary of node labels for encoding.
- `Net`: A neural network model for GED prediction.
- `RegressionMLP`: A regression model for the neural network.
- `create_dataset`: Creates a dataset for training the neural network.
- `regression`: Trains the neural network and returns insights into node and edge costs.
- Visualization of node and edge costs and loss.

For more detailed usage, refer to the code and comments provided.

## Installation

To use Deep-GED, you need Python 3 and the following dependencies:

- PyTorch
- NetworkX
- Matplotlib
- Triangular Losses (required for calculating Triangular Losses)

You can install these dependencies using pip:

```bash
pip install torch networkx matplotlib 
