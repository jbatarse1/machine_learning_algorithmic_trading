# Machine_Learning_Algorithmic_Trading

In this program, the objective is to develop a Machine Learning Algorithms that adapts to new data for enhanced trading signals.

This Python ML Algo Trading Bot application is set up in 4 sections. They are:

1. Establish Baseline Performance

2. Tune Baseline Trading Algorithm

3. Evaluate New Machine Learning classifier

4. Create Evaluation Report

The following Notebooks are used:

`machine_learning_trading_bot.ipynb`

`tune1_machine_learning_trading_bot.ipynb`

Resources folder contains the following CSV files:

`emerging_markets_ohlcv.csv`

## Technologies

This application incorportates the following required dependancies to run:

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

### Conclusion on the performance of the baseline trading algorithm

The baseline model Precision for the -1 class is 0.43 and for the 1 class is 0.55. This does not provide much confidence in the models performance. The Recall for -1 class is 0.04 and for 1 class is 0.96. This is heavily weighted towards predicting 1 class over -1 class.

<img width="429" alt="svm_report_original" src="https://user-images.githubusercontent.com/93550651/162646011-50042ec5-a42c-4ca1-9058-2aa233729b27.png">

The new model Precision for the -1 class is 0.44 and for the 1 class is 0.56. These results are a little bit better than that of the the baseline model's performance. The Recall for -1 class is 0.33 and for 1 class is 0.66. This is still heavily weighted towards predicting 1 class over -1 class but better results.

<img width="429" alt="new_model_rpt" src="https://user-images.githubusercontent.com/93550651/162646105-c43ede3b-d82a-492e-8fe9-8e7b2dfcc14a.png">

Looking at the Baseline and New Model Cumulative Returns Plots, the Strategy Returns performance is consistent with the actual returns upto the middle of 2018; at which point, the Strategy Returns are shown to outperform the Actual Returns. The Strategy Returns follow a similar trend with that of the Actual Returns on both plots.

![baseline_algo_trade](https://user-images.githubusercontent.com/93550651/162590072-dadf8186-209b-457e-94ac-2cc7521d2a75.png)

<img width="432" alt="Actual_versus_Strategy" src="https://user-images.githubusercontent.com/93550651/162645314-d179fed6-7436-4980-b03e-49a9d89c51cb.png">

In conclusion, the new model performed better than the baseline model.

### Conclusion on the performance of Tuning the baseline trading algorithm

To determine the best trading outcomes, several iterations were performed by changing the model input features. 

First, the `DateOffset` value was adjusted by changing the months from 3 months to 6 months.

<img width="635" alt="DateOffset_6_mos" src="https://user-images.githubusercontent.com/93550651/162644709-1175b159-45b2-4b28-bcd2-8ae24d24bdd7.png">

<img width="463" alt="6mos_date_report" src="https://user-images.githubusercontent.com/93550651/162644904-522d632f-8806-4af4-8896-13cee363cd3a.png">

<img width="458" alt="6mos_date_plot" src="https://user-images.githubusercontent.com/93550651/162644950-0a7f65b6-52a8-47d5-8b8b-fd5f75d67f0e.png">

<img width="452" alt="6mos_newmodel_report" src="https://user-images.githubusercontent.com/93550651/162645139-f9402d78-26f3-4d24-bacf-2149e7e87a55.png">

<img width="432" alt="6mos_newmodel_plot" src="https://user-images.githubusercontent.com/93550651/162645145-9aff71cd-7463-4db9-a51c-3e59f178e491.png">

By slicing the data from 3 months to 6 months, it also changes the size of the training dataset. As a result, the model did not improve.

Second, keeping the DateOffset at 3 months, let's adjust the short_window = 4 to 3; for the long_window = 100 to 75.

<img width="312" alt="tune_sma" src="https://user-images.githubusercontent.com/93550651/162647189-99186c4d-89c5-442f-9685-011414db6c06.png">

<img width="454" alt="adj_svm" src="https://user-images.githubusercontent.com/93550651/162647260-85577556-78f3-4695-9208-384725b1e72d.png">

<img width="429" alt="adj_plot" src="https://user-images.githubusercontent.com/93550651/162647322-a454025a-ecef-4a9c-b636-9baaa25bb20f.png">

<img width="467" alt="adj_rpt" src="https://user-images.githubusercontent.com/93550651/162647441-694ca93e-a8da-42ec-aa3b-ebb0fe905f42.png">

<img width="415" alt="adj_new_plot" src="https://user-images.githubusercontent.com/93550651/162647461-b4099c3c-f810-4b5c-abe2-ccb4feffb747.png">

Having performed several iterations to identify the best trading algorithm returns, it is concluded that the orginial parameters outperform the adjusted models.

### Conclusion on Backtesting the new model to evaluate its performance

Setting the data to the orginial parameters, the `AdaBoost` and `DecisionTree` classifiers have been iterated in pursuit of a better model. Here are the results:

AdaBoost Classifier

<img width="406" alt="Ada_Boost" src="https://user-images.githubusercontent.com/93550651/162648860-ea2aa9ca-aa01-478b-9f61-ad52a8bdd11a.png">

<img width="562" alt="Ada_Boost1" src="https://user-images.githubusercontent.com/93550651/162648865-e804da4b-ba3f-40dd-a25a-60f7fb1ec2a1.png">

<img width="455" alt="Ada_Boost2" src="https://user-images.githubusercontent.com/93550651/162648874-596ba636-7605-4ee7-9333-b42e497655e4.png">

<img width="411" alt="Ada_Boost3" src="https://user-images.githubusercontent.com/93550651/162648886-255866b6-c625-416f-92ae-5afda64cfef3.png">

The AdaBoost Classifier model perform slighly better than the provided baseline model.

DecisionTree Classifier

<img width="458" alt="DTC" src="https://user-images.githubusercontent.com/93550651/162649656-c576a104-95d7-4663-a963-bb0468da6cc1.png">

<img width="586" alt="DTC1" src="https://user-images.githubusercontent.com/93550651/162649662-ec955eaa-7880-46cb-ba24-61890be2fcb6.png">

<img width="435" alt="DTC2" src="https://user-images.githubusercontent.com/93550651/162649671-f57b52c9-985e-4226-a2b8-16cf6fe9c3ca.png">

<img width="424" alt="DTC3" src="https://user-images.githubusercontent.com/93550651/162649679-f700b0d8-bc2d-4a79-a793-5e533743bc8a.png">

The DecisionTree Classifier model performed differently than the original and tuned models. The precision are the same: 0.44 for -1 and .53 for 1. However, the recall has flipped to heavier weight of 0.84 for -1

The Returns Plots run consistant with the other models.

## Summary Evaluation Report

In sum, the best model is the original LogisticRegression "new_model" with the DateOffset at 3 months and the short window / long window set to 4 day and 100 days, respectively. The precision is about the same; but the recall of 0.33 for -1 class and 0.66 for the 1 class shows better performance in comparison to the other models.

## Contributors

Contributor: John Batarse  

Email: jbatarse@hotmail.com

LinkedIn: [Find me on LinkedIn](<https://www.linkedin.com/in/john-a-batarse-760a26116/>)


## License

Trilogy Education LLC. and UC Berkeley
