# Mnist_digit_classifier

## Project Overview

This project implements an MNIST digit classification using only classical algorithms:

- **Dataset**: MNIST CSV format (flattened 28×28 → 784 pixels per image)
- **Models**: KNN, SVM (RBF/Linear), Decision Tree + Voting Ensemble
- **Key Features**: Hyperparameter tuning, PCA dimensionality reduction, Ensemble Methods Integration
- **Performance**: Individual models ~95%-96%, Ensemble ~96% test accuracy

## Quick Start

### Prerequisites
```bash
Python 3.8+
NumPy, Pandas, scikit-learn, Matplotlib, Seaborn
```

### To clone the dataset
git clone https://github.com/HPunya/Mnist_digit_classifier

### Dataset
Unarchive the mnist_train folder and update the path accordingly as the mnist_train.csv file was too large to update on this repo.

Give the path to both the csv by making the following changes:
In this code, update change the path to the dataset e.g. /Dataset/mnist_test.csv
train_path = "/content/mnist_test.csv"
test_path  = "/content/mnist_train.csv"

## Key implementations:
- **Task 1: Data Loading & Exploration:** Handles missing values in CSV, and malformed CSV and class distribution analysis is given
- **Task 2: Preprocessing Pipeline:** Normalizes the pixels, splits the train and test data, visulaizes sample images and applies PCA with 50 components
- **Task 3: Classical ML Models (Hyperparameter Tuning):** Trains the models on 3 different algorithms KNN, SVM and Decision tree using different parameters to find the best parameter
- **Task 4: Comprehensive Evaluation:** Evaluated the models on their accuracy and confusion matrix. Also  a bonus of combining ensemble methods is applied to check if those help. and SVM and KNN are trained using the PCA to see how does that affect the model performance.
