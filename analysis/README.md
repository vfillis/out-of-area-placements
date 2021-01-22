# The analysis

I carried out the analysis in R and Excel. The following gives an overview over what tool I used for which aspect. 

## Inappropriate Out of Area Placements in England

I analysed inappropriate Out of Area Placements active at the end of the month, days, costs, and receiving organisations in England using R. 

The markdown can be found [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAPs-England.Rmd). 

## Inappropriate Out of Area Placements in the top five trusts

I analysed inappropriate Out of Area Placements days and costs in the top five trusts using R. I didn't base comparisons between the trusts on inappropriate Out of Area Placements that were active at the end of the month as they are subject to rounding. This means the number of active OAPs each month ranges in an interval of -2 and +2. These rounding differences could result in a different order of trusts.

The markdown can be found [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAPs-top-trusts.Rmd). 

## Inappropriate Out of Area Placements in Birmingham and Solihull Mental Health NHS Foundation Trust

I analysed inappropriate Out of Area Placements days and costs in Birmingham and Solihull Mental Health NHS Foundation Trust using R. 

The markdown can be found [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAPs-Birmingham.Rmd). 

## Change in the top five trusts over the past four years

Besides CSVs, NHS Digital offers Excel files on Out of Area Placements. They include a sheet <b>"6 - Inappropriate OAPs - Year"</b> which contains total inappropriate Out of Area Placement days in the last 12 months. 

The Excel files for October 2020, October 2019, October 2018, and October 2017 each contain how many days patients have spent placed outside their area inappropriately in the last 12 months. In each of these files I looked up the value for the top five trusts manually. I stored the values in a new file "OAP-days-Top5-yearly-changes.csv" which can be found and downloaded [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAP-days-Top5-yearly-changes.csv).

## Distance for Birmingham and Solihull Mental Health NHS Foundation Trust

Data on the distance of Out of Area Placements can also be found in the monthly Excel files. For Birmingham and Solihull Mental Health NHS Foundation Trust I based the distance on inappropriate Out of Area Placements that were active in the past 12 months. The [Excel file "Out of Area Placements (OAPs) - October 2020 - Additional data" for October 2020 published by NHS Digital](https://digital.nhs.uk/data-and-information/publications/statistical/out-of-area-placements-in-mental-health-services/october-2020) contains this information in the sheet <b>"6 - Inappropriate OAPs - Year"</b>. 

I stored the values in a new file "OAPs-distance-Birmingham.csv" which can be found and downloaded [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAPs-distance-birmingham.csv).

## Where are patients from Birmingham sent to?

The monthly Excel files also provide an overview over where patients from a sending organisation are being placed. For every month, this can be found in the sheet <b>"8 - Sender and Receiver"</b>. 

To find out where patients from Birmingham and Solihull Mental Health NHS Foundation Trust have been sent to in the past 12 months I went through the monthly Excel files from October 2020 back to November 2019. I filtered for the Birmingham and Solihull Mental Health NHS Foundation Trust and used a pivot table to get the total days for each receiving organisation in the past 12 months.

I stored the values in a new file "OAPs-birmingham-receiving-organisations.xlsx" which can be found and downloaded [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAPs-birmingham-receiving-organisations.xlsx). 

## Bed occupancy data 

Quarterly bed occupancy data is [published by NHS England](https://www.england.nhs.uk/statistics/statistical-work-areas/bed-availability-and-occupancy/bed-data-overnight/). For the top five trusts I looked up what their average daily mental health bed occupancy was in Q2 2020/21 (July to September 2020) since this was the latest available data. 

Additionally, I manually went through the bed occupancy files from Q4 2015/16 to Q2 2020/21 to find out since when the bed occupancy in Birmingham and Solihull Mental Health NHS Foundation Trust is staying above 95%. 

I stored the values in a new file "OAPs-bed-occupancy-top-5.csv" which can be found and downloaded [here](https://github.com/vfillis/out-of-area-placements/blob/main/analysis/OAPs-bed-occupancy-top-5.csv). 
