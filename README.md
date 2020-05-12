# Bayesian Rt Estimation and Epidemiological New Case Prediction for Indian States

This is a python script for estimation  of transmissibility, future case prediction and adaptive control of COVID-19 in Indian States.
  

## Data 

Timeseries data for Indian States can be downloaded from [COVID-19 in India](https://www.kaggle.com/sudalairajkumar/covid19-in-india)

To run the script at a terminal:

```
python indian_states_estimation_prediction.py
```
This will produce 3 images per State (States with less than 10 cases are not shown):

*The timeseries of new cases, showing also smoothing with a moving 5 day window (the number of days is a parameter)

<img src="./images/NewCases_Timeseries_Uttar Pradesh.png" >

*The running time estimation of Rt

<img src="./images/Rt_Estimation_Uttar Pradesh.png" >

*The running prediction of new cases (anomalies are shown as cases the  model did not initially predict well) in blue, with a two weeks forward prediction of adaptive control to bring Rt=0.9<1.

<img src="./images/Observed_Predicted_New_Cases_Control_Rtarget_Uttar Pradesh.png" >


## Issues:

The code is very simple, other versions are available for [nations, cities and US counties](https://github.com/mansueto-institute/Rt_Real-time_Estimation_Case_Prediction), without adaptive control. 

A much improved version applying to many [interconnected units with a movement matrix](https://github.com/mansueto-institute/adaptive-lockdown) is also available.

All codes are still under development and will continue to change.

## Authors

* [Luis M. A. Bettencourt](https://twitter.com/BettencourtLuis)

## License

This project is licensed under the MIT License.
