# Optimizing Custom Convolutional Blocks for Pre-trained CNNs in Tuberculosis X-ray Analysis via Bayesian Optimization

Code, notebooks, and dataset links for the paper: **"Optimizing Custom Convolutional Blocks for Pre-trained CNNs in Tuberculosis X-ray Analysis via Bayesian Optimization"**.

This repository provides resources to reproduce the results presented in the paper. Bayesian Optimization was used to find optimal hyperparameter configurations for custom convolutional blocks appended to fine-tuned ResNet50, Inception V3, and DenseNet121 base models for Tuberculosis X-ray classification.

## Notebooks

These notebooks contain the code used for Bayesian Optimization and subsequent model training/evaluation. They are designed to run on Kaggle.

* **Bayesian Optimization (Optuna) - ResNet50:** [Kaggle Notebook](https://www.kaggle.com/code/nicholasnevank/bo-resnet50)
    * Performs hyperparameter search using Optuna to find the best custom layer configuration for the ResNet50 base model.
* **Bayesian Optimization (Optuna) - InceptionV3:** [Kaggle Notebook](https://www.kaggle.com/code/nicholasnevank/bo-inceptionv3)
    * Performs hyperparameter search using Optuna to find the best custom layer configuration for the InceptionV3 base model.
* **Bayesian Optimization (Optuna) - DenseNet121:** [Kaggle Notebook](https://www.kaggle.com/code/nicholasnevank/bo-densenet121)
    * Performs hyperparameter search using Optuna to find the best custom layer configuration for the DenseNet121 base model.
    * These optimization notebooks generate the `optuna-study-db` and `bo-best-hyperparameters` datasets (see below).

* **ResNet50 Base Training:** [Kaggle Notebook](https://www.kaggle.com/code/nicholasnevank/resnet50-cnn-tb-2)
    * Trains and evaluates the ResNet50-based model using the optimized hyperparameters for Tuberculosis X-ray classification.
* **InceptionV3 Base Training:** [Kaggle Notebook](https://www.kaggle.com/code/nicholasnevank/inceptionv3-cnn-tb-2)
    * Trains and evaluates the InceptionV3-based model using the optimized hyperparameters for Tuberculosis X-ray classification.
* **DenseNet121 Base Training:** [Kaggle Notebook](https://www.kaggle.com/code/nicholasnevank/densenet121-cnn-tb)
    * Trains and evaluates the DenseNet121-based model using the optimized hyperparameters for Tuberculosis X-ray classification.

## Output Datasets

Datasets generated during the Bayesian Optimization process:

* **[Optuna Study DB](https://www.kaggle.com/datasets/nicholasnevank/optuna-study-db):** Contains the `optuna_study.db` files storing the progress of Optuna optimization trials for each base model.
* **[Best Hyperparameters (JSON)](https://www.kaggle.com/datasets/nicholasnevank/bo-best-hyperparameters):** Contains JSON files storing the best hyperparameter configurations found by Bayesian Optimization for each base model.

## Input Dataset

The original X-ray dataset used for training and evaluation (hosted on Kaggle):

* **[Tuberculosis (TB) Chest X-ray Dataset](https://www.kaggle.com/datasets/tawsifurrahman/tuberculosis-tb-chest-xray-dataset)**
