# Decision Tree Classifier for Titanic Dataset

This repository contains a Python implementation of a decision tree classifier to predict survival of passengers on the Titanic using the Titanic dataset. The decision tree is built using the ID3 algorithm. The implementation includes functions for preprocessing the data, calculating entropy and information gain, building the decision tree, and making predictions.

## Requirements
This implementation requires the following Python libraries:

+ pandas
+ scikit-learn
+ numpy
+ pprint

## Dataset
The Titanic dataset contains information about passengers on the Titanic, including their age, sex, passenger class, and whether or not they survived. The dataset is split into a training set and a test set.

## Implementation
The decision_tree.py file contains the following functions:

+ `preprocess`: preprocesses the dataset by dropping irrelevant columns, filling missing values, and one-hot encoding categorical features.
+ `Read_Data`: reads in the dataset from a CSV file.
+ `Entropy`: calculates the entropy of a given set of data.
+ `InfoGain`: calculates the information gain of a given split on a given attribute.
+ `ID3`: implements the ID3 algorithm to build the decision tree.
+ `predict`: recursively traverses the decision tree to predict the class of a given data point.
+ `test_`: tests the accuracy of the decision tree on a given test set.

## Results
The program will build a decision tree using the training data and display the tree, along with the accuracy of the model on the test data for different depths.
