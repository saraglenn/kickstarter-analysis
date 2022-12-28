# Kickstarting with Excel

## Overview of Project
The data contained in the spreadsheet provides information related to the Kickstarter campaign goals and timelines per activity. It details the type and location of each campaign, as well as the monetary goal and pledge amounts. An analysis of this data outines trends related the success and failure of each. 
### Purpose
In order to have a comprehensive understanding of the impact and how to make recommendations moving forward, the data was analyzed to provide insight into how various campaigns (specifically for * *theater and plays* *) fared in connection to their **funding goals** and **launch date**.
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The analysis of outcomes based on launch date provides a count for all successful, failed, and canceled campaigns in each parent category per month. Creating a pivot table in which the x-axis contained the months and the y axis contained the count of campaigns allowed for filtering bewteen campaigns and years as needed. When filtered for the theater campaign the data reveals that there were 839 successful campaigns, 493 failed campaigns, and 37 canceled campaigns between the years 2009 and 2017. The month of May is identified as the most successful month overall, while the month of December yielded the fewest successful campaigns. Interestingly, the month of May also yielded the most failed campaigns showing that this was the most active month overall in terms of monthly totals. 

Analyzing the data using the line chart provides a visual for the trends of successful, failed, and canceled theater campaigns over the course of nine years. With a bit of variation, the sucessful campaings trend upward through the month of May, afterwhich they begin to trend downward for the remaining months of the year. 


### Analysis of Outcomes Based on Goals

The analysis of outcomes based on goals provides a count for all successful, failed, and canceled play campaigns with respect to their funding goals. The total number of projects was then calculated using a =sum formula (ex. =SUM(B2:C2)), as well as the percentage of success and failure rate for each funding goal range by creating a formula that divided the number of campaigns in each category by the total projects (ex. =(B2/E2)). At a glance, it is clear that the most successful campaigns were those that in which the funding goal was <$5000.  The higher the campaign funding goal, the higher the rate of failure. 

### Challenges and Difficulties Encountered

One of the challenges I ran into while analyzing this data was utilizing the countifs formula for the outcomes based on goals. I was initially trying to create a formula for each column one at a time (number success, number failed, etc); learning that filtering the data in the excel spreadsheet only changes what you are able to view (not what you analyze) was useful. Eventually, I was able to figure out how to write the formulas to incude the filter of # successful, # failed, and # canceled based on plays and the goal ranges. Starting with the formula =COUNTIFS(Kickstarter!D:D, "<1000", Kickstarter!F:F, "successful", Kickstarter!Q:Q, "plays") provided all filters needed, thus only requiring editing based on the goal range and then the number "failed". 

Another challenge of my own is in identifying the opportunities and pain points once the analysis is complete. I tend to think about what data is missing and how that might impact the results, rather than simply analyzing the data I do have while acknowledging it's limitations.  

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

One conclusion that can be drawn from the Outcomes based on Launch Date is that the month of May significantly yields more successful campaigns. This is important information for Louise moving forward as she embarks on camapaign planning and target setting for the next several year. With this information, she may decide to focus more effort in launching campaigns during this time as opposed to say, the month of December, which yielded the fewest successful campaigns. We can make this assumption using the data provided because it is longitudinal and spans across nine years. In other words, it's not a single snapshot of time therefor we see the continous trend of success over time. She will now potentially be able to use this information to perform a diagnostic analysis of why the month of May yields more successful results. 

Another interesting trend can be found when looking at the trajectory of successful and failed campaigns together. In conclusion, when looking at the data from Jan - Dec, as the number of successful campaigns grew so did the number of failed campaigns. The successful and failed campaigns both peaked around the same time (*middle of the year*) and then as the successful campaign numbers began to decrease in the second half of the year so did the failed campaigns, generally speaking. 

- What can you conclude about the Outcomes based on Goals?

In analyzing the outcomes of campaigns for plays in relationship to their funding goals there is a statistically singifcant difference in the success of those in which the goal was $0-$999 and $1000-$4999, with a success rate of 76% and 73%, respectively. This is an important data point for Louise as it gives her information about attainable and likely successful funding goals in the future. The higher the campaign goals, the more more likely it is for a failed campaign. No campaigns were canceled, regardless of funding goal.   

- What are some limitations of this dataset?

We are limited in the depth of information we can analyze based on the given data. For example, it would be interesting to know who the backers were for each campaign so that we could pinpoint where funding is coming from and potentially use this knowledge to target funders. However, based on the data presented, access to this information is not provided. 

- What are some other possible tables and/or graphs that we could create?

The data points we analyzed for outcomes based on goals and outcomes by launch date are a fraction of the whole picture. Analyzing these points provides information specifically for those two categories, but does not provide a full picture of the campaign strategies and goals. Pulling this data and analyzing it for all parent categories would provide additional information about ideal campaign timing specific to the type of campaign. Additionally, further analyzing the outcomes based on goals by breaking down the parent category would allow for a deeper analysis of successful which campaigns were most successful based on the funding goal. 

Another interesting table to pull would be to analyze the breakdown of successful campaigns based on country. This would allow us to look at any trends based on population and location which could in turn support targeted marketing. 
