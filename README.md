# seattle_Police
Feature-engineering, time-series forecasting, big data, PySpark, Python, OpenRefine

This project used 4.3 million rows of police call data downloaded from the Seattle Open Data Project.
It used that data to assess police calls before and during COVID and the Black Lives Matter protest to gauge the impact of
those events on policing behaviors and resources. 

The project entailed using OpenRefine to fix naming irregularities in the raw data and to do some initial aggregation;
using PySpark in Google Cloud for cleaning, feature engineering, and further aggregations; and using Python Jupyter notebooks
for final cleaning, determining the ARIMA model parameters, and running the ARIMA models.

The repository contains the following elements:

* openrefine_rules_seattle.txt -- a file of json code that contains the rules
  for the OpenRefine transformations

* seattle_data_clean_sparkDay.ipynb -- a PySpark Jupyter notebook to run in the cloud; it does
  a series of transformations and returns a 'clean' data set aggregated by day

* Last_mile_cleaning.ipynb -- a Python notebook containing a short script to handle
  missing values

* seattle_arima_explore.ipynb -- a Python notebook used to generate the weights for each
  of the ARIMA models
  
* seattle_arima.ipynb -- a Python notebook with a script that takes in the processed
  data and outputs the ARIMA forecast data

