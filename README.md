# Energy Demand Forecaster with Machine Learning

This repository stores a Jupyter Notebook for energy demand forecasting using different machine learning algorithms, as part of a project for the [Institute for Integrated Energy Systems (IESVic)](https://www.uvic.ca/research/centres/iesvic/index.php) in fulfillement of the Technical Writing (ENGR 446) academic course at the [University of Victoria](https://www.uvic.ca/)

## Objective
This is a neural network application with the main task of predicting future energy demands (particularly space heat demand) profiles for the province of British Columbia, based on available data from the past

## Sample Results

Some sample graphs from each model:

[1] Linear Regression model:

![](https://github.com/criscfer/Demand_Learner/blob/main/Sample%20Result%20Images/linear_regression_PyTorch_Testing_set.png)

[2] LSTM model:

![](https://github.com/criscfer/Demand_Learner/blob/main/Sample%20Result%20Images/lstm_2_months_period.png)

[3] Holt-Winters model:

![](https://github.com/criscfer/Demand_Learner/blob/main/Sample%20Result%20Images/Holt-Winter's_model_Testing_set%20-%20With%20dates.png)

## Observations

It is important to note that the recurrent neural network (LSTM) shows the most diiscrepancy between predictions and ground truth data, because of hardware and time constraints it suffered during training. The training stage for the LSTM model can take up to several hours, depending on the quality of the hardware available. For a simple 
test run of the model, training was done with a small input batch and for a small number of epochs (only 10 epochs). Therefore, the RNN's performance can be greatly improved, should better hardware be available for training it.
