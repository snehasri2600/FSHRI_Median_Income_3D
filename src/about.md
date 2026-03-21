## About the Data

The data used in this dashboard merges two datasets:

1. [New York City's Flood Vulnerability Index](https://data.cityofnewyork.us/Environment/New-York-City-s-Flood-Vulnerability-Index/mrjc-v9pm/about_data)
2. [Median Household Income in past 12 months (inflation-adjusted dollars to last year of 5-year range)](https://www.arcgis.com/home/item.html?id=c9faa265b82848498bc0a8390c0afa65)

### NYC's Flood Vulnerability Index (FVI)
<br>

The FVI dataset includes a series of features aimed at assesing different neighborhodds' vulnerability to flooding events. It includes both current and future predictions of extreme flooding events in the city, along with the Flood Susceptibility to Harm and Recovery Index (FSHRI).

The FSHRI is primarily a socioeconomic variable, where calculations were made (ranging from 1-5) based on 12 different factors. All factors were sourced from the U.S. Census Bureau's Decennial Survey in 2020 and the American Community Survey (ACS) from 2016-2020. The factors themselves are based on race, gender, age, healthcare access, English-speaking ability, and poverty rates. An aggregation of these variables, combined with the flooding scenarios in the larger dataset, gives us the FSHRI. 

A complete description of the FSHRI calculations, along with other variables within the dataset, can be found in the original dataset's [documentation](https://www.nyc.gov/assets/climate/downloads/pdfs/NYC-VIA-Report.pdf).
<br>
<br>

### Median Household Income
<br>

The median household income values for this dataset came from the U.S. Census Bureau's American Community Survey (ACS) from 2020-2024. Since this dashboard is focused on building an interactive map experience, the dataset was downloaded directly from Esri's ArcGIS Living Atlas of the World, with underlying geography included. The original dataset includes values for median household incomes as separated by age, gender, race, etc. This map includes the overall median household income for each census tract. Additional information about how 5-year estimates are calculated and adjusted for inflation (used in this dashboard) can be found at [the Census Bureau's website](https://www.census.gov/programs-surveys/acs/guidance/estimates.html).