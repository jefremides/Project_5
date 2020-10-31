# California Wildfires: Measuring Economic Impact 


<br>

### DSIR - 824
#### 10/30/2020
#### Instructors:  Jeff Hale, Jacob Koehler
##### TAs:  Jobeth Muncy, Sara Soueidan, Bibor Szabo, Chuck D
  
<br>

## Authors:

- Claire Hester [Github](https://github.com/clairepetersen) | [LinkedIn](https://linkedin.com/in/claire-petersen-hester)
- Sean Cleary [Github](https://github.com/scleary2) 
- Jerry Efremides [Github](https://git.generalassemb.ly/jefremides) | [LinkedIn](https://linkedin.com/in/jerry-efremides)

<br>

## Problem Statement

Catastrophic wildfires in California have sweeping impacts: environmental costs, poor air quality, carbon emissions, homes lost, large numbers of people displaced, and suppression costs, to name a few. Our goal is to build a convincing argument for the redirection of funds to catastrophic wildfire prevention. For this project, we will be focusing on three factors and will set out to predict acres burned, fire suppression costs, and structures destroyed over the next 10 years.

<br>

## Executive Summary

California is home to the 10 costliest wildfires in US history.  Since 2012, not a month has gone by without a fire burning in a California forest.  To date, the CO2 emmissions from fires burned alone may exceed the entire C02 emmissions of the entire transportation industry and are estimated to exceed three times the CO2 emmissions the state's energy producers will produce to power the entire state.  

Human activity is the main cause for the increase in catostrophic wildfires and it comes in two flavors:  Climate change and the shift from forest restoration to fire supression.  Around the 1900s, the government and forest service began to look at every tree as a tax payer asset.  As a result, perscribed burns were stopped, leading to the overgrwoing of dense, thick, forestry around the state and increasing the "fuel" for widlfires.  More intense fires and longer fire seasons have increased the desctruction and cost of these wildfires, and measuring the full economic toll poses a real challenge.

After gathering data from a wide variety of sources and perspectives, we were faced with many questions and assumptions about how to quantify the economic impact, but ended up focusing on the cost of supression, and insurance damages.   We explored burn areas (visualized through Tableau, next section) as well as insurance losses in the Exploratory Data Analysis section.

We used an ensemble time series model that combined Naive Seasonal and Holt Winters models to forecast acres burned over the next 10 years. This model is solely based on acreage and does not include environmental factors, which we believe would have led to a more robust (though much more complicated) model, which we will leave to climate scientists for now. We believe we make a convincing argument that redirecting costs to fire prevention will save \\$16 billion in public funds over the next 10 years.


<br>

## Tableau Visualization
[California Wildfires, 2014-2019](https://public.tableau.com/profile/claire.hester#!/vizhome/CAWildfireMap2014-2019/CAWildfireMap)

<br>

## Contents
- 01 Data Collection
 -- claire_data
 -- jerry_data
 -- twitter
- 02 Data Cleaning
 -- claire_data_cleaning.ipynb
- 03 Exploratory Data Analysis
 -- claire_eda_fire_data.ipynb
 -- jerry_data_cleaning_eda.ipynb
- 04 Modeling
 -- claire_time_series_models.ipynb
- 05 Presentation
 -- Project 5.pdf

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

## Conclusions:

To conclude, we used an ensemble time series model to predict that over the next 10 years, nearly 13 million acres will burn, which will lead to 61,000 structures destroyed and fire suppression costs of almost \$40 billion. As it currently stands, there are 10 million acres of forest that are considered "high risk"[Source](https://www.thehour.com/news/article/Restoring-California-s-forests-to-reduce-wildfire-15643753.php). At a forest restoration cost of \\$2350 per acre, we believe that if funds were allocated to forest restoration we would see an overall savings of \$16 billion in public funds over the next 10 years.

<br>


## Areas for Further Study:

There is so much more that we should have liked to explore here. A few of our ideas include:
- An assessment of social and mental health through social media and NLP
- A deep dive into the environmental factors that cause and amplify catastrophic wildfires
- An investigation into carbon emissions and other pollutants due to wildfires
- A deeper look at the effect of catastrophic wildfires on ecosystems, including water reservoirs and water supply
- An exploration of the increase in home building in the Wilderness-Urban Interface, which leads to displacement and home loss during wildfires

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


