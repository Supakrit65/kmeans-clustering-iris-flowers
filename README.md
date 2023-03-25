# Iris Species Clustering Project

This project aims to cluster Iris flowers into species groups based on their petal and sepal dimensions. We use the famous Iris dataset and apply the k-means clustering algorithm to group the flowers into clusters. We also compare the clustering results with the actual species labels to evaluate the performance of our clustering model.

## Dataset

The dataset used in this project is the Iris dataset, which consists of 150 samples of Iris flowers, each belonging to one of three species: Iris setosa, Iris versicolor, or Iris virginica. Each sample has four features: sepal length, sepal width, petal length, and petal width (all in centimeters).

- `dataset/Iris.csv`: The Iris dataset file in CSV format.

## Files

- `clustering.ipynb`: A Jupyter Notebook that contains the code for data preprocessing, clustering, and visualizations.

## Project Overview

1. **Data Preprocessing:** We start by loading the dataset and renaming the columns to more convenient names. Then, we standardize the petal length and petal width features using StandardScaler from the scikit-learn library.

2. **Optimal Number of Clusters:** We use the elbow method to determine the optimal number of clusters or the k-means algorithm. We plot the inertia (sum of squared distances of samples to their closest cluster center) for different numbers of clusters and visually identify the "elbow" point in the plot. This point represents the optimal number of clusters that balances the trade-off between minimizing the inertia and avoiding overfitting.

3. **K-means Clustering:** We fit the k-means clustering model with the optimal number of clusters found in the previous step. We use the standardized petal length and petal width features to train the model.

4. **Performance Evaluation:** We evaluate the performance of our clustering model by comparing it with the actual species labels. We use the adjusted Rand index to measure the similarity between the true and predicted clusterings. A higher adjusted Rand index indicates better clustering performance.

5. **Visualizations:** We create various visualizations to compare the k-means clustering results with the actual species clustering, including side-by-side scatterplots of the actual species clustering and k-means clustering, and a confusion matrix to show the relationship between cluster labels and true species labels.

## Usage

To run the project, open the clustering.ipynb Jupyter Notebook and execute the cells in order. Make sure you have the required Python packages installed:

- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn
