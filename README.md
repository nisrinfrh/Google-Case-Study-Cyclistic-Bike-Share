# Cyclistic Bike Share Analysis 

 Hi! I invite you to  Join me in the Google Data Analyst Capstone Project,which focuses on the Cyclistic Bike Share Case Study.
 
 In this project,we well analyze a public dataset provided by the course for a fictional company. 

Through this case study , we wIll  delve deep into data analysis, applying advanced techniques to derive meaningful conclusions.

We will explore how  the  Cyclistic Bike Share Case Study  intersect with  the principles of the Google Data 

Analyst Professional Certificate,enhancing our skills in interpreting and presenting data.


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



*You can view more insights by downloading and opening this file in your browse Project Overview*


### *Summary of Findings*

In the exploration,The analysis indicates that


**.   The bike share service is  quite popular with the users as it has 62% of them as subscribers.**

**Subscribers use Cyclistic more on weekdays and  mostly start their rides from 06:00 AM TO 09:00 Am and from 03:00 Pm  TO 05:00 Pm**

**which could indicate they use it to go to work in the morning and back home in the evening .**

**Casual riders tend to take more rides during weekends(Saturday and Sunday ).**

**and mostly start their rides after 12:00pm and after 07:00pm untill 09:00 pm.**

**Most active months for Casual and Member riders are from June to September.**

**. Streeter Dr & Grand Ave station is the most used station by Cyclistic riders.**

**- Casual riders ride for a longer time period with an average ride duration of 48.3 minutes.**

**Members have a shorter average ride duration of 15.8minutes.**
just about season

## *Recommendations*

**Marketing recommendations to convert casual riders into members:**

 **Marketing effort targeting the top 10 most popular stations for riders could include posts on social media,**
 
**print media displayed on bikes or at locking stations, and contests starting from the most popular station.**
 
 **Offer promotional memberships during the summer months and weekends.**
 
 **An incentive system to encourage more trips within a membership framework**
 
**in order to receive discounts and partnership offers.**

**Implementing targeted social media ads towards individuals who have previously utilized bike-sharing services and** 

**have expressed  interest in travel, outdoor sports, parks, museums.**
*******************************************************

Introduction :

The cyclist started a successful Bike-sharing program: the cyclist customers are divided in two categories ;

Customers who purchase single ride or full-day rides referred to as Casual Riders
Customers who purchase annual membership are considered Cyclistic members
The dataset consists of the past 12 months data from the December 2020 to November 2021.

You can download the dataset from this link

Conflict:

The finance analysts concluded that the annual members are much more profitable than the Casual riders and the Manager, believed that maximizing the number of annual member will be key to future growth. She also believed that rather than creating a marketing campaign that targets all new-customers, there is a very good chance to convert Casual riders into members.

Tools used for Analysis

Microsoft Excel: Used to get hold and understand the data we are dealing with and the parameters.
Microsoft SQL Server : For further analysis I used MSSQL.
Powerbi: Used this tool for Visualization.
Data Preparation

Here we will process data cleaning and ensuring that the correct relevant, complete and free of error and outlier when performing analysis:

Explore and observe data
Check for and treat missing values
Transform data-format types types
Created a column named “total minutes” which calculates the time length of the rides
Created another column named “weekday” to calculate the day of the week
Removed columns where the ride-id length column isn't equal to 16 characters.
Further analysis took place in MSSQL Server.

Check out my Sql code 







