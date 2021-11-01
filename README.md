# DS Cyclist Project

## Codes and Resources Used
* **Python Version**: 3.8
* **Packages**: Pandas, Numpy, Matplotlib, OS
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
I analysed the distributions of the data and the value counts of all the categorical variables to find if there were any trends. Below you will find my some key findings when reviewing the data as well as some charts that I created from *Tableau* to display my findings:
**Bike Rides (by member type)**
  * Between the months of July and October are when the most bike rides take place. Some external factors that are correlated with these findings would be the season and wheather conditions. Members also are more consistant throughout the whole year. You can also conclude that the majority of members are locals and casual riders are most likely tourists or people looking for an activity to do.
**Avg Time of Bike Ride**
  * Taking a look at the average time spent riding, casual riders take longer bike rides than members. Something to consider is that casual riders may not be familiar with the routes as compared to members. Another reason for longer ride times would be using this service for a fun activity and/or for siteseeing.
**Day of the Week**
  * Members are riding more consistanly throughout the week as compared to casual riders. There is an increase in rides for casual riders starting Friday and the rides peak on Saturday. 
**Hour Started**
  * Both member and casual riders follow the same trend when it comes to the time of day. The majority of riders ride between the hours of 12PM to 9PM.

![Count of Rides by Member Type](https://user-images.githubusercontent.com/91089401/139720951-6db83f21-6afa-4247-b82b-81a2e1753e1d.png)
![Avg Time Riden](https://user-images.githubusercontent.com/91089401/139720904-354106d0-1359-4f79-b6ca-d0182f7dbba9.png)
![Day of Week (Ride Count)](https://user-images.githubusercontent.com/91089401/139720972-40fdcb6c-e4be-43f7-a2e5-19a89a11159e.png)
![Hour Started (ride count) (2)](https://user-images.githubusercontent.com/91089401/139724625-b44b57de-fb04-4264-95fc-0470844c1ef0.png)

## Findings/Trends
* Seasonal Trend
* Types of riders according to the member status
* Differences between Members and Casuals
| Members | Casuals |
|---|---|
| Residents of the area (work in the area or are students) | Tourists or people looking for an activity to do |
| Familiar with city Routes | Unfamiliar with city routes |
| Usage all year is more conistant (commuting) | Ride during favorable wheather/season (Summer/Fall) |
| Average ride time is consistant (18.2 minutes) | Average ride time is longer and inconsistant throughout the year (52.7 minutes) |
| Rides are conistant throughout the week with a slight decrease from Sunday to Monday | Prefer to ride on Friday and Saturday |

From the data, it is apparent that the amount of bike rides depend on timing (Season, day of week, hour of day). From "Count of Rides Member Type" chart you can see that between the months of July and October are when bike rides peak. Some external factors that may be correlated with these findings would be the season and wheather conditions. Also from this chart, members are more inclined to ride bikes all year as compared to the majority who Ride during the *"peak months"*. 

## Summary
The main differences between casual and member bike riders are: Day of the Week, Time of the Year (season), Time Spent Riding.
