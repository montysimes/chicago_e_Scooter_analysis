<!-- Banner -->
![Banner](https://cdn.crello.com/api/media/medium/419542852/stock-photo-cropped-view-businessman-formal-wear)

# Should E-Scooters be charging into Sydney?

<!--Introduction -->
Rideshare Electric scooters have become a popular mode of transport around the world. It is claimed that they are a convenient and environmentally friendly mode of urban transport for short journeys and complement public transportation by solving the first and last mile problem. 

This project will focus on the  analysis of the data from a recent e-scooter pilot trial in Chicago, Illinois 2020. We will investigate the when, where and why of escooter usage during the trial.

Based on our findings we plan to  make a recommendation to the question; Should we conduct a similar pilot trial of e-scooters in Sydney? 

<!-- Table of Contents -->

# Table of contents

- [Should E-Scooters be charging into Sydney?](#should-e-scooters-be-charging-into-sydney)
- [Data Sources](#data-sources)
- [Data Exploration and Investigation](#data-exploration-and-investigation)
- [Models](#data-models)
- [Group Members](#group-members)
 
<!-- Data Sources -->
# Data Sources 

The datasets that will be used in this analysis are sourced from the City of Chicago database for relevant traffic surveys, and Iowa State University for weather statistics. The links to the original data sources and brief description are listed below:

* [E-Scooter Trips - 2020](https://data.cityofchicago.org/api/views/3rse-fbp6/rows.csv?accessType=DOWNLOAD)
    * Electric scooter trips taken during the 2020 Chicago pilot program. 
    * _NOTE: file size was too large for repository, data was pulled directly from link_
* [Weather Statistics](https://mesonet.agron.iastate.edu/request/download.phtml?network=IL_ASOS)
    * Weather statistics gathered by Iowa State University
    * Available in the Data folder `MDW.csv`
* [CTA - Ridership - Daily Boarding Totals](https://data.cityofchicago.org/api/views/6iiy-9s97/rows.csv?accessType=DOWNLOAD)
    * This dataset shows systemwide boardings for both bus and rail services provided by CTA
    * Available in the Data folder `CTA_-_Ridership_-_Daily_Boarding_Totals.csv`
* [Taxi Trips](https://data.cityofchicago.org/api/views/wrvz-psew/rows.csv?accessType=DOWNLOAD)
    * Taxi trips reported to the City of Chicago in its role as a regulatory agency. 
    * _NOTE: file size was too large for repository, data was pulled directly from link_
    * Summaries of the data Available in the Data folder under `Taxi_Summary.csv` and `Taxi_Count_Summary.csv`
* [Traffic Crashes - Vehicles](https://data.cityofchicago.org/api/views/68nd-jvt3/rows.csv?accessType=DOWNLOAD)
    * This dataset contains information about vehicles involved in a traffic crash.
    * _NOTE: file size was to large for repository, data was pulled directly from link_
    * Summaries of the data available in the Data folder under `Traffic_Incident_Summary.csv.csv` 
* [Chicago community area population](https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Boundaries-Community-Areas-current-/cauq-8yn6)
    * This dataset contains information about community area population, area and density for Chicago
    * Available in the Data folder `chicago_community_population.csv`
* [Boundaries - Community Areas](https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Boundaries-Community-Areas-current-/cauq-8yn6#Export)
    * Current community area boundaries in Chicago.
    * Available in the Data folder `Boundaries - Community Areas (current).geojson`

The datasets were cleaned and joined to create two data frames from which models could be built.

The notebook which generates the dataframe for the regression modelling is `Regression Data Frame.ipynb` located in the Data_Cleaning folder. The output csv is located in the Data folder under `Regression_Model_Data.csv`.

The notebook which generates the dataframe for the clustering modelling is `Clustering data frame.ipynb` and the output csv is located `Clustering_data.csv` & `Clustering_data_Summary.csv`

<!-- Data Exploration and Investigation -->

# Data Exploration and Investigation

The datasets were explored and insights noted within the folowing notebooks available in the Data_Exploration Folder: 
1. `Escooter Data Exploration.ipynb`
    - 1.1	Importing Data
    - 1.2	Identifying and Addressing Outliers
    - 1.3	Investigating Null Values
    - 1.4	Distribution of Trip Volume by Starting Location Between Community Areas
    - 1.5	Distribution of Trip Volume by End Location Between Community Areas
    - 1.6	Migration of E-scooter Trips between Community Areas
    - 1.7	E-scooter Usage During The Program by Number of Trips
    - 1.8	E-scooter Usage During the Program by Total Distance Travelled and Total Duration of Trips
    - 1.9	Vendor Investigation
    - 1.10	Summary

2. `Taxi_Trips_Clean.ipynb`
    - 2.1.1 Importing and exploring data
    - 2.1.2 Addressing Outliers
    - 2.1.3 Filtering Data for August to December 2020
    - 2.1.4 Time Series during August to December 2020
    - 2.1.5 Filtering Data for final dataframe
    - 2.1.6 Summary

3. `Ridership_Data_Clean.ipynb`
    - 3.2.1 Importing and exploring data
    - 3.2.2 Filtering Data for August to December 2020
    - 3.2.3 Time Series during August to December 2020
    - 3.2.4 Filtering for final dataframe
    - 3.2.5 Summary
   
4. `Vehicle_Crash_Data_Clean.ipynb`
    - 4.1 Importing and cleaning data
    - 4.2 Filtering Data for August to December 2020
    - 4.3 Crash exploration by vehicle analysis
    - 4.4 Total daily crashes
    - 4.5 Summary

5. `Chicago_population_clean.ipynb`
    - 5.1 Importing and exploring
    - 5.2 Cleaning data
    - 5.3 Population exploration
    - 5.4 Summary

6. ``
7. ``
8. ``

<!-- Data Models -->

# Data Models

The following regression models were built to model the number of escooter trips completed during the trial:
- `Linear_Regression_Model.ipynb`
- `Decision Tree.ipynb`

The following clustering models were built to attempt to identify the uses of escooters during the trial:
- `Hierarchical Clustering .ipynb`
- `Hierarchical Clustering of trips .ipynb`

<!-- Group Members -->

# Group Members

Montgomery Simes 46437819

Christian Hallgren 45426465

Allan Mawande 45691215

James Folbigg 45946191
