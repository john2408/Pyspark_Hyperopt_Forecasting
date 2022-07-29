# Docker Containerized Jupyter Notebook 

## Hyperparameter Optimization using parallel model training in Spark


[![docker pulls](https://img.shields.io/docker/pulls/jupyter/pyspark-notebook.svg)](https://hub.docker.com/r/jupyter/pyspark-notebook/)
[![docker stars](https://img.shields.io/docker/stars/jupyter/pyspark-notebook.svg)](https://hub.docker.com/r/jupyter/pyspark-notebook/)
[![image size](https://img.shields.io/docker/image-size/jupyter/pyspark-notebook/latest)](https://hub.docker.com/r/jupyter/pyspark-notebook/ "jupyter/pyspark-notebook image size")

GitHub Actions in the <https://github.com/jupyter/docker-stacks> project builds and pushes this image to Docker Hub.

This docker stack allows to train forecasting models using any Machine Learning (sklearn based) or Statistical Model with the help of **pypspark**. Moreover, hyperparameter optimization via the package **hyperopt** is also available. 

Model training and management is done via **mlflow**. 

In order to reproduce the results