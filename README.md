# Optimizing Custom Convolutional Blocks for Pre-trained CNNs in Tuberculosis X-ray Analysis

[cite_start]This repository provides the code, notebooks, and dataset links for the paper: **"Optimizing Custom Convolutional Blocks for Pre-trained CNNs in Tuberculosis X-ray Analysis via Bayesian Optimization"**.

[cite_start]The research focuses on enhancing Tuberculosis (TB) detection from chest X-rays by appending custom convolutional blocks to pre-trained CNN architectures (ResNet50, InceptionV3, and DenseNet121). [cite_start]The hyperparameters of these custom blocks were tuned using Bayesian Optimization to maximize performance.

## Notebooks

These Kaggle notebooks contain the code used for the Bayesian Optimization process, as well as for training and evaluating the final models.

### Bayesian Optimization:
* **[ResNet50 Base - Bayesian Optimization (Optuna)](https://www.kaggle.com/code/nicholasnevank/bo-resnet50):** Performs hyperparameter search using Optuna to find the best custom layer configuration for the ResNet50 base.
* **[InceptionV3 Base - Bayesian Optimization (Optuna)](https://www.kaggle.com/code/nicholasnevank/bo-inceptionv3):** Performs hyperparameter search using Optuna to find the best custom layer configuration for the InceptionV3 base.
* **[DenseNet121 Base - Bayesian Optimization (Optuna)](https://www.kaggle.com/code/nicholasnevank/bo-densenet121):** Performs hyperparameter search using Optuna to find the best custom layer configuration for the DenseNet121 base.

### Model Training and Evaluation:
* **[ResNet50 Base - Training & Evaluation](https://www.kaggle.com/code/nicholasnevank/resnet50-cnn-tb-2):** Trains and evaluates the ResNet50-based model using the optimized hyperparameters for TB detection.
* **[InceptionV3 Base - Training & Evaluation](https://www.kaggle.com/code/nicholasnevank/inceptionv3-cnn-tb-2):** Trains and evaluates the InceptionV3-based model using the optimized hyperparameters for TB detection.
* **[DenseNet121 Base - Training & Evaluation](https://www.kaggle.com/code/nicholasnevank/densenet121-cnn-tb):** Trains and evaluates the DenseNet121-based model using the optimized hyperparameters for TB detection.

## Output Datasets

Datasets generated during the Bayesian Optimization process (hosted on Kaggle):

* **[Optuna Study Database Files](https://www.kaggle.com/datasets/nicholasnevank/optuna-study-db):** Contains the `optuna_study.db` files for the Optuna optimization trials for each base model.
* **[Best Hyperparameters (JSON)](https://www.kaggle.com/datasets/nicholasnevank/bo-best-hyperparameters):** JSON files storing the best hyperparameter configurations found by Bayesian Optimization for each base model.

## Input Dataset

The X-ray dataset used for training and evaluation (hosted on Kaggle):

* [cite_start]**[Tuberculosis (TB) Chest X-ray Dataset](https://www.kaggle.com/datasets/tawsifurrahman/tuberculosis-tb-chest-xray-dataset):** This public dataset contains normal and Tuberculosis positive chest X-ray images.

## Citation

If you use the code or findings from this research, please cite the original paper.
(Details of the paper to be added here once published)

[cite_start]The codebase for this study is also available at: [https://github.com/NicNev/optimizing-custom-convolutional-blocks-tb](https://github.com/NicNev/optimizing-custom-convolutional-blocks-tb)
