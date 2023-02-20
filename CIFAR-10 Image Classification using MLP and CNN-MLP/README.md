# CIFAR-10 Image Classification using MLP and CNN-MLP

This repository contains code for image classification of CIFAR-10 dataset using MLP and CNN-MLP models in Keras.

## Dataset

The CIFAR-10 dataset consists of 60,000 32x32 color images in 10 classes, with 6,000 images per class. There are 50,000 training images and 10,000 test images. The dataset is divided into five training batches and one test batch, each with 10,000 images. The test batch contains exactly 1,000 randomly-selected images from each class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another.

## Requirements
To run the code, you need to have the following Python packages installed:

+ Keras
+ TensorFlow
+ NumPy
+ Matplotlib

## Implementation

### Data Preprocessing
The `Data` class is defined to load and preprocess the CIFAR-10 dataset. The `__init__` method loads the dataset and divides it into training and test sets. The `normalize` method normalizes the pixel values to be between 0 and 1. The flatten method `flattens` the images and converts them to floating-point format. The one_hot method converts the class labels to `one-hot` encoding.

### Visualization
The `Show_Image` class is defined to visualize the first 10 images from the dataset along with their corresponding labels.

### Multilayer Perceptron
The `MLP` class is defined to create and train a multilayer perceptron model on the CIFAR-10 dataset. The `add_layer` method adds layers to the model with or without activation functions. The `Compile` method compiles the model with specified loss function and optimizer. The `Fit` method trains the model on the training set. The `Evaluate` method evaluates the model on the test set. The `Predict` method makes predictions on new data.

### Convolutional Neural Network with Multilayer Perceptron
The `CNN_MLP` class is defined to create and train a convolutional neural network with multilayer perceptron model on the CIFAR-10 dataset. The `add_mlp` method adds a multilayer perceptron layer to the model with or without dropout and batch normalization. The `add_cnn` method adds a convolutional layer to the model. The `add_pooling_batch` method adds a convolutional layer with max pooling and batch normalization to the model. The `add_dropout` method adds a convolutional layer with dropout to the model.

## Conclusion
This implementation of image classification on CIFAR-10 dataset using deep learning demonstrates the use of Keras library with TensorFlow as the backend. The implementation includes data preprocessing, visualization, and training of multilayer perceptron and convolutional neural network with multilayer perceptron models.
