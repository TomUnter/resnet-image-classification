# Residual Networks for Image Classification

A practical deep-learning project completed as part of a
Mathematical Data Science course.

The project explores image classification with TensorFlow/Keras
and compares a residual convolutional neural network with a
non-residual convolutional baseline.

## Project overview

The notebook contains:

- Implementation of configurable residual blocks with skip connections.
- Construction of a residual convolutional neural network.
- Implementation of a plain convolutional comparison model.
- Preprocessing of MNIST and Fashion-MNIST images.
- Model training with the Adam optimiser and categorical cross-entropy.
- Analysis and visualisation of training and validation loss and accuracy.

The project demonstrates practical experience with neural-network
implementation, data preprocessing, model training, and the
interpretation of learning curves.

## Technologies

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Jupyter Notebook / Google Colab

## Notebook

`P8ResNet.ipynb`

The notebook includes model definitions, data preprocessing,
training code, and analysis of saved training histories.

## Data

The project uses MNIST and Fashion-MNIST.

The preprocessing code:

- Normalises pixel values to the range [0, 1].
- Resizes images to 32 × 32 pixels.
- Expands grayscale images to three channels.
- Converts class labels to one-hot encoding.

The datasets are loaded through the Keras dataset interface.

## Model comparison

The residual model uses convolutional blocks with skip connections.
The plain comparison model does not use skip connections.

The implemented architectures also differ in activation placement,
batch normalisation, and aspects of their downsampling blocks.
The comparison should therefore be interpreted as a comparison
between these specific implementations, rather than an isolated
ablation of skip connections.

## Running the notebook

1. Download the notebook or clone this repository.
2. Open `P8ResNet.ipynb` in Google Colab or Jupyter.
3. Ensure TensorFlow, NumPy, and Matplotlib are available.
4. Review file paths before running the analysis cells.
5. Run the model and preprocessing cells before starting training.

A GPU is recommended for the larger training configurations.

The plotting cells require CSV files containing saved training
histories. These must either be provided separately or generated
by the corresponding training runs.

## Limitations and project context

This repository documents an educational project originally
developed in Google Colab. Compatibility with current library
versions has not yet been revalidated.

In the original training code, the Fashion-MNIST test split is
passed to Keras as validation data. The corresponding curves
therefore do not constitute an additional, untouched final test
evaluation.

The project focuses on image classification, not on omics data.
It provides a practical foundation in deep learning that can be
extended to other scientific data-analysis tasks.

## Academic context

Practical project within the Mathematical Data Science
qualification, complementing an interdisciplinary background
in Integrated Life Sciences and computational biology.
