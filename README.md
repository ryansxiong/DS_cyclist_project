# DS Cyclist Project

## Codes and Resources Used
* **Python Version**: 3.8
* **Packages**: Pandas, Numpy, Matplotlib
* **Visual Tools**: Tableau
* **License for data**: https://www.divvybikes.com/data-license-agreement
* **Link to combining multiple CSV files**: https://www.youtube.com/watch?v=dcQs8k9WGbY

## Background
* Capstone Case Study Project from (Google Data Analytics)
* **Objective**: How do annual members and casual riders use Cyclistic bikes differently?

## Data Collection
* **Link to data**: https://divvy-tripdata.s3.amazonaws.com/index.html

## Data Cleaning
After downloading the data,  I cleaned it for analysis. I made the following changes:

* Parsed datetime from *started_at and ended_at* columns:
  * *date_started, date_ended, time_started, time_ended, hour_started, hour_ended*  
* Columns created: 
    * Time spent riding bikes
    * Specified the day of the week for the ride
    * Determined if the ride was on a weekend
* Dropped duplicates and *NA* values from data

## EDA
I analysed the distributions of the data and the value counts of all the categorical variables to find if there were any trends. Below are some charts that I created from *Tableau* to display my findings:
![Avg Time Riden](https://user-images.githubusercontent.com/91089401/139720904-354106d0-1359-4f79-b6ca-d0182f7dbba9.png)
![Count of Rides by Member Type](https://user-images.githubusercontent.com/91089401/139720951-6db83f21-6afa-4247-b82b-81a2e1753e1d.png)
![Day of Week (Ride Count)](https://user-images.githubusercontent.com/91089401/139720972-40fdcb6c-e4be-43f7-a2e5-19a89a11159e.png)
![Hour Started (ride count) (2)](https://user-images.githubusercontent.com/91089401/139724625-b44b57de-fb04-4264-95fc-0470844c1ef0.png)

## Summary
