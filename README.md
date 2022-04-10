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

The baseline model Precision for the -1 class is 0.43 and for the 1 class is 0.55. This does not provide much confidence in the models performance. The Recall for -1 class is 0.04 and for 1 class is 0.96. Seems heavily weighted towards predicting 1 class over -1 class.

<img width="476" alt="svm_test_report" src="https://user-images.githubusercontent.com/93550651/162644434-6e4bfe81-f6fd-498e-83a7-5b8402d6195d.png">

Looking at the Baseline Cumulative Returns Plot, the Strategy Returns performance is consistent with the actual returns upto the middle of 2018; at which point, the Strategy Returns are predicted to outperform the Actual Returns. The Strategy Returns predictions follow a similar trend with that of the Actual Returns.

![baseline_algo_trade](https://user-images.githubusercontent.com/93550651/162590072-dadf8186-209b-457e-94ac-2cc7521d2a75.png)

<img width="432" alt="Actual_versus_Strategy" src="https://user-images.githubusercontent.com/93550651/162645314-d179fed6-7436-4980-b03e-49a9d89c51cb.png">

The new model Precision for the -1 class is 0.44 and for the 1 class is 0.56. These results are almost the same as in the baseline model's performance. The Recall for -1 class is 0.33 and for 1 class is 0.66. Seems heavily weighted towards predicting 1 class over -1 class.

<img width="476" alt="new_model_test_report" src="https://user-images.githubusercontent.com/93550651/162644415-a6e9a439-998f-4c0f-88ef-39bd33a18469.png">

In conclusion, the new model performed better than the baseline.


## Conclusion on the performance of Tuning the baseline trading algorithm

To determine the best trading outcomes, several iterations were performed by changing the model input features. 

First,  the `DateOffset` values was adjusted by changing the months from 3 months to 6 months.

<img width="635" alt="DateOffset_6_mos" src="https://user-images.githubusercontent.com/93550651/162644709-1175b159-45b2-4b28-bcd2-8ae24d24bdd7.png">

<img width="463" alt="6mos_date_report" src="https://user-images.githubusercontent.com/93550651/162644904-522d632f-8806-4af4-8896-13cee363cd3a.png">

<img width="458" alt="6mos_date_plot" src="https://user-images.githubusercontent.com/93550651/162644950-0a7f65b6-52a8-47d5-8b8b-fd5f75d67f0e.png">

<img width="452" alt="6mos_newmodel_report" src="https://user-images.githubusercontent.com/93550651/162645139-f9402d78-26f3-4d24-bacf-2149e7e87a55.png">

<img width="432" alt="6mos_newmodel_plot" src="https://user-images.githubusercontent.com/93550651/162645145-9aff71cd-7463-4db9-a51c-3e59f178e491.png">

from short_window = 4 to 7; for the long_window = 100 to 90.



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
