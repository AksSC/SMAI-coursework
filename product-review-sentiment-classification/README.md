# Product-review sentiment classification

The [notebook](product_review_sentiment.ipynb), uses provided bag-of-words product-review features to classify sentiment. It fits sklearn decision trees and random forests, tunes them with `GridSearchCV` on the supplied train/validation split, and evaluates balanced accuracy on the test split. The notebook imports the included `pretty_print_sklearn_tree.py` helper from the course starter material.

| Model | Test balanced accuracy |
| --- | ---: |
| Tuned decision tree | 0.749 |
| Tuned random forest | 0.837 |
