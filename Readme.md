# CoGraph: Co-Author Network Visualization

CoGraph is a tool for visualizing co-author networks using data from the DBLP SPARQL endpoint. It allows users to explore the relationships between authors based on their co-authored publications.

## Features

- Fetches co-author information from the DBLP SPARQL endpoint.
- Builds a co-author network up to a specified depth.
- Generates an interactive network visualization using PyVis.

## Installation

To use CoGraph, you need to install the required Python packages. You can install them using pip:

```bash
pip install SPARQLWrapper networkx pyvis
```

## Usage

1. Set the root person URI and the maximum depth for the co-author network in the `main.ipynb` file:

    ```python
    root_person_uri = "https://dblp.org/pid/82/7468"
    max_depth = 2
    ```

2. Run the notebook cells to fetch co-author information, build the network, and generate the visualization.

3. The interactive visualization will be saved in the `output` directory.

## Output

The output will include:

- An HTML file with the interactive network visualization.
- A pickle file containing the network graph object.
