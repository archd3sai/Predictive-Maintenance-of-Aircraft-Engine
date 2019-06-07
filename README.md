# Aircraft Engine RUL Prediction
Prediction of Remaining Useful Life of any machine is very essential due to its ability to prevent failure occurrences and maintenance costs. At present, mathematical and statistical modeling are the prominent approaches used for it. These are based on equipment degradation physical models and machine learning methods, respectively.

So, the objecive is to develop a system that identifies likelihood of failure of rotating equipment (for example motors, turbines) based on a stream of sensor data. The sensors monitor different parameters such as temperature, pressure and acceleration of different machine parts in order to keep a check on the performance of the rotary machine. At the server side, this data is used to train a machine learning model. This model predicts the remaining useful life (RUL) i.e., time to failure of the machine. These predictions are used to prevent failure of the machines by performing maintenance at appropriate time.

In this project I aim to model the task of estimating RUL of machines as a regression problem.

- Regression approach provides a prediction of the remaining useful life of the machine (in hours/cycles).

In order to accomplish this task, I built an LSTM model which can be shown below. 
![Neural-network model](https://github.com/archd3sai/Aircraft-Engine-RUL-Prediction/blob/master/Images/1.png)

The model is trained and losses can be see below.
![loss](https://github.com/archd3sai/Aircraft-Engine-RUL-Prediction/blob/master/Images/loss.png)

I used this trained model to predict the RUL of engines from the test dataset which can be seen below.
![RUL](https://github.com/archd3sai/Aircraft-Engine-RUL-Prediction/blob/master/Images/RUL.png)

