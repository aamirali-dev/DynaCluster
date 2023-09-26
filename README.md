# DynaCluster - Dynamic Clustering Algorithm

DynaCluster is a dynamic clustering algorithm designed to efficiently handle data streams and adapt to evolving data distributions. It provides several unique features, including novelty detection, concept drift handling, and the ability to detect clusters with different densities. This repository contains the Python implementation of the DynaCluster algorithm.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Introduction

With the increasing volume of data streams in various domains, there is a need for dynamic clustering algorithms that can adapt to changing data patterns. DynaCluster operates online in two stages: a fast distance-based stage that generates micro-clusters and a density-based stage that groups these micro-clusters into final clusters. It is suitable for handling complex data sets with varying densities, non-convex shapes, and noise.

## Features

- Online dynamic clustering of data streams.
- Novelty detection and concept drift handling.
- Ability to handle clusters of different densities.
- Support for complex data sets and non-convex clusters.
- Python implementation for ease of use.

## Getting Started

To get started with DynaCluster, you need Python installed on your system. You can clone this repository to your local machine:

```bash
git clone https://github.com/aamirali-dev/dynacluster.git
```

After cloning, you can install the required dependencies:

```bash
pip install -r requirements.txt
```

## Usage

You can use DynaCluster in your Python projects as follows:

```python
# Import DynaCluster
from dynacluster import DynaCluster

# Create an instance of DynaCluster
dc = DynaCluster()

# Load your data (replace 'data.csv' with your data file)
dc.load_data('data.csv')

# Cluster the data
dc.cluster()

# Access the final clusters
final_clusters = dc.get_clusters()

# Perform further analysis or visualization
```

## Contributing

If you would like to contribute to DynaCluster, feel free to open issues or submit pull requests. Your contributions and feedback are highly appreciated.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
