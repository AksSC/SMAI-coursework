# SMAI coursework: selected studies

Three studies from my individual Statistical Methods in AI coursework. Each folder contains the study code and its README.

| Study | What is in the folder | Recorded result |
| --- | --- | --- |
| [Rotated digit clustering](rotated-digit-clustering/) | Orientation heuristics, custom PCA and K-means, and clustering evaluation | Adjusted Rand index: 0.1544 for raw images; 0.3747 for the transformed pipeline |
| [Fashion-MNIST multi-task CNN](fashion-mnist-multitask-cnn/) | Clothing classification and image-ink regression with a shared PyTorch CNN | 91.56% test classification accuracy (classification-focused model); 0.0082 test regression RMSE (regression-focused model) |
| [Product-review sentiment classification](product-review-sentiment-classification/) | Bag-of-words decision trees and random forests with validation-set tuning | 0.837 test balanced accuracy for the tuned forest |

The clustering comparison changes scaling and PCA as well as orientation; it does **not** isolate the effect of rotation. The CNN results are from different loss-weight settings, not one model achieving both figures. See each study README for method and data notes.

The sentiment notebook uses course starter material and helper code; its sklearn models were tuned in the notebook. Dependencies are listed in [requirements.txt](requirements.txt).
