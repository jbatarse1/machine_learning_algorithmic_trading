# Machine_Learning_Algorithmic_Trading

Machine Learning Algorithms that adapt to new data for enhanced trading signals


This Python application is has 4 sections to the ML Algo Trading Bot. They are:

1. Establish Baseline Performance

2. Tune Baseline Trading Algorithm

3. Evaluate New Machine Learning classifier

4. Create Evaluation Report

In this program, objective is to 


Notebooks

`machine_learning_trading_bot.ipynb`

`tune1_machine_learning_trading_bot.ipynb`

## Technologies

This application incorportates the following required  dependancies to run:

### Import the required libraries and dependencies for Python

`import pandas as pd`

`import numpy as np`

`from pathlib import Path`

`import hvplot.pandas`

`import matplotlib.pyplot as plt`

`from sklearn import svm`

`from sklearn.preprocessing import StandardScaler`

`from pandas.tseries.offsets import DateOffset`

`from sklearn.metrics import classification_report`


## Installation Guide

The following installation must be performed before running the program. It include:

### Install the required libraries 

``Pandas``

``NumPy``

``hvPlot``

``Matplotlib``

``scikit-learn``



## Usage

To run this application, create a clone on the local desktop. Then, initiate your conda environment and launch in Jupyter Lab. 

Resources folder contains the following CSV files:

`emerging_markets_ohlcv.csv`


The following information evaluates the results of the           :




## Conclusion on the performance of the baseline trading algorithm

Looking at the Baseline Cumulative Returns Plot, the Strategy Returns performance is consistent with the actual returns upto the middle of 2018; at which point, the Strategy Returns are predicted to outperform the Actual Returns. The Strategy Returns predictions follow a similar trend with that of the Actual Returns.

![baseline_algo_trade](https://user-images.githubusercontent.com/93550651/162590072-dadf8186-209b-457e-94ac-2cc7521d2a75.png)

## Conclusion on the performance of Tuning the baseline trading algorithm

The set of parameters that best improved the trading algorithm returns...

4 time periods were tested to determine best model: 3, 6, 9, 12 months. 



## Conclusion on Backtesting the new model to evaluate its performance

The back test for the new model..;....

Did the new model perform better or worse than the provided baseline models....

Did this model perform better or worse than your tuned trading algorithm...


## Evaluation Report

Final conclusions and analysis.....

Findings are supported by the PNG images.




## Contributors

Contributor: John Batarse  

Email: jbatarse@hotmail.com

LinkedIn: [Find me on LinkedIn](<https://www.linkedin.com/in/john-a-batarse-760a26116/>)


## License

Trilogy Education LLC. and UC Berkeley
