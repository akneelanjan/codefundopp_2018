# codefundopp_2018
Idea for 2018 codefundo++

# TITLE : Earthquake magnitude forecasting over the Indian subcontinent using Artificial Neural Network (ANN) methods from past seismic datasets

## Source of Data: United States Geological Survey (USGS) earthquake catalog : Link: https://earthquake.usgs.gov/earthquakes/search/

## Methodology and Steps involved:

#### Obtaining the catalog data (spatial and temporal) from USGS website. 
#### Declustering the catalog to filter the mainshocks using method suggested by Gardner and Knopoff (1974).

#### Use of 7 seismic indicators as parameters-
    > the frequency of foreshocks (n events) before a mainshock during the time under consideration
    > Mean magnitude of the last n events
    > Rate of seismic energy release
    > b value obtained from Gutenberg-Richter relation 
    > Difference between maximum occurred and maximum expected magnitude for an event
    > Mean time difference between characteristic events
    > Source depth

#### Division of study area in a requisite number of tiles.
#### Feature extraction and feature modelling out of the chosen 7 parameters

#### Seven seismic parameters shall be passed as an input to seven neurons and one set of input features corresponding to 1 month. In this case, two hidden layers will be, each with 12 neurons. We shall use Matlab for the training and testing. Total number of synaptic connections would be given by w=(I+1)a1 + (a1+1)a2 + (a2+1)O

#### Generating a hypothesis by using Artificial Neural Networks
#### Training this hypothesis with training dataset and optimizing the cost function.
#### Running the model on the same spatial location (same grid and same tilings) in a new time-stepping and with different seismic         indicators to predict the probability of an earthquake to cross a certain magnitude threshold "m". This magnitude threshold is a user defined parameter. 
#### Creating Heat maps on the basis of numerous iteration results, representing the probabilities of exceedance of a given magnitude.
