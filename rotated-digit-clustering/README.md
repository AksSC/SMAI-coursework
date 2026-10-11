# Rotated digit clustering

The [notebook](rotated_mnist_clustering.ipynb) extracts Assignment 2, Q7 and its custom PCA/K-means implementations from the original individual submission. It compares border-based orientation heuristics on rotated digit images, then clusters the resulting images and reports adjusted Rand index (ARI) against the provided labels.

The recorded ARI is 0.1544 for raw flattened images and 0.3747 for the first corrected pipeline. That pipeline also applies `StandardScaler` and PCA to 150 components, while the raw baseline does not. The scores therefore compare **whole pipelines**, not rotation alone. Within-cluster sum of squares is also printed, but its values are not directly comparable across these differently scaled spaces.

To run, place the original `X_modified.npy` and `y_true.npy` in this folder, start Jupyter here, and run the notebook from top to bottom. The notebook outputs are cleared. The numerical pipeline was rerun against the original local arrays and reproduced the recorded ARI values. The input arrays are not included pending confirmation that they may be redistributed.
