<!-- Banner -->
![Banner](https://cdn.crello.com/api/media/medium/419542852/stock-photo-cropped-view-businessman-formal-wear)

# Chicago E-Scooters Analysis

<!--Introduction -->

This analysis was part of my contribution to a group assignment which aimed to answer the question "Should Sydney adopt an E-scooter program?".

This project will focus on the  analysis of the data from a recent e-scooter pilot trial in Chicago, Illinois 2020. 

<!-- Data Sources -->
# Data Sources 

The datasets that will be used in this analysis are sourced from the City of Chicago database for relevant traffic surveys, and Iowa State University for weather statistics. The links to the original data sources and brief description are listed below:

* [E-Scooter Trips - 2020](https://data.cityofchicago.org/api/views/3rse-fbp6/rows.csv?accessType=DOWNLOAD)
    * Electric scooter trips taken during the 2020 Chicago pilot program. 
    * _NOTE: file size was too large for repository, data was pulled directly from link_
* [Boundaries - Community Areas](https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Boundaries-Community-Areas-current-/cauq-8yn6#Export)
    * Current community area boundaries in Chicago.
    * Available in the Data folder `Boundaries - Community Areas (current).geojson`


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
