# Logistic Regression for MNIST Digit Recognition

This code implements a logistic regression classifier using gradient descent and stochastic gradient descent optimization techniques for classifying images of handwritten digits from the MNIST dataset. The code performs preprocessing of the data to keep only the images of the digits '2' and '7'. The performance of the classifier is evaluated on both the training and test datasets.

## Functions
+ `Pre_Processing`: This function takes the training and test datasets and removes all images other than those corresponding to digits 2 and 7. The images are then normalized and the labels are converted to either 1 or -1 depending on whether the digit is a 7 or 2 respectively.
+ `accuracy`: This function calculates the accuracy of the classifier.
+ `miu`: This function calculates the sigmoid of the dot product of the image and the weights of the classifier.
+ `J_b`: This function calculates the partial derivative of the cost function with respect to the bias.
+ `J_w`: This function calculates the partial derivative of the cost function with respect to the weights.
+ `J`: This function calculates the cost function.
forward: This function performs gradient descent optimization on the data to obtain the weights and bias of the classifier.
+ `SGD`: This function performs stochastic gradient descent optimization on the data to obtain the weights and bias of the classifier.

## Conclusion
This code demonstrates the implementation of logistic regression using gradient descent and stochastic gradient descent for binary classification of handwritten digits from the MNIST dataset. The results show that both gradient descent and stochastic gradient descent are effective in updating the weights and bias to achieve high classification accuracy.