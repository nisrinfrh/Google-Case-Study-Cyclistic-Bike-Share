# Cyclistic Bike Share Analysis 
Cyclistic bike-share analysis case study is one of the capstone projects for the Google 

Data Analytics Professional Certificate which I completed in March2024.

## Introduction
This project is based on data curated for a fictional bike-sharing company called Cyclistic. 

The Company has more than 5,800 bicycles plus reclining bikes, hand tricycles and cargo bikes 

With over 600 docking stations to hold the bikes. The company has a flexible strategy that allows

Riders to unlock a bike from one station and return it to any other station anytime.


 Cyclistic  has two types of riders :-

Casual Riders: Customers who purchase single-ride or full day passes.

Members Riders : Customers who purchase annual memberships.


** steps used for this case study**

***Ask → Prepare → Process → Analyze → Share → Actions***

## ASK

These questions identified the business task and considered the demands of the key stakeholders:

1-How do annual members and casual riders use Cyclistic bikes differently?

2-Why would casual riders buy Cyclistic annual memberships?

3-How can Cyclistic use digital media to influence casual riders to become members?

In our project, we will focus on the first question.

#### *BUSINES Task*

Analyze the differences in bike usage Patterns between casual riders and annual members, and develop a new 

Marketing strategy  aimed at  converting  casual riders in to annual subscribers.

led by lily Morenothe the Director of Marketing, and supported by Cyclistic's Markiting analytics team.

This project will collect analyze and report data to  inform the company's strategic marketing decisions. .


### Tools Used for Analysis

I utilized the following tools for this case study:

**RStudio**: to clean, process, and analyze the data.

**PowerBI**: to generate insightful visualizations from the analyzed data.

**GitHub**: to establish a repository for the utilized code and to create public links for the visuals produced, respectively.

These were the steps taken for data processing:

**Limitations**

I had to remove some columns that were unnecessary for my analysis.

I had to delete rows with negative values in the duration column.







## *Data Preparation*

## *PREPARE*

I Use Cyclistic’s historical trip data to analyze and identify trends. 

I chose 2020 data  with 13 columns and 3527368  rows. 

 I create a document folder named Bike_share.

12 CSV files of Divvy quarterly trips data are  located , stored and  organized in the above folder .

 *licensing, privacy, security, and accessibility*
 
The data has been made available by Motivate International Inc under this license (https://www.divvybikes.com/data-license-agreement.)


#######  The 12 csv files were merged into a master data named *alltrips*#######
 
there  is no issues with bias or credibility in this data

**The data seems to fit the definition of ROCCC:-**

**Reliable**  the data is reliable as it is directly downloaded from the company’s servers.

**Original** the data is collected and owned by Cyclistic.

**Comprehensive** The data as stated earlier is a collection from 2013 till present. We have enough data to work with given the huge historical data.

**Current**  The data is regularly updated by the geotrackers in the bikes. So the data satisfies this property.

**Cited** -no citing needed as the data is collected and owned by the company Cyclistic itself.
 
 For the purposes of this case study, the datasets are appropriate and

  will enable me to answer the business questions.

## *Data Processing*

## **PROCESS**

 Iused  RStudio Desktop  as the data processing tool.

I installed the required packages for the analysis of these datasets. 

The “tidyverse” package to analyze and clean the data.

“Lubridate ‘’ for the date attributes and “dplyer” for cleaning .

I uploaded trips datasets which are in 12 csv format to R using the ‘read_csv’ function.

And assigned them each to a more consistent name.
 
 Following are the steps in cleaning and manipulating the data
 
- Add  additional columns of data such as day ,month and year that provide additional  opportunities to aggregate the data

- Combined all 12 csv files into one file named *alltrips*

- Add acalculated field for length of ride*ride_lenght*  and week_day since the data did not have the tripduration coulum.

-  I deleted the negative “ride_length” and the “HQ QR” rows which is a representation of when bikes were out of circulation.

  Since data is being removed, i reated a new version of the data frame “alltrips2”

## *ANALYZE*

*The analysis was performed using RStudio*

After cleaning and properly formatting the data, I did a descriptive analysis on it. 

The new and clean version of the data frame contained a total of 3,776,042 rows with the annual members having 

76.7% of Cyclistic’s total customers while the casual members had only 23.3%.

 *CONDUCT DESCRIPTIVE ANALYSIS* on *ride_length (all figures in seconds)

#### Summary of ride_length:_


![Screenshot (134)](https://github.com/nisrinfrh/google_project/assets/157531427/351f8af9-00f5-4bcc-b950-2b36526adc39)


#### Compare Members and Casual users:_

![Screenshot (135)](https://github.com/nisrinfrh/google_project/assets/157531427/dd3f856d-bb6c-4137-8e95-7dbe70a9a056)

  
#### See the average ride time by each day for Members vs Casual users:

![Screenshot (137)](https://github.com/nisrinfrh/google_project/assets/157531427/0522f602-1584-4a6d-bca9-a3ae9a6772ba)

##### Analyze ridership data by Type and Weekday

*calculates the number of rides and average duration*

![Screenshot (140)](https://github.com/nisrinfrh/google_project/assets/157531427/260c80c0-d095-4fb6-848f-e52a115660b4)

## *SHARE*
I created insightful visualizations of the data with PowerBi.

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

ACTIONS
At this phase, I took some observations from the analyzed data which turned out to be important insights and I also pointed out a few recommendations which will all be summarized below.

OBSERVATIONS

Because they most likely ride for leisure, Casual Riders ride for a significant longer period than Annual Members.
.
Annual Members take over 75% of the total rides in a year.
Casual Riders ride for a longer period during the winter season while Annual Members ride longer in the summer.
Annual Members ride more during weekdays as they mostly use it to commute to work while Casual Riders ride more on weekends.


In the exploration,The analysis indicates that


**The bike share service is  quite popular with the users as it has 62% of them as Annual Members .**

**Annual Members ride more during weekdays and  most active in the morning around 6:00 AM to 9:00 AM and early evening around 3:00 PM to 5:00 PM**

**which could indicate they use it to go to work in the morning and back home in the evening .**

**Casual riders tend to take more rides during weekends(Saturday and Sunday ).**

**and mostly start their rides after 12:00pm and after 07:00pm untill 09:00 pm.**

**Both Annual Members and Casual Riders are most active in the summer**

**Most active months for Casual and Member riders are from June to September.**

**. Streeter Dr & Grand Ave stations are the most used stations by Cyclistic riders.**

**- Casual riders ride for a longer time period with an average ride duration of 48.3 minutes.**

**Members have a shorter average ride duration of 15.8 minutes.**


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










