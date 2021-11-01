# DS Cyclist Project
* Capstone Case Study Project from (Google Data Analytics)

## Codes and Resources Used
* **Python Version**: 3.8
* **Packages**: Pandas, Numpy, Matplotlib, OS
* **Visual Tools**: Tableau
* **License for data**: https://www.divvybikes.com/data-license-agreement
* **Link to combining multiple CSV files**: https://www.youtube.com/watch?v=dcQs8k9WGbY

## Background
In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that
are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and
returned to any other station in the system anytime.

* **Objective**: How do annual members and casual riders use Cyclistic bikes differently?

## Findings/Trends Overview
* Seasonal Trend
* Ridable Type Preference
* Average Ride Times
* Day of Week
* Hour Started

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
I analyzed the distributions of the data and the value counts of all the categorical variables to find if there were any trends. Below you will find some key findings (with explanation/ thought process) when reviewing the data as well as some charts that I created from *Tableau* to display my findings:

**Seasonal Trend**
  * Between the months of July and October are when the most bike rides take place. Some external factors that are correlated with these findings would be the season and weather  conditions. Members are more consistent throughout the whole year with a slight decrease during the Winter. Although there is a decrease during the winter, there are more members riding during the off season as compared to casuals who mostly ride during the warmer seasons (summer/fall).
![Count of Rides by Member Type](https://user-images.githubusercontent.com/91089401/139720951-6db83f21-6afa-4247-b82b-81a2e1753e1d.png)

**Rideable Type Preference**
 * Docked Bikes were favorable up until the introduction of Classic Bikes, which was implemented in December 2020. With classic Bikes being the favorite, you also see a huge decrease in the usage of docked bikes. 
![Ridable Type](https://user-images.githubusercontent.com/91089401/139749687-ab099e26-ac1d-4272-9101-d311f5d28885.png)

**Avg Time Riden**
  * Taking a look at the average time spent riding, casual riders with an average time of 52.7 minutes take longer bike rides than members with an average ride time of 18.2 minutes. Member ride times are more consistent throughout the year staying close to its average ride time, as compared to casuals which are more inconsistent. Something to consider is that casual riders may not be familiar with the routes or they may be using this service as a fun activity and/or for sightseeing.
![Avg Time Riden](https://user-images.githubusercontent.com/91089401/139720904-354106d0-1359-4f79-b6ca-d0182f7dbba9.png)

**Day of the Week**
  * Members are riding more consistently throughout the week as compared to casual riders. There is an increase in rides for casual riders starting Friday and the rides peak on Saturday. Although the drop in riders for both casuals and members starts to decline on Sunday, the drop for casuals is much larger. There is a bigger drop in ride counts for Casuals starting from Sunday up until Thursday and will see exponential growth during the weekends (Friday/Saturday).
![Day of Week (Ride Count)](https://user-images.githubusercontent.com/91089401/139720972-40fdcb6c-e4be-43f7-a2e5-19a89a11159e.png)

**Hour Started**
  * Both member and casual riders follow the same trend when it comes to the time of day. The majority of riders ride between the hours of 12PM to 9PM.
![Hour Started (ride count) (2)](https://user-images.githubusercontent.com/91089401/139724625-b44b57de-fb04-4264-95fc-0470844c1ef0.png)

**Differences between Members and Casuals**

| **Members** | **Casuals** |
|---|---|
| **Residents** of the area (work in the area or are students) | **Tourists** or people looking for an activity to do |
| Familiar with city **Routes** | Unfamiliar with city **routes** |
| Usage all year is more consistent (commuting) | Ride during favorable weather/season (Summer/Fall) |
| Average ride time is consistent | Average ride time is longer and inconsistent throughout the year |
| Rides are consistent throughout the week with a slight decrease from Sunday to Monday | Prefer to ride on Friday and Saturday |

## Recommendations
* Focus on increasing the number of classic bikes
* Look towards getting rid of docked bikes and transition to classic/electric bikes only 
* Implement a tool that guides you through the quickest/effective routes

## Further Analysis
* Dive more in depth on the location to find where the majority of rides take place and end.
  * Provides more insight on which places are hotspots for this service as well as building more stations where it is needed.



