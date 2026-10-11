# Product-review sentiment classification

The [notebook](product_review_sentiment.ipynb), from Assignment 4, Q3, uses provided bag-of-words product-review features to classify sentiment. It fits sklearn decision trees and random forests, tunes them with `GridSearchCV` on the supplied train/validation split, and evaluates balanced accuracy on the test split. The notebook imports the included `pretty_print_sklearn_tree.py` helper from the course starter material.

| Model | Test balanced accuracy |
| --- | ---: |
| Tuned decision tree | 0.749 |
| Tuned random forest | 0.837 |

To run, place the course-provided `x_train.csv`, `y_train.csv`, `x_valid.csv`, `y_valid.csv`, `x_test.csv`, and `y_test.csv` in `data_product_reviews/`, then start Jupyter from this folder. The CSVs are not included pending confirmation that they may be redistributed. Results above are from the saved notebook and have not been rerun for this repository.
