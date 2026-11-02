# mnist-low-data-pytorch

How much do architecture and data augmentation matter when labels are scarce? This project trains PyTorch models on a balanced 1,000-image MNIST subset (100 per digit) and compares them against full-data training.

| Experiment | Params | Test acc. |
|---|---|---|
| MLP, 1k subset | 269,322 | 89.36% |
| CNN, 1k subset | 105,866 | 93.89% |
| CNN, 1k subset + augmentation | 105,866 | 96.58% |
| CNN, full 60k | 105,866 | 98.95% |

Single seed, fixed hyperparameters, final-epoch accuracy on the 10k test set. See the notebook for details and limitations.

## Run it
Open `mnist_low_data_pytorch.ipynb` in Colab or Jupyter and run all cells (MNIST downloads automatically).