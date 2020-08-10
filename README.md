# deCovid 
A COVID-19 Visualization (in Delaware) and Prediction project

## Data
Data was obtained from the covidtracking.com api, using the ```daily``` csv provided at a state level in the United States, as well as a county wise dataset from [kaggle](https://www.kaggle.com/imdevskp/corona-virus-report?select=usa_county_wise.csv).

## Visualization - deCovid

The data was processed in Python with ```pandas``` in order to combine daily data into cumulative case and death counts. Then, using ```plotly```, heatmaps were created for cumulative and daily positive case and death counts.

![cumulative positive](/heatmaps/cumuPositive.png?raw=true)
![cumulative deaths](/heatmaps/cumuDeaths.png?raw=true)
![daily positive](/heatmaps/dailyPositive.png?raw=true)
![daily deaths](/heatmaps/dailyDeaths.png?raw=true)


## Prediction - COVIDPrediction

Predictions are made with ```scipy```'s ```curve_fit``` in Python. A standard exponential function was fitted to the data in order to obtain the predictions. Sample predictions are found in the {state}Predictions.csv files.

### Sample Fitted Curve
![curve](/heatmaps/samplePrediction.png?raw=true)
