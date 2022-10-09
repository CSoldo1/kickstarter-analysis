# kickstarter-analysis

## Overview

An up-and-coming playwrite asked me to help her plan a successful fundraisng campaign. By organizng, sorting, and analyzing data from thousands of Kickstarter campaigns  all over the world, I was able to identfy trends and give her valuable insight on the goal and timing of her campaign. 

## Analysis and Challenges

Two factors that can influence the success of a fundraising campaign are the date when the campaign was launched and the target goal, or the total money requested. I performed all analyses in Excel, and I utilized data from Kickstarter, a popular crowd-funding platform.


### Analyses
To determine the success of theater campaigns based on the date launched, I created a pivot table like the one pictured below:

![Pivot Table Example](https://github.com/CSoldo1/kickstarter-analysis/blob/main/Pivot_Table_Screenshot.PNG)

I then looked to see whether or not a play's contribution goal determined success. This analysis was a little more involved because it required the use of the "Countifs" function in excel. I categorized contribution goals from values less than $1,000 to greter then $50,000 in increments of 5,000. I used the following Excel code code:
=COUNTIFS(Kickstarter!F:F,"successful",Kickstarter!R:R,"plays",Kickstarter!D:D, ">=5000",Kickstarter!D:D,"<=9999")
 
### Challenges
I didn't have any challenges with the pivot table. Pivot tables are very user-friendly, and they make it easy to quickly analyze data. The "Countifs" function, on the other hand, was a little more complicated. Each cell could be populated with the same code, but the number values had to be entered manually. It was time-consuming and required a lot more focus, so that mistakes were not made. 

## Results

### Theater Outcomes Based On Launch Date

![Outcomes Based on Launch Date](https://github.com/CSoldo1/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

The date the campaign is launched effects the campaign's success. When launched in summer, theater campaigns are more successful than those launched in other times of the year. Interestingly, throughout the rest of the year, the proportion of successful campaigns relative to failed campaigns remains equal. Othere than December, there is not a time of the year where campaigns fail rather than succeed. 

####Quick Speculation
When campaigns are launched in December, they have the lowest success rate. More than likely, donors are cash-limited because of the Christmas holiday, and they are less likely to contribute to campaigns. 

### Success Based on Fundraising Goal

![Outcomes Based on Fundraising Goal](https://github.com/CSoldo1/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

The majority of campaigns were successful when the goal was less $1,000. Successful campaigns exceeded failed campaigns as long as the goal amount remained less than ~ 20,000. Furthermore, over 60% of play campaigns were successful if the goal was between $35,000 and $45,000. 

####Quick Speculation
If launch data truly determined campaign success, I would expect to see the data more linearly regressed. 

## Limitations and Future Analyses

Outcomes based on fundraising goal would be represented better with a stacked bar graph instead of a line graph. Bar graphs, especially stacked bar graphs, make it easier to visualize percentages. Furthermore, the Kickstarter data was missing campaign length data. I would assume that the length of a fundraising campaign would be more indicative of success. 


