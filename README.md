# Predictive Maintenance of Aircraft Engine

Predictive Maintenance techniques are used to determine the condition of an equipment to plan the maintenance/failure ahead of its time. 

## Data
Data sets consists of multiple multivariate time series. Each data set is further divided into training and test subsets. Each time series is from a different engine – i.e., the data can be considered to be from a fleet of engines of the same type. Each engine starts with different degrees of initial wear and manufacturing variation which is unknown to the user. This wear and variation is considered normal, i.e., it is not considered a fault condition. There are three operational settings that have a substantial effect on engine performance. These settings are also included in the data. The data is contaminated with sensor noise.

The engine is operating normally at the start of each time series, and develops a fault at some point during the series. In the training set, the fault grows in magnitude until system failure. In the test set, the time series ends some time prior to system failure. The objective of the competition is to predict the number of remaining operational cycles before failure in the test set, i.e., the number of operational cycles after the last cycle that the engine will continue to operate. Also provided a vector of true Remaining Useful Life (RUL) values for the test data.

The training set includes operational data from 100 different engines. In each data set, the engine was run for a variable number of cycles until failure. The lengths of the run varied with a minimum run length of 128 cycles and the maximum length of 356 cylces. The testing set includes operational data from 100 different engines. The engines in the test dataset and copletely different from engines in the training data set.

## Objectives
Objective of this project is to implement various Predictive Maintenance models and assess the performance of each. The various models are shown below.

- Exponential Degradation model for RUL Prediction
- Similarity-based model for RUL Prediction
- LSTM model for RUL Prediction

- RNN for Binary and Multiclass classification
- LSTM for Binary and Multiclass classification
- GRU for Binary and Multiclass classification
- 1D CNN for Binary and Multiclass classification

To Do:
- Autokeras failure prediction
- Tsfresh 
- DTW and Time series clustering
- Genetic Algorithm
- Hidden Markov Models
- Survival Analysis
- Autoencoder






## References

[https://www.mathworks.com/help/predmaint/ug/rul-estimation-using-rul-estimator-models.html]

