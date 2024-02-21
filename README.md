### Pipline Flow
![Pipline-Diagram](/model/wdb.png)

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
    - download     

    - preprocess      

    - check_data       

    - segregate      

    - random_forest      

    - evaluate      

- project files 
    - main.py ----> main script for the pipeline that runs each step 
    - conda.yml -----> creates conda environment for mlflow pipeline execution
    - config.txt -----> Configuration file for the project and default model parameters 
    - MLproject -------> Mlflow project configuration 

## Running Files
* First create conda environment using :
```
conda create --name serve python=3.8 mlflow=1.14.1 wandb=0.10.28 numpy=1.18.1 pandas=1.2.3 -c conda-forge
```
* Login to Wandb using:
```
wandb login
```

* Run the project using:
```
 mlflow run https://github.com/sidahmed-faisal/Genre-Classification-pipline-with-MLflow.git \ 
             -v 1.0.0 \
             -P hydra_options="main.project_name=remote_execution"
``` 

* Or Clone the project and run it using:
```
mlflow run . -P hydra_options="main.project_name=your_project_name"
```

* Deploy the project as gunicorn server:
```
mlflow models serve -m model &
```
* Or as a Docker Container
```
mlflow models build-docker -m model -n "genre_classification"
```





