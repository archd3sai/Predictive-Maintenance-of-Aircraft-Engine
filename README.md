# Predictive Maintenance (PdM) of Aircraft Engine

Predictive Maintenance techniques are used to determine the condition of an equipment to plan the maintenance/failure ahead of its time. This is very useful as the equipment downtime cost can be reduced significantly. 

The objective of this project is to implement various Predictive Maintenance methods and assess the performance of each. Each method can be classified broadly into two categories.

1. Classification: Predicting the failure of machine in upcoming n days
2. Regression: Predicting the remaining useful life of a machine 

## Data
Data sets consists of multiple multivariate time series. Each time series is from a different engine – i.e., the data can be considered to be from a fleet of engines of the same type. You can find the data [here](https://www.kaggle.com/datasets/behrad3d/nasa-cmaps).

The engine is operating normally at the start of each time series, and develops a fault at some point during the series. In the training set, the fault grows in magnitude until system failure. In the test set, the time series ends some time prior to system failure. 

The training set includes operational data from 100 different engines. The lengths of the run varied with a minimum run length of 128 cycles and the maximum length of 356 cylces. The testing set includes operational data from 100 different engines. The engines in the test dataset and copletely different from engines in the training data set.

## EDA

## Models for Predictive Maintenance

(1) Exponential Degradation model for RUL Prediction

(2) Similarity-based model for RUL Prediction

(3) LSTM model for RUL Prediction

(4) LSTM model for binary and multiclass classification

(5) RNN model for binary and multiclass classification

(6) 1D CNN for binary and multiclass classification

(7) 1D CNN-SVM for binary classification

### Experimenatation


## To Do:
- Autokeras failure prediction
- Tsfresh 
- DTW and Time series clustering
- Genetic Algorithm
- Hidden Markov Models
- Survival Analysis
- Autoencoder






## References

https://www.mathworks.com/help/predmaint/ug/rul-estimation-using-rul-estimator-models.html

