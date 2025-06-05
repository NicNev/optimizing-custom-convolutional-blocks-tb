# Optimizing Custom Convolutional Blocks for Pre-trained CNNs in Tuberculosis X-ray Analysis via Bayesian Optimization

Code, notebooks, and dataset links for the paper: **"Optimizing Custom Convolutional Blocks for Pre-trained CNNs in Tuberculosis X-ray Analysis via Bayesian Optimization"**.

[cite_start]This repository provides resources to reproduce the results presented in the paper.  [cite_start]Bayesian Optimization was used to find optimal custom convolutional blocks appended to fine-tuned ResNet50, Inception V3, and DenseNet121 models (pre-trained on RadImageNet) for Tuberculosis X-ray classification. 

## Notebooks

These notebooks contain the code used for optimization and model training/evaluation. They are designed to run on Kaggle.

* **Bayesian Optimization (Optuna):** Performs the hyperparameter search using Optuna to find the best custom layer configurations.
    * [ResNet50 Base](https://www.kaggle.com/code/nicholasnevank/bo-resnet50)
    * [InceptionV3 Base](https://www.kaggle.com/code/nicholasnevank/bo-inceptionv3)
    * [DenseNet121 Base](https://www.kaggle.com/code/nicholasnevank/bo-densenet121)
* **Model Training:** Trains and evaluates the models using the optimized hyperparameters for each respective base architecture.
    * [ResNet50 Base Training](https://www.kaggle.com/code/nicholasnevank/resnet50-cnn-tb-2)
    * [InceptionV3 Base Training](https://www.kaggle.com/code/nicholasnevank/inceptionv3-cnn-tb-2)
    * [DenseNet121 Base Training](https://www.kaggle.com/code/nicholasnevank/densenet121-cnn-tb)

## Output Datasets

Datasets generated during the Bayesian Optimization process:

* **[Optuna Study DB](https://www.kaggle.com/datasets/nicholasnevank/optuna-study-db):** Contains the `optuna_study.db` files for Optuna optimization trials for each base model.
* **[Best Hyperparameters (JSON)](https://www.kaggle.com/datasets/nicholasnevank/bo-best-hyperparameters):** JSON files storing the best hyperparameter configurations found by the optimization for each base model.

## Input Datasets

The original X-ray dataset used for training and evaluation (hosted on Kaggle):

* [cite_start]**[Tuberculosis (TB) Chest X-ray Dataset](https://www.kaggle.com/datasets/tawsifurrahman/tuberculosis-tb-chest-xray-dataset)**
