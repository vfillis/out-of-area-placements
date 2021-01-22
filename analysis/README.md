# Analysis in R



File too big for r, but filtering first, then doing formatting worked (although it meant converting the date column every time). Might have been easier to use command line / sql 

## Change in the top five trusts over the past four years

Besides CSVs, NHS Digital offers Excel files on Out of Area Placements. They include a sheet "6 - Inappropriate OAPs - Year" which contains total inappropriate Out of Area Placement days in the last 12 months. 

The Excel files for October 2020, October 2019, October 2018, and October 2017 each contain how many days patients have spent placed outside their area inappropriately in the last 12 months. In each of these files I looked up the value for the top five trusts manually. I stored the values in a new file "OAP-days-Top5-yearly-changes.csv" which can be found and downloaded [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAP-days-Top5-yearly-changes.csv).

## Distance for Birmingham and Solihull Mental Health NHS Foundation Trust

Data on the distance of Out of Area Placements can also be found in the monthly Excel files. For Birmingham and Solihull Mental Health NHS Foundation Trust I based the distance on inappropriate Out of Area Placements that were active in the past 12 months. The [Excel file "Out of Area Placements (OAPs) - October 2020 - Additional data" for October 2020 published by NHS Digital](https://digital.nhs.uk/data-and-information/publications/statistical/out-of-area-placements-in-mental-health-services/october-2020) contains this information in the sheet "6 - Inappropriate OAPs - Year". 

I stored the values in a new file "OAPs-distance-Birmingham.csv" which can be found and downloaded [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAPs-distance-birmingham.csv).

## Where are patients from Birmingham sent to?

The monthly Excel files also provide an overview over where patients from a sending organisation are being placed. For every month, this can be found in the sheet "8 - Sender and Receiver". To find out where patients from Birmingham and Solihull Mental Health NHS Foundation Trust have been sent to in the past 12 months I went through the Excel files from October 2020 back to November 2019. In the sheet "8 - Sender and Receiver" I filtered for the Birmingham and Solihull Mental Health NHS Foundation Trust and stored the values in a new file "OAPs-birmingham-receiving-organisations.xlsx" which can be found [here](). 

I used a pivot table to get the total days for each receiving organisation in the past 12 months. 

## Bed occupancy data 

Quarterly bed occupancy data is [published by NHS England](https://www.england.nhs.uk/statistics/statistical-work-areas/bed-availability-and-occupancy/bed-data-overnight/). For the top five trusts I looked up what their average daily mental health bed occupancy was in Q2 2020/21 (July to September 2020) since this was the latest available data. 

Additionally, I manually went through the bed occupancy files from Q4 2015/16 to Q2 2020/21 to find out since when the bed occupancy in Birmingham and Solihull Mental Health NHS Foundation Trust is staying above 95%. 

I stored the values in a new file "OAPs-bed-occupancy-top-5.csv" which can be found and downloaded [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAPs-bed-occupancy-top-5.csv). 
