# Cyclistic-Bike-Share-Analysis

First Case study research (April, 2023)

**Case Study: How Does a Bike-Share Navigate Speedy Success?**

### Introduction

This is the first case study among the three case study I will do in my capstone project as the requirement for completion of the Google Data Analytics Certificate. As a junior data analyst in this case study I will analyse data of the fictional company called “Cyclistic” provided by the Course. To answer a business task; Cyclistic’s historical trip data is used to analyse and identify trends of the previous twelve (12) Months from April 2022 to March 2023.

### About the company
**Cyclistic** a fictional company having casual riders and members
Casual Riders are Customers who purchase single-ride or full-day passes and Members are Customers who purchase annual memberships 
The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, the team wants to understand how casual riders and annual members use Cyclistic bikes differently.

- Cyclistic: A bike-share program that features more than 5,800 bicycles and 600 docking stations. Cyclistic sets itself apart by also offering reclining bikes, hand
  tricycles, and cargo bikes, making bike-share more inclusive to people with disabilities and riders who can’t use a standard two-wheeled bike. The majority of riders opt
  for traditional bikes; about 8% of riders use the assistive options. Cyclistic users are more likely to ride for leisure, but about 30% use them to commute to work each
  day.

Characters and teams
- Lily Moreno: The director of marketing and your manager.
- Cyclistic marketing analytics team
- Cyclistic executive team
  
Insights from this analysis will help the marketing team design a new marketing strategy to convert casual riders into annual members.

**Business Task**: How do annual members and casual riders use Cyclistic bikes differently?


**Part one: Ask Phase** 
General Objective of the analysis
The general objective of this analysis is to provide insight on the difference between casual riders and annual members that will help marketing department design a marketing strategy that will convert casual riders to annual members

Expected Results of the analysis
Insight from this analysis will enable my team to design new marketing strategy to convert casual riders into annual members so as to guarantee Cyclistic company’s future success that is expected to depends on maximizing the number of annual memberships
 
Key Stakeholders
- The director of marketing and my manager (Lily Moreno)
- Cyclistic executive team
- Cyclistic marketing analytics team
 
Business task to tackle: To identify the difference between casual riders and annual members

Part two: Prepare Phase
Data used for this analysis is located at Bucket loading...(divvy-tripdata.s3.amazonaws.com) 

The data used for this analysis data has been made available by Motivate International Inc. under the specified license at this link https://divvybikes.com/data-license-agreement

Data is from the fictional company Cyclistic's database It is a credible data for its first-hand data collected by the company and is updated on a monthly basis.
Data in obtained from this source will be only used for analysis purposes.

The data that are used for analysis are ROCCC which means they are Reliable, Original, Comprehensive, Current, Cited. This is because data is Reliable and is not biased, Its Original because it’s original public data, and its Comprehensive because not missing important information required for the analysis, it is also Current because its updated monthly and its Cited.


#### Data Exploration
I ran the queries for each column from left to right in order to determine the **data type** and to uncover any **missing values, outliers, inconsistencies, and errors** within the dataset. 

The data set consists of **13 variables**, as shown in the following: <br>

| **No.**|  **Variable**       |  **Description**                                        |
|--------|------------------   | --------------------------------------------------------|
| 1      | ride_id             | Unique ID assigned to each ride                         |
| 2      | rideable_type       | classic, docked, or electric                            |
| 3      | started_at          | Date and time at the start of trip                      |
| 4      | ended_at            | Date and time at the end of trip                        |
| 5      | start_station_name  | Name of the station where the ride journey started from |
| 6      | start_station_id    | ID of the station where the ride journey started from   |
| 7      | end_station_name    | Name of the station where the ride trip ended at        |
| 8      | end_station_id      | ID of the station where the ride trip ended at          |
| 9      | start_lat           | Latitude of starting station                            |
| 10     | start_lng           | Longitude of starting station                           |
| 11     | end_lat             | Latitude of ending station                              |
| 12     | end_lng             | Longitude of ending station                             |                            
| 13     | member_casual       | Type of membership of each rider                        |


This data is organized in monthly basis. This analysis is done using the data of the previous twelve (12) months from January 2023 to December 2023. File names are saved by the following format YYYYMM-divvy-tripdata such i.e (202301-divvy-tripdata). All files (Monthly) saved in Comma Delimited format(CSV) and in each sheet.

The data provided will be useful in answering the business questions.


