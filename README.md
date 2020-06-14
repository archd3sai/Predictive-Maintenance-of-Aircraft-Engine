# Aircraft Engine RUL Prediction
Prediction of Remaining Useful Life of any machine is very essential due to its ability to prevent failure occurrences and maintenance costs. At present, mathematical and statistical modeling are the prominent approaches used for it. These are based on equipment degradation physical models and machine learning methods, respectively.

So, the objecive is to develop a system that identifies likelihood of failure of rotating equipment (for example motors, turbines) based on a stream of sensor data. The sensors monitor different parameters such as temperature, pressure and acceleration of different machine parts in order to keep a check on the performance of the rotary machine. At the server side, this data is used to train a machine learning model. This model predicts the remaining useful life (RUL) i.e., time to failure of the machine. These predictions are used to prevent failure of the machines by performing maintenance at appropriate time.

## Data
Data sets consists of multiple multivariate time series. Each data set is further divided into training and test subsets. Each time series is from a different engine – i.e., the data can be considered to be from a fleet of engines of the same type. Each engine starts with different degrees of initial wear and manufacturing variation which is unknown to the user. This wear and variation is considered normal, i.e., it is not considered a fault condition. There are three operational settings that have a substantial effect on engine performance. These settings are also included in the data. The data is contaminated with sensor noise.

The engine is operating normally at the start of each time series, and develops a fault at some point during the series. In the training set, the fault grows in magnitude until system failure. In the test set, the time series ends some time prior to system failure. The objective of the competition is to predict the number of remaining operational cycles before failure in the test set, i.e., the number of operational cycles after the last cycle that the engine will continue to operate. Also provided a vector of true Remaining Useful Life (RUL) values for the test data.

The data are provided as a zip-compressed text file with 26 columns of numbers, separated by spaces. Each row is a snapshot of data taken during a single operational cycle, each column is a different variable. The columns correspond to:

1) unit number

2) time, in cycles

3) operational setting 1

4) operational setting 2

5) operational setting 3

6) sensor measurement 1

7) sensor measurement 2

...

26) sensor measurement 26

The training set includes operational data from 100 different engines. In each data set, the engine was run for a variable number of cycles until failure. The lengths of the run varied with a minimum run length of 128 cycles and the maximum length of 356 cylces.

The testing set includes operational data from 100 different engines. The engines in the test dataset and copletely different from engines in the training data set.

## Objectives (Currently working)
Objective of this project is to implement various Predictive Maintenance methods on this dataset and assess the performance of each.

(1) Build a Classification model which predicts if an engine is going to fail using past 50 cycles data.
(2) Build a Regression model which predicts the remaining useful life of an engine using past 50 cycles data.
(3) Time Series Clustering
