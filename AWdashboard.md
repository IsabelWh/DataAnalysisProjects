# Adventure Works Dashboard

## Situation (fictitious):

Adventure World Company has requested a tool, for use by staff across the company, to quickly analyse and visualise KPIs of the company and gain insights into performance.

This will help inform and shape their decision making for the future.

## Task:

Develop an interactive dashboard in PowerBI to allow others to analyse and visualise Adventure Works Sales data.

This tool must be suitable for use by those with only basic IT skills and present information clearly and simply. 

## About the Data

-The data provided consists of 7 csv files:
  -Calendar
  -Customer
  -Territories
  -Sales
  -Returns
  -Products
  -Product Categories

## Actions using PowerBI:
 
### Data View

I loaded the csv files into PowerBI and inspected them. 

Then I transformed the data by changing column types, renaming tables, appending the 3x sales tables to one table, creating conditional columns and creating new date and time columns from the calendar table. 

### Relationship View

I normalised the database by creating a <b>data model</b>. I connected the the tables through cardinality, by 'one to many' relationships based on columns such as OrderDate and TerritoryKey.

Next, I created Measures (using DAX formulas) for Revenue, Returns, Profits etc, in their related columns to keep it tidy and easy to work with. 

### Report View

Using report view, I imported the logo first, to inform my decision making regarding the colour scheme and themes.

I then created the interactive dashboard pictured below. Please see the 'Result' section below for an explanation of the features.

## Result:

The dashboard has the following features:

- An interactive Date slider, to select a time between two dates in the sales records, this changes the output in all of the visualisations
  
- A Country slicer, including a 'Select all' button to easily refresh the filters. this changes the output of the visualisations to show the info relating to one or more countries.
  
- A card for Top Product by profit and A card for Top Product by orders.
  
- A treemap of the Total Orders by Category
  
- A matrix chart showing Category, Total Orders and Return Rate

- 3 KPI cards

- A nested Bar Chart showing Total Orders By Subcategory

![Alt text](https://github.com/IsabelWh/DataAnalysisProjects/blob/7004ed15ecc8db05c0b4330cf29aad34c2558342/AW_dashboard_screenshot.png)


