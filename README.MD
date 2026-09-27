# Iris Dataset Analysis

A Jupyter notebook exploring the classic Iris dataset using supervised classification, unsupervised clustering, and dimensionality reduction.

## Overview

This project walks through a complete mini machine learning workflow on the Iris flower dataset:

1. **Exploratory Data Analysis** — inspecting the data, checking for missing values, and reviewing descriptive statistics and distributions (e.g. sepal length histogram).
2. **Preprocessing** — standardizing features with `StandardScaler` and splitting the data into training and test sets.
3. **Classification** — training a **Logistic Regression** model to predict Iris species, evaluated with accuracy, a classification report, and a confusion matrix.
4. **Clustering** — applying **K-Means** clustering, using the Elbow Method to select the optimal number of clusters, and visualizing the resulting clusters against petal length/width.
5. **Dimensionality Reduction** — using **PCA** to reduce the four features to two principal components and visualizing the class separation in 2D.

## Dataset

The [Iris dataset](https://scikit-learn.org/stable/datasets/toy_dataset.html#iris-plants-dataset) is loaded directly from `sklearn.datasets`, so no external data file is required. It contains 150 samples of iris flowers with four features (sepal length, sepal width, petal length, petal width) across three species.

## Requirements

- Python 3.x
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

Install dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage

1. Clone this repository.
2. Launch Jupyter:
   ```bash
   jupyter notebook ML.ipynb
   ```
3. Run all cells in order.

## Results

- The Logistic Regression model achieves high accuracy in classifying the three Iris species.
- The Elbow Method indicates that **3 clusters** is the appropriate choice for K-Means, which aligns naturally with the three known species.
- PCA shows that most of the dataset's variance can be captured in two principal components, allowing clear visual separation between species in 2D.

## License

Feel free to use and adapt this project for learning purposes.