# codefundopp_2018
Idea for 2018 codefundo++

# TITLE : Earthquake magnitude forecasting over the Indian subcontinent using Artificial Neural Network (ANN) methods from past seismic datasets

## Source of Data: United States Geological Survey (USGS) earthquake catalog : Link: https://earthquake.usgs.gov/earthquakes/search/

## Methodology and Steps involved:

#### Obtaining the catalog data (spatial and temporal) from USGS website. 
#### Declustering the catalog to filter the mainshocks using method suggested by Gardner and Knopoff (1974).

#### Use of 6 seismic indicators as parameters-
    > the frequency of foreshocks (n events) before a mainshock during the time under consideration
    > Mean magnitude of the last n events
    > Rate of seismic energy release
    > b value obtained from Gutenberg-Richter relation 
    > Difference between maximum occurred and maximum expected magnitude for an event
    > Mean time difference between characteristic events

#### Division of study area in a requisite number of tiles.
#### Feature extraction and feauture modeling put of the chosen 6 parameters
#### Generating a hypothesis by using Artificial Neural Networks
#### Training this hypothesis with training dataset and optimizing the cost function.
#### Running the model on the same spatial location (same grid and same tilings) in a new time-stepping and with different seismic         indicators to predict the probability of an earthquake to cross a certain magnitude threshold "m". This magnitude threshold is a user defined paramter. 
#### Creating Heat maps on the basis of numerous iteration results.
