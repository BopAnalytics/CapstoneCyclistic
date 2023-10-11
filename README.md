# Google Data Analytics Capstone Project: Cyclistic

## Introduction
This case study showcases the abilities I've acquired through the Google Data Analytics Professional Certificate Course. 
I intend to apply these skills to fulfill the responsibilities of a data analyst at the imaginary bike-share company Cyclistic.
Employing the structured data analysis approach, encompassing Ask, Prepare, Process, Analyze, Share, and Act stages, I aim to address the given business challenge comprehensively.
By leveraging data-driven insights, I will assist the company in making informed decisions.
### Scenario
Lily Moreno, the Marketing Director at Cyclistic, is convinced that the company's prosperity hinges on increasing annual memberships. 
Our objective is to discern the distinctions in bike usage patterns between casual riders and annual members.
These insights will serve as the foundation for devising a targeted marketing approach aimed at converting casual riders into loyal annual members.
However, our recommendations necessitate approval from Cyclistic's leadership. Hence, they must be substantiated with compelling data insights and polished data visualizations to make a persuasive case.

### About the Company
In 2016, Cyclistic introduced a highly successful bike-sharing service. Over time, the program has expanded to include a fleet of 5,824 bicycles, each equipped with geotracking and secure locking systems, available at 692 stations throughout Chicago.
Users have the freedom to unlock bikes from one station and return them to any other station within the network at their convenience.

Cyclistic stands out due to its flexible pricing options, including single-ride passes, full-day passes, and annual memberships.
Customers purchasing single-ride or full-day passes are categorized as casual riders, while those opting for annual memberships are recognized as Cyclistic members. 

According to Cyclistic’s financial analysts, annual members generate significantly higher profits compared to casual riders.
Moreno is optimistic about the possibility of converting casual riders into members, setting a clear objective: to develop marketing strategies focused on this conversion. To achieve this goal, Moreno and her team are keen on analyzing Cyclistic's historical bike trip data to discern underlying trends.

## Ask

### Business Task
Analyze Cyclistic's trip data from 2022 to identify variances in bike usage patterns between casual riders and annual members. The insights extracted from this analysis will guide the marketing team in shaping their campaign strategies.
### Stakeholders

Lily Moreno: Marketing Director in charge of creating promotional campaigns for the bike-share program, utilizing various channels such as email and social media.

Cyclistic Marketing Analytics Team: A group of data analysts tasked with gathering, analyzing, and presenting data to inform Cyclistic's marketing strategies.

Cyclistic Executive Team: A meticulous group of executives responsible for approving proposed marketing initiatives.

## Prepare
To initiate my preparation process, I begin by downloading the necessary data for analysis. Specifically, we will utilize the Cyclistic trip data from 2021. This data is acquired in 12 distinct .csv files, each corresponding to a different month of the year, and is organized into a designated folder. It's important to note that this data is provided by Motivate International Inc. and is subject to the terms outlined in this [license](https://ride.divvybikes.com/data-license-agreement).
## Process
### Data Cleaning
#### Excel
To begin the data cleaning process, I opened each .csv file in excel and did the following
* Verified and eliminated any duplicate entries.
* Established a new column called trip_duration_minutes by calculating the time difference between the started_at and ended_at columns.
* Duplicated two columns for started_at and ended_at, renamed to start_date, start_hour, end_date, and end_hour
* Formatted start_date and end_date columns to date format
* Formatted start_hour and end_hour columns by transforming to hours format
* Filtered out rides that were either shorter than 1 minute or longer than 24 hours by sorting the spreadsheet.

## Analyze
To begin the analysis phase, I wanted to reemphasize the business task ***How do casual riders and members use bikes differently?*** 

To answer this question, there were a few things that I identified that I could pull from the data. I created the following PivotTables to reflect:
* **Total # of trips per rider type**
* **Total # of trips per rider type per bike type**
* **Average ride length per rider type**
* **Total # of trips and average length of trip per rider type per month, day, and hour of day**
* **Most Popular Start and End Stations per rider type**

All Pivot tables and PowerQuery data can be found [here](https://github.com/BopAnalytics/CapstoneCyclistic/blob/main/PowerQuery)

After analyzing the Pivot tables, there are multiple facts to state:
* Riders peak at 5pm
* Casual riders have a longer average ride time for each type of bike
* The classic bike is used the most

Here is a look at the charts: [here](https://github.com/BopAnalytics/CapstoneCyclistic/commit/45e905b3958c6bf80ef7ae823056b49b9edf0658)

Here is a summary of the key differences found between Member and Casual Riders:
* Casual riders ride longer than regular members
* Casual members use the docked bike the most
* Members use the docked bike the least
* On average the trip druation is 25minutes for casual members using docked bike
* On average the trip duration is less than 5minutes for regular members using docked bikes
* Classic bike is the most popular regardless of member type

## Act
Based on my analysis, I'd recommend for management to encourage casual members to convert into regular members. Casual members are using the services more than regular members. 

1. Seasonal Membership: Summer (May to August), Fall (September to November), Winter (December to February), Spring (March to April)
2. 
