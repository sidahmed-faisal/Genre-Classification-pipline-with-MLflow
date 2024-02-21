# Genre Classification Pipeline using MLFlow and Weights and Biases 

- Project **Genre Classification Model** using MLflow and Weights and Biases to manage the preprocessing of the dataset and feature engineering and storing the model to inference artifact

## Project Description
- This project implements a Machine Learning project pipline using MLflow and Weights and Biases to manage the preprocessing of the dataset and feature engineering and storing the model to inference artifact and offers flexibility for interactive or command-line execution summeraized in the following:

* Machine learning model development and training for Genre Classification.

* Experiment Tracking using Weights and biases and MLflow.

* Model Exporting to inference artifact.

* Deploying model to Production using MLflow as Docker container or RestApi.

## Files and data description
The project is organized with the following directory architecture:
- Folders
    - Download     
        - eda       --> contains output of the data exploration
        - results   --> contains the dataset in csv format
    - preprocess      
        - eda       --> contains output of the data exploration
        - results   --> contains the dataset in csv format
    - check_data       
        - eda       --> contains output of the data exploration
        - results   --> contains the dataset in csv format
    - segregate      
        - eda       --> contains output of the data exploration
        - results   --> contains the dataset in csv format
    - random_forest      
        - eda       --> contains output of the data exploration
        - results   --> contains the dataset in csv format
    - evaluate      
        - eda       --> contains output of the data exploration
        - results   --> contains the dataset in csv format
    - images        --> contains model scores, confusion matrix, ROC curve
    - models        --> contains saved models in .pkl format
    - logs          --> log generated druing testing of library.py file

- project files 
    - main.py
    - conda.yml
    - config.txt
    - MLproject

## Running Files
* First create conda environment using :
* ``
* conda create --name serve python=3.8 mlflow=1.14.1 wandb=0.10.28 numpy=1.18.1 pandas=1.2.3 -c conda-forge
* ``

* Second Run the Machine learning pipline using:





