# UK Bird Species Trend Indicator

## Situation (fictitious):

An environmental concern organisation has requested a tool to help users view and understand information about long and short term species trends of birds in England based on official studies. 


## Task:

Create an interactive report that shows the key info about long and short term trends of individual bird species in England. This will help users easily look up a species and visualise whether the population has increase or decreased in both the long and short term, using data collected from official studies.

## About the Data

The data is contained in a csv file entitled 'Wild Bird Populations in England' sourced from the [UK government website](https://www.data.gov.uk/dataset/dbdf36bb-5ae9-45d7-a96b-834a6e9cb655/wild-bird-populations-in-england).

The file is a flat dataset that contains data about location, species, short/long term study duration (between years), short/long term percentage change and short/long term trends.

##Actions using Excel:

Before opening in PowerBi, I opened this file in Excel to simplify the type column to a more useable format and remove the introduction cells. The type column was now renamed to location and contains the following values: Water and Wetland, Woodland, Upland, Farmland, Other and Seabird.

## Actions using PowerBI:
 
### Data View

I loaded this dataset into data view transformed it in Power Query. I split the duration columns (text type) to start and end columns (date/year type) for both long and short term time periods. I also split the species column into name and latin name columns. I removed blank rows and columns. Next, I created references to the main sheet and created a separate table for Species Key, Locations, Calendar, Trends, Short Term Trends and Long Term Trends.

### Relationship View

After applying the changes above, I created one to many relationships between the tables, using Name, Date and Location and making sure to hise the Name and Location columns from the Key tables.

### Report View

In report view, I chose a colour theme and added visuals based on the data. I was initially planning on having line graphs to show the species trends, but I only had 2 dates to work with. This would present an over simplistic line chart with a straight line, so I decided to use a gauge to display and compare both long and short term trends. 

I then created the interactive dashboard pictured below. Please see the 'Result' section below for an explanation of the features.

## Result:

The dashboard has the following features:

-A filter by species, using the name column for simplicity. It allows the user to only select one option at a time.

-A colourful treemap of distribution of all species across the six locations studied, the locations the selected bird is found in will be in the spotlight when one is selected in the filter.

-Cards for Species name, Latin name, and Long term trend, that change when a different bird is selected.

-Gauges for Long term % population change and Short term % population change. As the values are often quite close together, I have change the colour fill to have a conditional formula so that all values under 0 are red and all over are blue, so the user can quickly identify a decline or increase to the population.

-Adjoining the gauges I have put 2 cards that change depending on the long/short term study start years, this helps add more context to the information presented.


![Alt text](https://github.com/IsabelWh/DataAnalysisProjects/blob/main/Blackbird.png)


![Alt text](https://github.com/IsabelWh/DataAnalysisProjects/blob/main/Wren.png)


![Alt text](https://github.com/IsabelWh/DataAnalysisProjects/blob/main/Avocet.png)

