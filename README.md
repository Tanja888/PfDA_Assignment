#### Programming for Data Analysis Project 1

#### About the Project
The purpose of this project is to gain knowledge in creating a **synthesised data set** by simulating a real-world phenomenon using numpy.random package in **Python** and implementing it in a Jupyter notebook. The minimum requirement for the dataset is one-hundred data points over four variables. 

#### Technologies
Python 3.9.13

#### Starting Jupyter Notebook
Jupyter Notebook can be started through command line by running jupyter notebook in Terminal for Linux and Mac or Command Prompt for Windows.[[1]](https://docs.jupyter.org/en/latest/running.html#starting-the-notebook-server) 
The notebook will automatically open in the browser, it is possible to navigate it through the dashboard that contains files, notebook with .ipynb extension, Readme file and all the other files uploaded for the project.

#### Data
Data used for the project were retreived from Kaggle platform about Quality of Life in cities across the world based on different variables. [[2]](https://www.kaggle.com/datasets/orhankaramancode/city-quality-of-life-dataset). After data exploration and data cleaning 229 datapoints were used over 7 variables.

#### Setup
##### Reading data through csv 
```python
    scores = pd.read_csv('scoresData.csv')
```

#### Libraries

```python
    import pandas as pd
    import numpy as np
    import matplotlib.pyplot as plt
    import random
    import seaborn as sns
    import sys
```

#### Data Exploration and Data Cleaning
To obtain information on data types we used info() function, columns were renamed for easier reading, unwanted variables were dropped and index slicing was used in order to remove rows with zero values. 

#### Statistics and visualization 
To get the insight into the variables we did their summary statistics and correlation between them was examined. Variables were grouped based on categorical Continent variable and visualization was done using strip plots. Histograms showed distributions of variables and scatter plots were used for the correlation.

#### Generating new data
To generate new data NumPy library and **numpy.random.default_rng** function were used, data set was sliced into two parts to be able to compare them. The reference point for generating data was correlation between the variables while values themselves were generated according to the quartiles ranges of the independent variables.   