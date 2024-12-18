# Cell Clustering
# Project Overview
This project aims to cluster HeLa cells based on various morphological, positional, and intensity features derived from time-lapse microscopy data. By applying unsupervised clustering techniques - Ensemble methods (e.g., K-Means, DBSCAN, GMM), we can identify distinct groups of cells that share similar characteristics. This approach may help in understanding cell-to-cell variability and identifying phenotypes or states of interest.

# Data Description
The input data is a CSV file containing information extracted from microscopy images. Each row represents a single cell detected at a particular frame. The features include:

Frame Information: id, frame_num
Shape Features: area, major_axis_length, minor_axis_length
Bounding Box Coordinates: min_row_bb, min_col_bb, max_row_bb, max_col_bb
Positional Features: centroid_row, centroid_col
Intensity Features: max_intensity, mean_intensity, min_intensity

# Results Interpretation
Clustering results are exploratory. Clusters may represent:

Cells of different sizes or shapes.
Cells at different stages of the cell cycle (as indicated by intensity or shape).
Spatial groupings that could reflect subtle experimental conditions.
Use the provided visualizations and metrics to interpret and refine your clustering strategy.

# Future Directions
* Dimensionality Reduction:
Implement PCA or UMAP to reduce feature dimensionality before clustering.

* Time-Series Analysis:
Incorporate temporal features (e.g., changes in mean_intensity over frames) to cluster cells by their dynamics over time.

* Model Selection:
Experiment with other clustering algorithms or tune hyperparameters for better performance.
