# Fashion-MNIST multi-task CNN

The [notebook](fashion_mnist_multitask_cnn.ipynb), trains a shared PyTorch CNN with two heads on Fashion-MNIST: clothing-class classification and regression of normalized average pixel intensity (“ink”). The [report](fashion_mnist_multitask_cnn_report.pdf) records the loss-weight experiments and results. The saved `.pth` files are the classifier-focused and regressor-focused checkpoints used in the notebook.

| Loss weights (classification, regression) | Test accuracy | Test RMSE |
| --- | ---: | ---: |
| (1, 1) | 91.56% | 0.0363 |
| (1, 1000) | 88.53% | 0.0082 |

These are separate trained models. The notebook downloads Fashion-MNIST through `torchvision` and uses Weights & Biases for experiment logging and sweeps. Run it from this folder with the dependencies in the repository root installed; sweep cells require a W&B account.
