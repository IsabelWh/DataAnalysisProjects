# Housing Market Analysis

## Objectives:

1 - To describe key market trends for house prices in England and Wales over a 5 year period (2019-2023). 

2- To identify regional property hotspots (places with the largest % increase of average house price)

## Data

-This is a large dataset taken from HM Land Registry Price Paid Data. 

-Five csv files, one for each year(January 2019 and December 2022).

-Each row is an individual transaction, containing Price Paid data for England and Wales 

-Contains HM Land Registry data © Crown copyright and database right 2021. This data is licensed under the Open Government Licence v3.0.

## Actions using Excel:

- Cleanse: Removed any columns that were irrelevant to this project to save memory, as it is a large dataset. Removed the 5th property type of 'Other', as this is an unpredictable category and has the potential to skew the validity of these results. Calculated and removed outliers in the Price Paid column using IQR.
- To assign each county to a region, I created a Lookup table and then used VLOOKUP to add a new column for County.
- I used pivot tables to work out the average price paid for each region by year.
- To save memory, I then copied the key values into a summary table in a new workbook, then calculated the average price increase from 2019 to 2023 to create the visualisations.


## Actions using Power BI:

- I appended the datasets to each other and created a choropleth map using the filled maps function and a custom topojson file I made. I fine tuned it and chose a colour theme that is accessible for people who are colourblind. If used in a PowerBI report this would be a useful interactive tool.

## Visualisations

Average Price Paid 2019-2023
![Alt text](https://github.com/IsabelWh/DataAnalysisProjects/blob/main/PriceByType.png)


![Alt text](https://github.com/IsabelWh/DataAnalysisProjects/blob/main/RegionalOverview.png)

Property Hotspots Map 2019-2023
![Alt text](https://github.com/IsabelWh/DataAnalysisProjects/blob/main/ChoroplethHotspot.png)

## Reflection

- If I have time, I will create a PowerBI dashboard to allow users to explore the data in their own time.
