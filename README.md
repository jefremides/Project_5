# California Wildfires: Measuring Economic Impact 


<br>

### DSIR - 824
#### 10/30/2020
#### Instructors:  Jeff Hale, Jacob Koehler
##### TAs:  Jobeth Muncy, Sara Soueidan, Bibor Szabo, Chuck D
  
<br>

### Authors:

- Claire Hester [Github](https://github.com/clairepetersen) | [LinkedIn](https://linkedin.com/in/claire-petersen-hester)
- Sean Cleary [Github](https://github.com/jefremides) | [LinkedIn](https://linkedin.com/in/____________)
- Jerry Efremides [Github](https://git.generalassemb.ly/jefremides) | [LinkedIn](https://linkedin.com/in/jerry-efremides)

<br>

## Problem Statement

Catastrophic wildfires in California have sweeping impacts: environmental costs, poor air quality, carbon emissions, homes lost, large numbers of people displaced, and suppression costs, to name a few. Our goal is to build a convincing argument for the redirection of funds to catastrophic wildfire prevention. For this project, we will be focusing on three factors and will set out to predict acres burned, fire suppression costs, and structures destroyed over the next 10 years.

<br>

## Executive Summary


<br>

## Tableau Visualization
[California Wildfires, 2014-2019](https://public.tableau.com/profile/claire.hester#!/vizhome/CAWildfireMap2014-2019/CAWildfireMap)

<br>

## Data Dictionary

|Feature|Type|Dataset|Description| 
|---|---|---|---| 
|Incident Number|object|fires_compiled|Assigned incident number| 
|Incident Name|object|fires_compiled|Name of fire| 
|Incident Type|object|fires_compiled|Coded Incident type| 
|Latitude|int64|fires_compiled|Latitude of the incident's point of origin| 
|Longitude|int64|fires_compiled|Longitude of the incident's point of origin|
|Size|float64|fires_compiled|The size of the incident|
|Unit of Measure|object|fires_compiled|Unit of Measure, related to Size|
|Costs|float64|fires_compiled|Associated costs, cost of fire suppression (in the case of wildfire)|
|Structures Destroyed|int64|fires_compiled|Total number of structures destroyed|
|Fire Name|object|fires_compiled|Incident Name field in all caps that will match the Fire Name field in the shapefile|
|start_date|object|fires_compiled|Start date of incident|
|year|int64|fires_compiled|Year of incident|
|county|object|fires_compiled|County that aligns with the origins latitude and longitude|
|year|int64|acres_clean|Years ranging from 1950-2020|
|acres_burned|float64|acres_clean|Acres burned per year|

<br>

## Data Sources & Information

###### Wildfire:

https://cal-adapt.org/tools/wildfire/
https://www.fire.ca.gov/
https://fam.nwcg.gov/fam-web/
https://www.fire.ca.gov/incidents/2020/
https://searchworks.stanford.edu/view/xj043rd8767


###### Economic:

https://fred.stlouisfed.org/
https://www.labormarketinfo.edd.ca.gov/data/labor-force-and-unemployment-for-cities-and-census-areas.html
http://www.californiacityfinance.com/index.php#PROPTAX
https://www.bls.gov/regions/west/california.htm#eag
http://www.dof.ca.gov/Forecasting/Economics/Economic_and_Revenue_Updates/index.html
https://www.census.gov/data/data-tools.html
http://www.insurance.ca.gov/01-consumers/120-company/04-mrktshare/


##### Social Media:

https://developer.twitter.com/


##### Geospacial:

https://www.firelab.org/project/fsim-wildfire-risk-simulation-software
https://cal-adapt.org/tools/wildfire/

##### Coding Tips and Tricks:
https://pypi.org/project/uszipcode/
https://stackoverflow.com/questions/12608788/changing-the-tick-frequency-on-x-or-y-axis-in-matplotlib/12608937


##### Additional Citations:

https://www.goldstandard.org/blog-item/carbon-pricing-what-carbon-credit-worth 
https://www.sfchronicle.com/projects/california-fire-map/air-quality/
https://www.wri.org/blog/2020/us-fires-climate-emissions
https://ww3.arb.ca.gov/cc/inventory/pubs/ca_wildfire_co2_emissions_estimates.pdf
https://resources.ca.gov/CNRALegacyFiles/wp-content/uploads/2018/05/California-Forest-Carbon-Plan-Final-Draft-for-Public-Release-May-2018.pdf
https://www.nature.org/content/dam/tnc/nature/en/documents/TNC_Pathways_2020vf.pdf
https://www.nytimes.com/2019/08/20/climate/fire-insurance-renewal.html
https://news.mongabay.com/2020/09/off-the-chart-co2-from-california-fires-dwarf-states-fossil-fuel-emissions/

<br>

##### Image Attribution:


<br>

## Conclusions:

