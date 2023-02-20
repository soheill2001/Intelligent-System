# Wine Classification with KNN and Metric Learning Algorithms

This code provides a simple implementation of the k-Nearest Neighbors (KNN) algorithm and compares the accuracy of the model with different values of k. It also demonstrates the use of dimensionality reduction techniques, namely Principal Component Analysis (PCA), Local Fisher Discriminant Analysis (LFDA), and Large Margin Nearest Neighbor (LMNN), to transform the dataset and visualize the results. Finally, it plots a heatmap to show the correlation between the features of the wine dataset.The goal of this project is to classify the wines into three different types (classes) based on their chemical compositions.

## Requirements
To run this code, you need the following packages:

+ numpy
+ pandas
+ scikit-learn
+ metric-learn
+ seaborn
+ matplotlib

## Dataset
The wine dataset is used in this implementation, which is included in the sklearn.datasets module. This dataset contains 13 features that describe the chemical composition of different wines, and the target variable is the class of each wine, which can be 0, 1, or 2.

## Implementation
The `Data` function is used to load the wine dataset and split it into training and testing sets. The KNN algorithm is implemented using the `euclidean_distance` and `KNN` functions, which calculate the Euclidean distance between two points and return the k-nearest neighbors, respectively. The `predict` function is used to predict the target variable for a given set of test data. The accuracy and confusion matrix of the model are printed for different values of k using a loop.

PCA is used to reduce the dimensionality of the dataset, and the `PCA_` function is used to transform the data into a two-dimensional array that can be visualized. The `LFDA_` and `LMNN_` functions are used to transform the dataset using LFDA and LMNN, respectively, and the transformed datasets are plotted using the `Plot` function.

Finally, a heatmap is plotted to show the correlation between the features of the wine dataset using the `seaborn` and `matplotlib` libraries.

## Conclusion
In conclusion, this code provides a simple implementation of the KNN algorithm and demonstrates the use of dimensionality reduction techniques to visualize the results. The accuracy of the model is compared for different values of k, and the correlation between the features of the wine dataset is visualized using a heatmap.