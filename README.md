# Docker Containerized Jupyter Notebook 

## Hyperparameter Optimization using parallel model training in Spark


[![image size](https://img.shields.io/docker/image-size/johntorrestensor/pyspark-ml)](https://hub.docker.com/r/johntorrestensor/pyspark-ml/ "johntorrestensor/pyspark-ml image size")


This docker stack allows to train forecasting models using any Machine Learning (sklearn based) or Statistical Model with the help of **pypspark**. Moreover, hyperparameter optimization via the package **hyperopt** is also available. 

Currently **RandomForestRegression** and **XGBRegressor** can be used to train models using temporal cross validation and then make inferences based on the best model. 

Model training and management is done via **mlflow**. 

In order to reproduce the results initialize docker. If using WSL2:

```bat
sudo /etc/init.d/docker start
```

If using Linux based distributed System: 

```bat
sudo systemctl start docker
```
Then, create image from Docker file: 

```bat
sudo docker build -t pysparkforecast:latest .
```

Run interactive Jupyter Lab session from Docker Image: 


```bat
sudo docker run -it --rm -p 8888:8888 -v "${PWD}":/home/jovyan/work pysparkforecast:latest
```

<img src="img/Univariate_training_chart.png" alt="alt text" title="image Title" height="400"/>


