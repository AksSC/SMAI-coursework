# Rotated digit clustering

The [notebook](rotated_mnist_clustering.ipynb) compares border-based orientation heuristics on rotated digit images, then clusters the resulting images and reports adjusted Rand index (ARI) against the provided labels.

The recorded ARI is 0.1544 for raw flattened images and 0.3747 for the first corrected pipeline. That pipeline also applies `StandardScaler` and PCA to 150 components, while the raw baseline does not. The scores therefore compare **whole pipelines**, not rotation alone. Within-cluster sum of squares is also printed, but its values are not directly comparable across these differently scaled spaces.
