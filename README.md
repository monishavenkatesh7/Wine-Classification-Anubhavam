Here's a draft of the README for your GitHub repository:

---

# Wine Clustering Project

## Overview
This project focuses on clustering wines based on various attributes such as alcohol content, color intensity, and more. Using custom matrix operations and clustering techniques, we calculate Euclidean and Weighted Euclidean distances to group similar wines. The project demonstrates core concepts like matrix standardization, centroid calculation, and weight updates for efficient clustering.

## Features
- **Matrix Class**: Provides methods to load data, standardize, and compute distances.
- **Clustering**: Implements custom clustering based on distance metrics.
- **Dynamic Weight Updates**: Adjusts feature weights during each iteration for optimal clustering.
- **Custom Distance Metrics**: Computes both Euclidean and Weighted Euclidean distances.

## Key Methods
### `load_from_csv(filename)`
Loads data from a CSV file into a matrix for further processing.

### `standardise()`
Standardizes the matrix by scaling each feature.

### `get_distance(other_matrix, row_i)`
Calculates the Euclidean distance between rows of two matrices.

### `get_weighted_distance(other_matrix, weights, row_i)`
Calculates the weighted Euclidean distance using feature weights.

### `get_centroids(data, S, K)`
Determines centroids of clusters based on current data points assigned to clusters.

### `get_separation_within(data, centroids, S, K)`
Calculates the separation within clusters to measure cohesion.

### `get_separation_between(data, centroids, S, K)`
Calculates separation between clusters to measure distinctness.

### `get_new_weights(data, centroids, weights_old, S, K)`
Updates the weights of each feature based on separation metrics.

## Running the Project
1. Clone the repository.
2. Ensure the dataset `Data.csv` is present.
3. Run the `run_test()` function to test clustering across multiple values of K.

## Technologies Used
- Python
- NumPy
- Pandas
- CSV

## Author
Monisha R
