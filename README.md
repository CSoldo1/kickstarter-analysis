# kickstarter-analysis

## Overview

An up-and-coming playwrite asked me to help her plan a successful fundraisng campaign. By organizng, sorting, and analyzing data from thousands of Kickstarter campaigns  all over the world, I was able to identfy trends and give her valuable insight on the goal and timing of her campaign. 

## Analysis and Challenges

Two factors that can influence the success of a fundraising campaign are the date when the campaign was launched and the target goal, or the total money requested. I performed all analyses in Excel, and I utilized data from Kickstarter, a popular crowd-funding platform.


###Analyses
To determine the success of theater campaigns based on the date launched, I created a pivot table like the one pictured below:

![Pivot Table Example]()

I created a pivot table with data obtained from Kickstarter. From this, I created a pivot table and was able to filter campaigns based on outcome and launch date. I then looked to see whether or not a play-focused theater campaign was successful by contribution goal. This analysis was a little more involved because it required the use of the [Countifs] function in excel. I broke the contribution goals down into several categories from 1,000 to 50,000 in increments in 5,000. The code, like the one below

###Challeneges
=COUNTIFS(Kickstarter!F:F,"successful",Kickstarter!R:R,"plays",Kickstarter!D:D, ">=5000",Kickstarter!D:D,"<=9999")
Was more intricate than a pivot table, and it required manual entry of each number value. 



![Success Based on Category](https://github.com/CSoldo1/Photos/blob/main/Parent_Category_Outcomes_Graph.png)

The success of Kickstarter campaigns is highly variable. About half of all theater-based fundraising campaigns are successful.


![Outcomes Based on Launch Date](https://github.com/CSoldo1/Photos/blob/main/Outcomes_Based_on_Launch_Date.png)

The above figure shows the results of theater-based Kickstarter campaigns that launched througout the year. 
A higher proportion of theater campaigns are successful when they are launched in the summer, as opposed to other times of the year. 


A campaign's success was also determined by the fundraising goal. Successful campaigns had an average goal of $5,000 while failed campaigns had a goal of $10,000. 

Based on the analyses briefly outlined above, I would recommend that the playwrite begin her fundraising campaign in June, and she should try to limit her budget to $5,000. 


