# Visualizing MNIST Handwritten Digits Using Multi-Dimensional Scaling (MDS)
  # Introduction
In this project, we utilize Multi-Dimensional Scaling (MDS) to transform the MNIST handwritten digit dataset into a 2D space. MNIST contains grayscale images of handwritten digits (0-9) with dimensions of 28x28 pixels, resulting in 784-dimensional feature vectors.

# Purpose
The primary aim is to reduce the MNIST dataset's dimensionality from 784 to 2 dimensions with MDS. This dimensionality reduction helps visualize high-dimensional data in a 2D plane while preserving the distances between data points as accurately as possible.

# Implementation
  # Data Loading:

MNIST data is fetched from gzip-compressed files (train-images-idx3-ubyte.gz for images and train-labels-idx1-ubyte.gz for labels).
Custom functions (read_images and read_labels) are used to read the dataset.
  # Applying MDS:

Compute pairwise Euclidean distances to generate a distance matrix.
Create the centering matrix and compute the B matrix based on MDS.
Perform eigenvalue decomposition on the B matrix to get eigenvalues and eigenvectors.
Select the top eigenvalues and corresponding eigenvectors to project the data into a 2D space.
 # Visualization:

Plot the 2D projection of the dataset using matplotlib.
Different digits (0-9) are represented with distinct colors to show the clustering patterns.
 # Outcome
MDS effectively reduces the MNIST dataset from 784 to 2 dimensions.
The 2D projection reveals clusters of different digits, highlighting MDS's ability to maintain data structure.
