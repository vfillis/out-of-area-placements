# Analysis in R



File too big for r, but filtering first, then doing formatting worked (although it meant converting the date column every time). Might have been easier to use command line / sql 

## Change in the top five trusts over the past four years

Besides CSVs, NHS Digital offers Excel files on Out of Area Placements. They include a sheet "6 - Inappropriate OAPs - Year" which contains total inappropriate Out of Area Placement days in the last 12 months. 

The Excel files for October 2020, October 2019, October 2018, and October 2017 each contain how many days patients have spent placed outside their area inappropriately in the last 12 months. In each of these files I looked up the value for the top five trusts manually. I stored the values in a new file "OAP-days-Top5-yearly-changes.csv" which can be found and downloaded [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAP-days-Top5-yearly-changes.csv).

## Distance for Birmingham and Solihull Mental Health NHS Foundation Trust

Data on the distance of Out of Area Placements can also be found in the monthly Excel files. For Birmingham and Solihull Mental Health NHS Foundation Trust I based the distance on inappropriate Out of Area Placements that were active in the past 12 months. The [Excel file "Out of Area Placements (OAPs) - October 2020 - Additional data" for October 2020 published by NHS Digital](https://digital.nhs.uk/data-and-information/publications/statistical/out-of-area-placements-in-mental-health-services/october-2020) contains this information in the sheet "6 - Inappropriate OAPs - Year". 

I stored the values in a new file "OAPs-distance-Birmingham.csv" which can be found and downloaded [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAPs-distance-birmingham.csv).

## Where are patients from Birmingham sent to?



## Bed occupancy data 

