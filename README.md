# GilaBN #

R script used to preprocess Gila data, construct a BN Structure, and implement the BN Model for three scenarios (natural, scenario 1, and scenario 2).

This documents describes the scripts used to run the Bayesian network for the revisiting the the Gila Project (O.G. 2014).

The required scripts are:
- 1-gila-preprocessing.Rmd
- 2-gila-BNstructure.Rmd

##R Notebooks##

#1-gila-preprocessing.Rmd#

This R notebook is used to process the existing hydrology (Gila at Gila River USGS gage No.09430500). Conditional probabilities for inundation and recession rates are calculated in this script. Recession rates were calculated using information for site 1 only for this recreation of the historical model/process.

#2-gila-BNstructure.Rmd#

This R notebook is used to used to build and Bayesian network used to infer recruitment potential. Conditional probabilities for each node are populated using results from the "1-gila-preprocessing.Rmd".**Bayesian networks** are a class of graphical models that allow a concise representation of the probabilistic dependencies between a given set of random variables as a **directed acyclic graph** where each node represents a random variable.
