# Thousands of heat and hot water complaints from an address in the Bronx. City blames one woman.

This project analyses 311 service requests related to heat and hot water from NYC Open Data. It explores the complaints on the zip code level from 2020 to 2022. The data has been normalized by the zip code level population data gathered from U.S. Census Bureau. It also explored the complaints at the tract level for 2021.

## Guide to the repository ##

1. `notebooks:` This folder contains all the python notebook. 

* `census.ipynb` contains the code that was used make calls to the U.S. Census API, and gather census tract codes from censusgeocode.
Zip code level data on population, race, median income and percentage below poverty was collected for this project. Tract level data on population, race and percentage below poverty was collected.
It must be noted that the U.S. Census Bureau releases estimates every year. It publishes American Community Survey (ACS) 5-year and 1-year data. 
ACS-5 released in the year 2020 and 2021 have been used for analysis. The data for 2022 is yet to be made available by the Bureau through the API. 
Therefore, 2021 data has been considered for 2022 in the analysis in the zip code level.
At the tract level, complaints from 2021 have been used against census data from 2021.

* `analysis_tract.ipynb` contains the code used to run regression analysis to assess which variable causes a statistically significant change in the complaints at the tract level.

* `analysis_zip.ipynb` contains the code used to run regression analysis to assess which variable causes a statistically significant change in the complaints at the zip code level.

2. `docs:` This folder contains the parquet and csv files for the 311 data, census data and zip codes. 

3. The story has been written on a html page and the code for the same can be found on `index.html`.

Link to the story - https://poojachaudhuri.github.io/311-complaints-bronx/
