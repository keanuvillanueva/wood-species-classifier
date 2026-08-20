# Wood Species Classifier

A CNN-based image classification model developed for identifying 20 wood species from wood micrograph images.


## Overview

This project uses transfer learning with VGG16 pretrained on ImageNet. 
The model consists of a customized classification head followed by fine-tuning of the later VGG16 convolutional layers.
The final model achieved an F1 score of 88.43% on the test dataset.


## Model Architecture

- VGG16 pretrained on ImageNet
- Global Average Pooling
- Fully connected classification layers
- Batch Normalization
- Dropout
- Fine-tuning of the later VGG16 layers


## Dataset

The dataset consists of 6,312 curated wood micrograph images covering 20 wood species.

The images were provided for the undergraduate research project and are therefore not included in this repository.

To run the notebook, place the dataset in:

  dataset/wood\_dataset/

with one subdirectory per wood species.


## Results

Precision: 88.67%
Recall: 88.46%
F1 Score: 88.43%


## Files

- `Wood_Classifier.ipynb` — Jupyter notebook containing the model development, training, evaluation, and visualization.
- `models/wood_classifier_final.tflite` — TensorFlow Lite version of the trained model.
