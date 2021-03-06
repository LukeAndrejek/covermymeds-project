# CoverMyMeds Project: Predicting Prior Authorization Volume

This directory contains files in which I build and analyze a model of prior authorization (PA) volume from a dataset provided by CoverMyMeds.

CoverMyMeds is a healthcare company whose products include an electronic solution for filling out a PA, which is a form that patients can use to dispute an insurance company's rejection of a medication insurance claim. I chose to predict PA volume because CoverMyMeds uses PA volume as a predictor of revenue. Therefore, PA volume forecasting can directly benefit financial forecasting.

Here is a link to a video explaining my model:
https://youtu.be/FLShWBwDhfM

I used Holt-Winters seasonal models to predict daily PA volume on workdays and non-workdays. The model was trained using data from January 2017 through March 2019, and it was tested on data from April 2019 through December 2019. The following graph shows the performance of the best performing model at a monthly level:
![](https://raw.githubusercontent.com/LukeAndrejek/covermymeds-project/main/Images/Monthly_PA_Volumes.png)

This model achieves an accuracy on the testing set of 98.33%. Details of the model construction and accuracy calculation can be found in the above Jupyter notebook.
