# Cyclistic-Bike-Share-Analysis


**Case Study: How Does a Bike-Share Navigate Speedy Success?**

### Introduction

This is the first case study among the three case study I will do in my capstone project as the requirement for completion of the Google Data Analytics Certificate. As a junior data analyst in this case study I will analyse data of the fictional company called “Cyclistic” provided by the Course. To answer a business task; Cyclistic’s historical trip data is used to analyse and identify trends of the previous twelve (12) Months from January 2023 to December 2023.

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
Data used for this analysis is located at Bucket loading...[divvy-tripdata](https://divvy-tripdata.s3.amazonaws.com/index.html) <br>

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

**Part three: Process Phase** 

To analyse the data I used Oracle SQL and Excel
Data processing for analysis 
1.  I downloaded the data from January 2023 to December 2023
2.  Load twelve (12) months data
3.  Created a table named Bike Share data in Power BI
4. Imported the data from excel to  Bike Share data table
5.Drop all “NA” columns
6.Due to the large number of datasets, I choose to work with both Spreadsheet and Oracle SQL.
7.Document the cleaning process
a. Create a column called “ride_length.” Calculate the length of each ride by subtracting the column “started_at” from the column “ended_at”.
b. Add day_of_week, and Month. 
c. Separate the dates into month, day, year, and create a column called “day_of_week”.

1. Calculate the  ride_length for all
- Ensure I have columns for started_at and ended_at.
- Name of column ride_length and use the following formula:
- [ended_at] - [started_at]

2. Calculate Day of the Week
- Name of column day_of_week and use the following formula:
- Date.DayOfWeek([started_at], Day.Monday)
- This will create a column with values from 0 (Monday) to 6 (Sunday).

**Part Four: Analysis Phase**

Summary of the analysis
Data were formatted, organized and filtered monthly, and weekly and all data were filtered based on the objective of the first question to differentiate casual riders from members

The analysis shows that 
i. The mean length of the a ride is 17:56:58,
ii.The median length of the a ride is 00:10:02,
iii. The max length of the a ride is17:47:15
iv. Mode day of the week SATURDAY
v.  Number of rides for members 59.7% and casual riders 40.3%. Members rides more than casual riders
vi. August in Rider Type Member made up 8.05% of Total Rides.﻿﻿
vii. Average Total Rides was higher for Member (3,05,058.17) than Casual (1,71,598.25).﻿﻿
viii. Total Rides for Member and Casual diverged the most when the Month was October, when Member were 182971 higher than Casual.﻿﻿
ix. At 2945579, Electric_Bike had the highest Total Rides and was 3,662.54% higher than Docked_Bike, which had the lowest Total Rides at 78287.﻿﻿
X. Electric_Bike had the highest Total Rides at 2945579, followed by Classic_Bike at 2696011 and Docked_Bike at 78287.﻿﻿

**Part Five: Share**
Visualization was created from the exported query results Power BI
- Data visualization - [Power BI](https://app.powerbi.com/links/KQ76lsjF05?ctid=4b469bf3-7edf-4593-9b77-e4807953c730&pbi_source=linkShare)

![WhatsApp Image 2024-08-20 at 17 56 44_23aa9da2](https://github.com/user-attachments/assets/2270aa7a-f3c9-42cd-84a3-a68a5d4030ea)


Findings 
**Members** 
- Have many number of rides but few ride length
- Riders more on weekdays
- Use their bikes to commute to work
**Casual Riders**
- Have few riders but long ride length
- Rides more on weekend
- Use their bike for leisure

**Part Six: Act**
#### <ins>Recommendations</ins>
From the analysis above, we can design marketing strategies to convert casual riders to Cyclistic members. Here are my suggested approach:

- **Membership Personalisation** <br>
Provide a range of membership personalizations: yearly, monthly and daily. For example, $365/year, $45/month, $3/day. Users will be able to choose their membership type according to their own preferences. By introducing shorter-term membership plans with appropriate pricing, we can cater the needs of riders who might not need an annual membership.

- **Group Membership Discounts** <br>
Offerdiscounted plans for friends, students, and families can encourage collective memberships. Furthermore, it encourages users to cycle together and strengthen the bonds between people.

- **Membership Loyalty Points System** <br>
Implement a membership loyalty points system for users to collect points for each ride. Rewards such as membership discount will be given based on the number of points collected. This will encourage riders to use the service more frequently, driving engagement and loyalty. 

- **Member-Exclusive Events** <br>
Organize member-exclusive events such as group rides, urban exploration challenges, or themed cycling events. This approach not only encourages more rides from current members but also entices casual riders to join as members to participate in these unique experiences. 

- **Seasonal campaigns** <br>
Launch seasonal campaigns by offering limited-time discounts, special weekdays offers, or extended ride durations for members during these seasons to help in making the service more sustainable and manageable.

- **Social Media Engagement** <br>
Utilize digital media, including social media platforms, to engage with both casual riders and potential members. Share success stories, testimonials, and user-generated content from Cyclistic members who have benefited from the membership. Create visually appealing content showcasing the joy of cycling during different seasons and scenarios, enticing casual riders to become members. 


## 🔮 Conclusion
In short, this analysis provides valuable insights into the preferences and behaviors of Cyclistic members and casual riders. By tailoring strategies to the identified differences and preferences, Cyclistic can effectively convert casual riders into portential members.


