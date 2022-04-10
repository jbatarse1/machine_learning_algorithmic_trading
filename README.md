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

To Tune the Baseline Trading Algorithm, use:


`from sklearn.tree import DecisionTreeClassifier`

`from sklearn.ensemble import AdaBoostClassifier`


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

The baseline model Precision for the -1 class is 0.43 and for the 1 class is 0.55. This does not provide much confidence in the models performance. The Recall for -1 class is 0.04 and for 1 class is 0.96. Seems heavily weighted towards predicting 1 class over -1 class.

The new model Precision for the -1 class is 0.44 and for the 1 class is 0.56. These results are almost the same as in the baseline model's performance. The Recall for -1 class is 0.33 and for 1 class is 0.66. Seems heavily weighted towards predicting 1 class over -1 class.

In conclusion, the new model performed better than the baseline.

![baseline_algo_trade](https://user-images.githubusercontent.com/93550651/162590072-dadf8186-209b-457e-94ac-2cc7521d2a75.png)

## Conclusion on the performance of Tuning the baseline trading algorithm

To determine the best trading outcomes, several iterations were performed by changing the model input features. 

First,  the `DateOffset` values were adjusted; the size of the training dataset by changing from short_window = 4 to 7; for the long_window = 100 to 90.
 
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
