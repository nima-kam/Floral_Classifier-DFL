# Floral Classifier using Discriminative Feature Learning 

The goal of this project is to train a ResNet-18 model to understand the differences and similarities of different types of flowers and generate a disentangled feature to classify pairs of flowers as a similar type or not. The project includes functions for data loading, transformation, training, validation, and optimization, as well as the definition of the ResNet-18 model, Center Loss module, and optimization parameters.

## Dataset
link to dataset documents: https://www.robots.ox.ac.uk/~vgg/data/flowers/102/index.html
The dataset consists of multiple image files, categorized into 102 different classes of flowers.

## Feature Extractor
A pre-trained ResNet-18 model is used as the feature extractor to extract high-level features from the images.

## Classification Layer
The original fully connected layer of the ResNet-18 model is replaced with a new linear layer that outputs the number of .
## Disentangled Feature Learning
The Center Loss technique is used to generate a disentangled feature representation of the flowers that captures the differences and similarities between them.

## Pairwise Classification
The disentangled feature representation is used to classify pairs of flowers as similar type or not.

## Center Loss
link to complete implementation of center loss: https://github.com/KaiyangZhou/pytorch-center-loss
The **Center Loss** technique is used to improve the performance of the model. This involves calculating the distance between the features and the class centers and computing the loss based on the distance and the ground truth labels.

## Code Overview
Class Distribution Visualization
This section of code visualizes the distribution of the dataset across different classes, loads the paths of all images, and creates a pandas dataframe containing the image paths and corresponding labels.

