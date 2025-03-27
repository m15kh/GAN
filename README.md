# Vanilla Autoencoder

This project implements a simple vanilla autoencoder using PyTorch. The autoencoder is trained on the MNIST dataset to reconstruct input images.

## Project Structure

- **`pipeline.py`**: Contains the training pipeline for the autoencoder. 
- **`net.py`**: Defines the architecture of the autoencoder.
- **`inference.py`**: Performs inference using the trained autoencoder model.
- **`dataloader.py`**: Handles loading and preprocessing of the MNIST dataset.
- **`checkpoints/`**: Directory to save trained model checkpoints.
- **`img-output/`**: Directory to save output images during inference.

## Requirements
 
- Python 3.8+
- PyTorch
- torchvision
- matplotlib
- numpy

Install the required packages using:
```bash
pip install torch torchvision matplotlib numpy
```

## Training the Model

1. Run the `pipeline.py` script to train the autoencoder:
   ```bash
   python pipeline.py
   ```
2. The trained model will be saved in the `checkpoints/` directory.

## Running Inference

1. Run the `inference.py` script to generate predictions:
   ```bash
   python inference.py
   ```
2. Output images will be saved in the `img-output/` directory.

## Dataset

The MNIST dataset is automatically downloaded and used for training and validation.

## Notes

- Ensure that the `content/` directory is included in the `.gitignore` file to avoid committing large datasets.
- Modify hyperparameters such as learning rate, batch size, and number of epochs in the respective scripts as needed.
