# Machine_Learning_Algorithmic_Trading

Machine Learning Algorithms that adapt to new data for enhanced trading signals


This Python application is a binary classifier and is developed to predict the success rate of venture fund's startup investments using Neural Network models. This program notebook is set up to run on Google Colab; due to Apple M1 incompatability; however, it can be customized to function on MS Windows.

In this program, objective is to build, train, evaluate, and optimize the Neural Network model. It compiles a neural network model; then tests other parameters to determine the values that generate the best Loss and Accuracy. It uses dataset manipulation and trial and error methods to develop best possible predictive model. Optimization techniques are utilized to enhance the data preprocessing and model design.

Total of four (4) iterations of trials and error are performed in pursuit to define best possible model.

Notebooks

`GC_venture_funding_with_deep_learning.ipynb`

`GC_alternatives_neural_networks.ipynb`

## Technologies

This application incorportates the following required  dependancies to run:

### Import the required libraries and dependencies for Python

`import tensorflow as tf`

`import pandas as pd`

`from tensorflow.keras.layers import Dense`

`from tensorflow.keras.models import Sequential`

`from sklearn.model_selection import train_test_split`

`from sklearn.preprocessing import StandardScaler, OneHotEncoder`


## Installation Guide

The following installation must be performed before running the program. It include:

### Install the required libraries 

For Window users:

`TensorFlow 2.0` and `Keras`

Use the pip install command to install the TensorFlow 2.0 library

`pip install --upgrade tensorflow`

Apple M1 Chip Users:
The Apple M1 Chip is not currently compatible with a typical Tensorflow installation, run this app on Google Colab


## Usage

To run this application, create a clone on the local desktop. Then, initiate your conda environment and launch in Jupyter Lab. For Apple Mac users, launch in Google Colab.

Resources folder contains the following CSV files:

`applicant_data.csv`


The following information evaluates the results of the orginal monels and 2 alternate models:


<img width="774" alt="accuracy scores" src="https://user-images.githubusercontent.com/93550651/161475831-925c1f7b-2994-4c45-b8e3-8dc677c8f2e6.png">


## Contributors

Contributor: John Batarse  

Email: jbatarse@hotmail.com

LinkedIn: [Find me on LinkedIn](<https://www.linkedin.com/in/john-a-batarse-760a26116/>)


## License

Trilogy Education LLC. and UC Berkeley