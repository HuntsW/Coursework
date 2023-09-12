# Selangor Flood Modelling

This is a compilation of the code for a flood modelling project focused on predicting floods Selangor, Malaysia based off data from NASA's Integrated Multi-satellitE Retrievals for GPM (IMERG) product for use as a final year project.

Each of the main files/folders of this project are as follows:

Website Files - A set of files used to set up a basic HTML website to present the models constructed throughout this project. Files in this folder include app.py (main python script for running the html website using Flask), IMERG_scraper.py (python script to scrape the IMERG database for the most recent data), various .pkl files (python pickle files used to store trained models), SelangorMap.png (image of Selangor used in visualization), and a standard index.html file.

Flood Model Comparison (HQprecip) - A jupyter notebook that contains code for preprocessing the HQprecipitation Data.csv file (also found in this repository) and training several machine learning models on it in order to generate flood predictions for the area of interest. High Quality precipitation data comes primarily from processed satellite data.

Flood Model Comparison (PrecipCal) - A jupyter notebook that contains code for preprocessing the precipitationCal Data.csv file (also found in this repository) and training several machine learning models on it in order to generate flood predictions for the area of interest. Precipitation Calibrated data comes from calibrating processed satellite data with local gauge station data and average rainfall amounts.

IMERG_Loader - A python script to download 10 years of rainfall data gathered from the NASA IMERG data product and to perform some preprocessing on it to prepare the two .csv files above. (NOTE: Running this script may take upwards of 5 hours for it to complete).

River-specific Flood Model (Failed) - Attempt at a flood model that can further specify its predictions down to a specific river in Selangor. Failed primarily due to a lack of data, however other solutions may exist for this.
