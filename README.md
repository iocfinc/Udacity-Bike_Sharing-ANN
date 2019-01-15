# Udacity-Bike_Sharing-ANN

## Background

This project was created as part of the requirements for Udacity's Deep Learning Nanodegree. This is the project for the Artificial Neural Network module of the course.

The objective of this project is to for us to create our first Artificial Neural Network and use this network to create a model that would forecast daily ridership from the previous data. In this project we had to define our forward pass and backpropagation functions with the use of NumPy. We had to read about loading and preparing data for input to the model and splitting to test, train and validation sets.

The goal of the ANN was to provide a forecast of daily ridership for a given time on a given day to allow the company to allocate its resources to serve the demand.

## Results

The metric we were asked to monitor was the losses for the validation and training set. After 2000 iterations we are able to plot the losses in the graph below.

<p align="center"><img src='.\images\LOSS-ANN.png' width=500px alt = "boxer"></p>

The final result was `Progress: 100.0% ... Training loss: 0.079 ... Validation loss: 0.177`.

Once we were done with training the neural network, we then used it to provide a prediction of the possible ridership for ~21 days and compare it to the actual data on the same period. The resulting graph of Prediction vs. Actual is seen in the graph below.

<p align="center"><img src='.\images\ANN-RESULTS.png' width=1000px alt = "boxer"></p>

The ANN was able to provide a good approximation of the data although obviously it still had some difficulty in forecasting ridership in certain cases like during holidays (Dec 20-31) where it still expected a substantial number of ridership.

## Possible Improvements

Since this is a time series forecasting, it could also be a good idea to test out a different model more suited to time series data like RNNs and LSTMs.