# Cyclistic Bike Share Analysis 

 Hi, Join me in the Google Data Analyst Capstone Project, focusing on the Cyclistic Bike Share Case Study.
 
 In this case study I will be analyzing a public dataset for a fictional company provided by the course.

In this case study , we  dive deep into data analysis, applying advanced techniques to extract meaningful conclusions.

Explore the intersections of the Cyclistic Bike Share Case Study and the principles of the Google Data Analyst Professional Certificate

solidifying  our skills in interpreting and presenting data.


### *BUSINES Task*
Cyclistic bike share company based in Chicago,reccognizes the importance of increasing the number of annual subscribers for its future success.To achieve this goal,this project aims

to analyze the differences in bike usage between casual riders and annual members and develop anew marketing strategy to convert casual riders in to annual subscribers.led by lily

Morenothe director of marketing, and supported by Cyclistic's markiting analytics team,this project will collect analyze and report data to guide the companys smarketing strategy.and to solve the question :-

How do annual members and casual riders use Cyclistic bikes differently?

Based on this, i will produce this case study  with the following deliverable.

***Tools***
*R  Clean and transform data  and  Data  Analysis*

*Powerbi  Visulaization and  Creating reports*

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

I use primary source data downloaded from Cyclistic's internal data.

 **licensing, privacy, security, and accessibility** 
 
The data has been made available by Motivate International Inc. under this license (https://www.divvybikes.com/data-license-agreement.)

  The Raw data is downloaded and kept in my laptop and will not be shared by any means. 

 Data is kept in csv ,these files were import to R Studio using read_csv function .The 12 csv files were merged into a master Data Named
 
 *all_trips*
 
**there  is no issues with bias or credibility in this data**

**The data seems to fit the definition of ROCCC:-**

**Reliable**Yes, the data is reliable as it is directly downloaded from the company’s servers.

**Original**Yes, the data is collected and owned by Cyclistic.

**Comprehensive** -The data as stated earlier is a collection from 2013 till present. We have enough data to work with given the huge historical data.

**Current**- The data is regularly updated by the geotrackers in the bikes. So the data satisfies this property.

**Cited** -no citing needed as the data is collected and owned by the companyCyclistic itself.

The data is a collection of all years from 2013 to 2022, for our analysis we have chosen the most complete data wich is 2020 data  with 13 columns and 3527368  rows. 

## *Data Processing*

 Iused  RStudio Desktop  as the data processing tool. the master data was fed into the software as a data sourse 
 **.transfomed, andling missing values, Data cleaning and formatting.**
 
**.add some additional columns of data such as day ,month ,year  that provide additional  opportunities to aggregate the data**

**.Combined all 12 csv files into one file named *all_trips***

**.add acalculated field for length of ride*ride_lenght*  and week_day since the data did not have the tripduration coulum.**

**.There are some rides where tripduration shows up as negative,where Divvy took bikes 
out of circulation for quality control reasons.we will want too delet these rides.**

## *Data Analysis* 

Data has been cleaned and now we will move toward the analysis process

the analysis was performed using R code 

 **CONDUCT DESCRIPTIVE ANALYSIS  on *ride_length (all figures in seconds)***

##### Summary of ride_length:_

![Screenshot (134)](https://github.com/nisrinfrh/google_project/assets/157531427/351f8af9-00f5-4bcc-b950-2b36526adc39)

##### Compare members and casual users:_

![Screenshot (135)](https://github.com/nisrinfrh/google_project/assets/157531427/dd3f856d-bb6c-4137-8e95-7dbe70a9a056)
  
#### See the average ride time by each day for members vs casual users:

![Screenshot (137)](https://github.com/nisrinfrh/google_project/assets/157531427/0522f602-1584-4a6d-bca9-a3ae9a6772ba)

##### Analyze ridership data by type and weekday
*#calculates the number of rides and average duration*

![Screenshot (140)](https://github.com/nisrinfrh/google_project/assets/157531427/260c80c0-d095-4fb6-848f-e52a115660b4)


### Key Insights for Presentation
For the presentation, I focus on the usage of the service by users according to their user category . Istart by introducing a new column called *start_hour* that extracts the hour of the day when the users use the service. This is an important insight because it could help the service providers know what time of day to do repairs or maintenance for their bikes with affecting their users negatively. plotted it on a *Line  chart*  to visulize most popular hour :-

![Screenshot (148)](https://github.com/nisrinfrh/google_project/assets/157531427/f026cd18-f887-45bf-96f9-90c3e34400c6)

###Then i followed by plotting a *pie chart* showing the Ride type distribution of the users:- 

![Screenshot (147)](https://github.com/nisrinfrh/google_project/assets/157531427/c705c0cb-a86e-4bc5-98d3-8cbdeac6e167)


###Afterwards, I looked at how each category of users uses the service per day of the week and plotted it on a *Clustered  bar chart* which showed clearly the most popular days. 

![Screenshot (143)](https://github.com/nisrinfrh/google_project/assets/157531427/aa57b87f-169b-417a-8058-c92ea3baf545)


You can view more insights by downloading and opening this file in your browse
Project Overview

### Summary of Findings

In the exploration,The analysis indicates that


**.The bike share service is  quite popular with the users as it has 62% of them as subscribers.**

**.Subscribers use Cyclistic more on weekdays and  mostly start their rides from 06:00 AM TO 09:00 Am and from 03:00 Pm  TO 05:00 Pm**

**which could indicate they use it to go to work in the morning and back home in the evening  , while for Casual**

**The day with the most rides is Saturday and Sunday ,and mostly start their rides after 12:00pm and after 07:00pm untill 09:00 pm.**

**.The longest ride is  minutes which is about 23 hours and the shortest ride is**

**. cll station are the most used station by Cyclistic riders.**

**.The Average of tripduration for Casual is 48.3 Minutes, and  for ember is 15.81 Minutes.**




Step 2: Prepare

How is the data organized? 


###################################################3

How did you verify the data’s integrity? The identification of missing values ( start/end station names and their ID’s) are all identifiable given the coordinates which can be rounded off the station’s name and ID can be recovered.



Step 3 & 4: Process & Analyse
Following are the steps in cleaning and manipulating the data

Firstly, we will use excel to clean and transform the data.So, these were the steps used: + Join the data to make one data frame + save it in a separate spreadsheet. + add two columns (i.e. ride_length ) and calculate its values. + add filters to the headers and filter end_lat with empty cells. Select all the visible cells and delete them. + delete rows with negative values in ride length. + find answers to the following values using formulas in excel. Here are the results.

mode_weekday 7
mean_ride_length 00:15:37
max_ride_length 23:47:38
members_average_ride_length 00:13:21
casual_average_ride_length 00:25:04

no_of_rides_on_Sunday 17078
no_of_rides_on_Monday 17757 no_of_rides_on_Tuesday 19154 no_of_rides_on_Wednesday 20987 no_of_rides_on_Thursday 21354 no_of_rides_on_Friday 23519 no_of_rides_on_Saturday 26289

most_rides_week 26289 Saturday least_rides_week 17078 Sunday

Start loading the file in R studio for further visualization and analysis.
Key takeaways
Average ride length by customer type and day of the week: Length of the rides of Causal riders is 40% more than that of the Members.

Biketype used by each type of subcribers and casual riders Clasic bikes are No#1 in demand and electric bikes. Demand for docked bikes is very insignificant compared to the two.
####draaaaffft 



Total rides analysis by weekday Causal riders use the service for leisure and members use it to mainly commute.
