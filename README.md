# Cyclistic Bike Share Analysis 
cyclistic bike-share analysis case study is one of the capstone projects for the Google 

Data Analytics Professional Certificate which I completed in October 2023.



 Hi! I invite you to  Join me in  my project cyclistic bike-share analysis case study 
 
 its one of the capstone projects for the Google Data Analytics Professional Certificate which I completed in March 2024.


 the Google Data Analyst Capstone Project,which focuses on the Cyclistic Bike Share Case Study.
 
 In this project,we well analyze a public dataset provided by the course for a fictional company. 

Through this case study , we wIll  delve deep into data analysis, applying advanced techniques to derive meaningful conclusions.

We will explore how  the  Cyclistic Bike Share Case Study  intersect with  the principles of the Google Data 

Analyst Professional Certificate,enhancing our skills in interpreting and presenting data.

### Tools used for Analysis

**Microsoft Excel**: Used to get hold and understand the data we are dealing with and the parameters.

**RStudio** : For further analysis I used MSSQL.

**Powerbi**: Used this tool for Visualization.



### *BUSINES Task*
Cyclistic bike share company based in Chicago,reccognizes the importance of increasing the number of annual subscribers for its future success.To achieve this goal,this project aims

to analyze the differences in bike usage between casual riders and annual members and develop anew marketing strategy to convert casual riders in to annual subscribers.led by lily

Morenothe director of marketing, and supported by Cyclistic's markiting analytics team,this project will collect analyze and report data to guide the companys smarketing strategy.and to solve the question :-

How do annual members and casual riders use Cyclistic bikes differently?

Based on this, i will produce this case study  with the following deliverable.

***Tools***

**R**   *Clean , transform data  and  Data  Analysis*

**Powerbi**     *Visulaization and  Creating reports*


***Limitations***

I had to remove some columes i dont need in my analysis.

Ihad to delete rows with negative values in duration column. 

## *BUSINESS QUESTIONS*

1- How do casual and  member riders use Cyclistic Bike Share diferently.

2- Why would casual rides buy annual Cyclistic  memberships.

3-How can Cyclistic use digital media to influence casual riders to become members.

**For this project ,I will focouse on the first busnis question .**


## *Data Preparation*

 I Use Cyclistic’s historical trip data to analyze and identify trends. For the purposes of this case study, the datasets are appropriate and

will enable me to answer the business questions.

The data is located and stored in Amazon web server and is owned (first-party) by Cyclistic.


 **licensing, privacy, security, and accessibility** 
 
The data has been made available by Motivate International Inc under this license (https://www.divvybikes.com/data-license-agreement.)

The Raw data is downloaded and kept in my laptop and will not be shared by any means. 

Data is kept in csv ,these files were import to R Studio using read_csv function.

The 12 csv files were merged into a master data named *alltrips*
 
there  is no issues with bias or credibility in this data

**The data seems to fit the definition of ROCCC:-**

**Reliable**  the data is reliable as it is directly downloaded from the company’s servers.

**Original** the data is collected and owned by Cyclistic.

**Comprehensive** The data as stated earlier is a collection from 2013 till present. We have enough data to work with given the huge historical data.

**Current**  The data is regularly updated by the geotrackers in the bikes. So the data satisfies this property.

**Cited** -no citing needed as the data is collected and owned by the company Cyclistic itself.

The data is a collection of all years from 2013 to 2022, for our analysis we have chosen the most complete data wich is 2020 data  with 13 columns and 3527368  rows. 

## *Data Processing*


 Iused  RStudio Desktop  as the data processing tool.
 
 Following are the steps in cleaning and manipulating the data
 
- Data cleaning and formatting.
 
- Add some additional columns of data such as day ,month ,year  that provide additional  opportunities to aggregate the data

- Combined all 12 csv files into one file named *alltrips*

- Add acalculated field for length of ride*ride_lenght*  and week_day since the data did not have the tripduration coulum.

- There are some rides where tripduration shows up as negative,where Divvy took bikes 

   out of circulation for quality control reasons.we will want too delet these rides.

## *Data Analysis* 

Data has been cleaned and now we will move toward the analysis process

the analysis was performed using RStudio

 **CONDUCT DESCRIPTIVE ANALYSIS***  on *ride_length (all figures in seconds)

#### Summary of ride_length:_


![Screenshot (134)](https://github.com/nisrinfrh/google_project/assets/157531427/351f8af9-00f5-4bcc-b950-2b36526adc39)


#### Compare members and casual users:_

![Screenshot (135)](https://github.com/nisrinfrh/google_project/assets/157531427/dd3f856d-bb6c-4137-8e95-7dbe70a9a056)

  
#### See the average ride time by each day for members vs casual users:

![Screenshot (137)](https://github.com/nisrinfrh/google_project/assets/157531427/0522f602-1584-4a6d-bca9-a3ae9a6772ba)

##### Analyze ridership data by type and weekday

*calculates the number of rides and average duration*

![Screenshot (140)](https://github.com/nisrinfrh/google_project/assets/157531427/260c80c0-d095-4fb6-848f-e52a115660b4)


#### Key Insights for Presentation

For the presentation, I focus on the usage of the service by users according to their user category.


 *pie chart* showing the Ride type distribution of the users:- 


![Screenshot (147)](https://github.com/nisrinfrh/google_project/assets/157531427/c705c0cb-a86e-4bc5-98d3-8cbdeac6e167)


 Then i followed by introducing a new column called *start_hour* that extracts the hour of the day when the users use the service. 

This is an important insight because it could help the service providers know what time of day to do repairs or maintenance for their bikes 

with affecting their users negatively.

 *Line  chart*  to visulize most popular hour :-


![Screenshot (153)](https://github.com/nisrinfrh/google_project/assets/157531427/c2366f20-d8ea-4ba4-95f8-2582bbeba717)





Then  I looked at how each category of users uses the service per day of the week.   

 *Clustered  bar chart  which showed clearly the most popular days.* 

![Screenshot (149)](https://github.com/nisrinfrh/google_project/assets/157531427/205d517e-a706-4f5e-a68f-ce2527d6fc72)



### *Summary of Findings*

In the exploration,The analysis indicates that


**.   The bike share service is  quite popular with the users as it has 62% of them as subscribers.**

**Subscribers use Cyclistic more on weekdays and  mostly start their rides from 06:00 AM TO 09:00 Am and from 03:00 Pm  TO 05:00 Pm**

**which could indicate they use it to go to work in the morning and back home in the evening .**

**Casual riders tend to take more rides during weekends(Saturday and Sunday ).**

**and mostly start their rides after 12:00pm and after 07:00pm untill 09:00 pm.**

**Most active months for Casual and Member riders are from June to September.**

**. Streeter Dr & Grand Ave stations are the most used stations by Cyclistic riders.**

**- Casual riders ride for a longer time period with an average ride duration of 48.3 minutes.**

**Members have a shorter average ride duration of 15.8minutes.**


## *Recommendations*

**Marketing recommendations to convert casual riders into members:**

**Enhance user experience by improving bike availability and maintenance.**

**Start promotions at the top stations and focus interaction efforts during peak times of the day.**

 **Marketing effort targeting the top 10 most popular stations for riders could include posts on social media,**
 
**print media displayed on bikes or at locking stations, and contests starting from the most popular station.**
 
 **Offer promotional memberships during the summer months and weekends.**
 
 **An incentive system to encourage more trips within a membership framework**
 
**in order to receive discounts and partnership offers.**

**Implementing targeted social media ads towards individuals who have previously utilized bike-sharing services and** 

**have expressed  interest in travel, outdoor sports, parks, museums.**

*******************************************************

yclistic bike-share analysis case study is one of the capstone projects for the Google Data Analytics Professional Certificate which I completed in October 2023.

![image](https://github.com/nisrinfrh/google_project/assets/157531427/8644d2df-23ca-478f-96af-16aa145ccb6d)

BACKGROUND
This project is based on data curated for a fictional bike-sharing company called Cyclistic. The Company has more than 5,800 bicycles plus reclining bikes, hand tricycles and cargo bikes with over 600 docking stations to hold the bikes. The company has a flexible strategy that allows riders to unlock a bike from one station and return it to any other station anytime. Cyclistic is made up of two teams; a team of data analysts, the marketing analytics team and the executive team, the team that approves or disapproves recommended marketing programs.

Due to flexibility of its pricing plans, Cyclistic also has two types of riders;

Casual Riders: Customers who purchase single-ride or full day passes.

Cyclistic Members: Customers who purchase annual memberships.

DATA ANALYSIS PHASES
The following steps were used for this case study;

Ask → Prepare → Process → Analyze → Share → Actions

ASK
The ask phase was where I identified the business task and considered the demands of the key stakeholders.

Business Task: The aim of this case study is to understand how casual riders and annual members use Cyclistic bikes differently.

Insights: The insights obtained from this case study will be used by the Cyclistic marketing analytics team to design a new marketing strategy aimed at converting casual riders into annual members.

PREPARE
The datasets used for this case study to analyze and identify trends is Cyclistic’s historical trip data . Since the business task requires only 12 months of Cyclistic trip data, I downloaded the quarterly datasets (from the second quarter of 2019 to the first quarter of 2020) for my analysis .


Below are some important observation and task carried out at this phase;

The datasets are located in a document folder named Cyclistic Case Study.
Four CSV files of Divvy quarterly trips data are organized in the above folder with an appropriate naming convention classified by years and quarters.
There is no issue with bias or credibility in this data as it is Reliable, Original, Comprehensive, Current and well Cited.
The data is made available for the purpose of this case study by Motivate International Inc. under this license.
PROCESS
I used the following tools for this case study;

RStudio to clean, process and analyze the data.
Google Sheets for further statistical evaluation on the results from the analyzed data.
Tableau and R’s ggplot2 to create meaningful visualizations from the analyzed data
R Markdown to create an HTML documentation of the project.
GitHub and RPubs to create a repository for the codes used and create a public link to the visuals created respectively
These are the steps taken for the processing of the data:

I set my working directory to the folder that has the datasets.
I installed the required packages for the analysis of these datasets. The “tidyverse” package to analyze and clean the data, “Lubridate ‘’ for the date attributes and “ggplot2” for visualization.
I uploaded the four quarterly trips datasets which are in csv format to R using the ‘read_csv’ function and assigned them each to a more consistent name.

I checked for consistency in the column names of the datasets using the ‘colnames’ function and I discovered that the columns of datasets ‘q2_2019’, q3_2019, ‘q4_2019’ match perfectly but some of their columns do not match with ‘q1_2020’.
I renamed the columns to make them consistent with ‘q1_2020’ as it’s the most recent year and it is assumed it will be the table design for divvy going forward.
I made sure the data frames are in the same format, then I combined them using the ‘bind_rows’ function into one big data frame named “all_trips”.
I removed some irrelevant columns such as ‘lat’, ‘long’, ‘ birthyear’, and ‘gender’ as this data was dropped starting in 2020.
DATA CLEAN UP

One of the most important things to do before analyzing is to clean the data so as to avoid errors and bias. The first thing to do is to inspect the new table created (all_trips) and I used the following functions to do that;

colnames(all_trips) — to check the list of column names.
nrow(all_trips) — to see how many rows are in the data frame.
dim(all_trips) — to check dimensions of the data frame.
head(all_trips) / tail(all_trips) — to see the first or last few rows of the data frame.
str(all_trips) — to see a list of columns and data types of the data frame.
summary(all_trips) — to see the statistical summary of the data.
Observations & Solutions

Observation: In the “member_casual” column which is one of the most important columns to be analyzed, there are two names for members — “member” and “Subscriber” and same for casual riders — “casual” and “Customer”.

Solution: Consolidation of the column labels from four to two by replacing the “Subscriber” label with “member” and the “Customer” label with “casual”.


Observation: The data can only be aggregated at the ride-level which is not enough for our analysis

Solution: Addition of some columns to the data such as day, month, year to provide more opportunities to aggregate the data.

Observation: The q1_2020 data did not have the “tripduration” column which is a necessary field to determine the length of ride.

Solution: Addition of a calculated field “ride_length” to the entire data frame for consistency.


Observation: There are some rides where trip duration shows up as negative, including several hundred rides where bikes were taken out of circulation for Quality Control reasons.

Solution: Created a new version of the data frame, “all_trips_v2” since data is being removed, then I deleted the negative “ride_length” and the “HQ QR” rows which is a representation of when bikes were out of circulation.

ANALYZE
After cleaning and properly formatting the data, I did a descriptive analysis on it. The new and clean version of the data frame contained a total of 3,776,042 rows with the annual members having 76.7% of Cyclistic’s total customers while the casual members had only 23.3%.


Through the analysis performed, I discovered trends on how Cyclistic member and casual riders use bikes, I also gained the following insights;

The mid-point number and average ride length.
The longest and shortest ride.
The average ride time by each day of the week for members and casual users.
Ridership data (number of rides and average duration) by type and weekday.

I was also able to identify trends in the ‘number of rides by rider type’ and ‘average duration by rider type’ column graphs I created using the ggplot2 R package. These insights and discoveries gave me a better understanding of how annual members use Cyclistic bikes differently from casual riders.

SHARE
I created insightful visualizations of the data with Tableau Public and RStudio.


The Tableau and RStudio visualizations can be found here on Tableau Public Story and RPubs respectively.

I also created a markdown report which shows details on how the RStudio plots and dashboards were created, the link can be found here on RPubs Cyclistic Report.

ACTIONS
At this phase, I took some observations from the analyzed data which turned out to be important insights and I also pointed out a few recommendations which will all be summarized below.

OBSERVATIONS

Because they most likely ride for leisure, Casual Riders ride for a significant longer period than Annual Members.
Both Annual Members and Casual Riders are most active in the summer.
Annual Members take over 75% of the total rides in a year.
Casual Riders ride for a longer period during the winter season while Annual Members ride longer in the summer.
Annual Members ride more during weekdays as they mostly use it to commute to work while Casual Riders ride more on weekends.
Annual Members are most active in the morning around 7:00 AM to 9:00 AM and early evening around 4:00 PM to 6:00 PM while Casual Members are most active in the day around 12:00 PM to 6:00 PM.
RECOMMENDATIONS

Cyclistic should add new plans under the annual membership that will be favorable to the Casual Riders. For example, a weekend yearly plan can be introduced as most Casual Riders love to ride on weekends. This weekend plan would be cheaper than the full membership plan as riders who opt for this will be limited to riding on just weekends for a full calendar year.
An Annual day plan valid at noon only (12pm — 6pm) can be introduced as the Casual Riders prefer to ride during this time frame. To attract riders, this plan should be significantly cheaper than the full membership plan as well.
The company can also give exciting annual offers to Casual Riders. For example, for customers who love single-rides, they can create a family / friends plan that allows up to three users to share an annual membership.
There should be certain treats that should be limited to just the Annual Members. The company could restrict Casual Riders to ride for just a certain duration while Annual Members can ride for as long as they want. They could also restrict the Casual Riders who purchase single-rides to a certain amount of rides per day or per week. This can prompt Casual Riders who want to enjoy the full riding package to opt for annual membership.
As both users are most active during summer, there could be congestion and it is best to have both users under one accord for easy management. To achieve this, the company should introduce a seasonal pass exclusive to the summer period for Casual Riders only as Annual Members would always stand to enjoy the full package regardless of the season. Rather than paying extra for a seasonal pass in the summer, some Casual Riders would opt for the annual membership to enjoy the complete Cyclistic package.
Cyclistic should launch a campaign to introduce the new membership options and its benefits to the users with Casual Riders being the main audience.
ADDITIONAL SUGGESTION: For more important insights, data like “Unique Member ID” which will allow us to know the number of distinct riders and “Membership / Plan Prices” which will allow us to know the prices of existing plans ( one of the major factors riders would consider before choosing a plan) should have been provided.

IMPORTANT LINKS
Listed below are the links to all important details about this project from the codes used to the visualizations created and more.

GitHub - You can find all code files used to clean, analyze and visualize the data in this repository.

RPubs - Every visualization created using RStudio’s ggplot2 package including the HTML documentation file can be found here.

Tableau - The link to a well curated story for the visualizations created on Tableau.


This concludes the article, thank you for your time and I hope it would be of great help to you!










