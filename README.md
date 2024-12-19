# JSONDrivenML
# Machine Learning Pipeline with Dynamic Configuration

This repository contains a Python script that dynamically builds machine learning pipelines based on a configuration file (in JSON format). The pipeline includes feature handling (encoding, scaling), feature reduction (correlation-based, tree-based, or PCA), and model training with hyperparameter tuning using GridSearchCV. The pipeline can adapt based on the selected configuration, enabling flexibility for different machine learning tasks such as regression or classification.

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Getting Started](#getting-started)
4. [Configuration Format](#configuration-format)
5. [Example Use Case](#example-use-case)
6. [Technologies Used](#technologies-used)
7. [License](#license)

## Overview

The goal of this project is to provide a flexible and configurable machine learning pipeline that can easily be customized to different datasets and machine learning tasks. The pipeline reads a JSON configuration file that specifies the following:

- Target variable and prediction type (regression or classification).
- Preprocessing steps for numerical and categorical features.
- Feature reduction methods (e.g., correlation, tree-based selection, or PCA).
- Algorithms to be used (e.g., Linear Regression, Random Forest, SVR, etc.).
- Hyperparameters for each algorithm.

By updating the JSON configuration file, users can change the model, feature reduction method, or feature handling steps, and rerun the script without changing the code.

## Features

- **Feature Handling**: Handles numerical and categorical features with scaling and encoding.
- **Feature Reduction**: Options for correlation-based feature selection, tree-based feature importance, and PCA.
- **Model Selection**: Supports multiple regression and classification algorithms with GridSearchCV for hyperparameter tuning.
- **Dynamic Configuration**: The pipeline is configured using a JSON file, making it easy to adjust without modifying the code.

## Getting Started

### Prerequisites

- Python 3.x
- Required libraries (see `requirements.txt`)

