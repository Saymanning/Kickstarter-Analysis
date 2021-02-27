# Kickstarting with Excel
---
## Overview of Project
##### The client, Louise, is an enterprising playwright. In a previous project, analysis was performed on a dataset of over 4000 Kickstarter crowdfunding campaigns to help Louise plan a successful crowdfunding campaign of her own for her play, Fever. The results of this analysis provided Louise with insights and information that enabled her play quickly come close to its fundraising goal of $12,000. She is now interested in finding out how successful or unsuccessful different campaigns were by comparing their launch dates and their funding goals. Specifically, are there distinct reasons that make one campaign more successful than another in relation to their launch dates and fundraising goals?
---
### Purpose
##### The purpose of this project was to glean more specific details from the Kickstarter dataset to help Louise’s campaign be a successful one and to provide insights with date and charts to help her visualize the findings of campaign outcomes based on their launch dates and funding goals.
---
---
## Analysis and Challenges
##### In order to dig deeper into the details regarding campaign outcomes based on launch data and funding goal, the first step in the analysis was to find out the launch dates of all theater projects. This was achieved by creating a new column in the Kickstarter data sheet called, “Years”. The YEAR()function was used to extract the year from the “Date Created Conversion” column.
---
##### A pivot table was created and placed in a new sheet labeled, “Theater Outcomes by Launch Date”. The pivot table was sorted by “Parent Category” and then by “Years”.
---
##### Next the pivot table was filtered by the column labels to show only “successful”,” failed” and “canceled” campaigns.
---
##### To show only the data for theater projects, the “Parent Category” was filtered to “theater”. The outcomes were then sorted in descending order so “successful” shows first, since that is important information to Louise.
---
##### To help Louise visualize the theater outcomes based on their launch date.
##### A line chart was created from the pivot table showing the number of successful, failed and canceled projects by month.
---
##### The second part of the analysis was to gather the data needed to visualize campaign outcomes based on funding goal amount.
---
##### A new sheet labeled “Outcomes Based on Goals” was created in the Kickstarter data sheet. The following columns were created in the new sheet:
##### Goal, Number successful, number failed, number canceled, Total Projects, Percentage successful, Percentage failed and Percentage canceled.
##### The dollar-amount ranges listed below were added to the Goal column.
---
##### Less than 1000
##### 1000 to 4999
##### 5000 to 9999
##### 10000 to 14999
##### 15000 to 19999
##### 20000 to 24999
##### 25000 to 29999
##### 30000 to 34999
##### 35000 to 39999
##### 40000 to 44999
##### 45000 to 49999
##### Greater than 50000
---
##### In order to find and populate the number of successful, failed and canceled campaigns, the COUNTIFS() function was used by filtering on the columns “outcome” and “goal” on the Kickstarter sheet using the ranges above. Then filtered the “Subcategory” column by plays.
---
##### To calculate the percentage of successful, failed and canceled projects, first the SUM() function was used to populate “Total Projects” column with the total number of successful, failed and canceled projects. Then the percentage was calculated for each row.
---
##### Using the data compiled above, an Outcomes_vs_Goals line chart was created to illustrate the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed or canceled campaigns on the y-axis.
---
---
### Analysis of Outcomes Based on Launch Date
---
##### According to the pivot chart seen here: Outcomes based on Launch date, the month with the highest number of successful campaigns is May, closely followed by June. This trend is easily visualized by the line chart here:
##### The line chart also shows that the number of failed campaigns is consistent January to October. The months with the lowest number of successful campaign launches are November, December and January. December had almost the same number of successful and failed campaigns. Successful campaigns begin to trend up slightly in February, however the chart indicates the rate of successful campaigns launched doesn’t really begin to rise significantly until April.
---
---
---
### Analysis of Outcomes Based on Goals
---
##### The data in the Outcomes based on Goals sheet tells us that campaigns with a goal amount of less than $1000 had the highest percentage of success with 76% being successful. Campaigns with a goal amount of $1000 to $4999 was a close second with 73% being successful. However, there were almost 3 times as many campaigns with a goal in the $1000 to $4999 range. The percentage of failed campaigns in the two goal ranges was close as well. It can be concluded that campaigns with a goal in the range of less than $1000 to $4999 are the most successful. Only about half the campaigns with goal ranges from $5000 to $14000 were successful. Louise’s campaign performed well considering she almost reached her goal of $12,000 in a short amount of time and her goal was nearly twice the amount of the average successful campaign goal.
---
##### The campaigns with the highest goal amounts of $45000 and above performed poorly with the lowest percentage of success. The goal amounts are 4 to 5 Campaigns with goals in the range of $45000 and above performed poorly with the lowest percentage of success. However, these goals were almost 3 times the amount of Louise’s goal so, this information may not be useful to her. Although, it can be noted that campaigns may have failed because the goal was simply too high.
---
---
### Challenges and Difficulties Encountered
---
##### The campaigns with the highest goal amounts present some challenges in analyzing the dataset. It is possible that these campaigns are anomalies or outliers and may not be relevant to Louise’s campaign. The solution is to eliminate those campaigns from the dataset.
---
---
## Results
---
---
##### It can be concluded that campaigns launched in May and June have the most successful outcomes. May and June are ideal for launching a successful campaign.
##### It can also be concluded that a campaign is less likely of a success if it is launched in the months of November, December, January or February.  
---
---
##### Based on the data compiled from campaigns with goal ranges between less than $1000 and $4999, these campaigns have the highest percentage of success. Campaigns with a goal in the range of $5000 to $14000 have only about a 50% chance of being successful. Campaigns with goals above $45000 were the least successful in reaching their goals.
---
---
##### The dataset has some possible limitations. For example, it would be useful to know more specifics about what exactly a theater crowdfunding campaign is for. Is the campaign to raise funds to promote a play or a musical? Is the campaign to raise funds to renovate a theater? Having these details could eliminate some of the campaigns with higher goal amounts as well as provide Louise with details more specific to campaigns for plays like her own.
---
---
##### The addition of a pivot table showing the number of backers for successful and failed campaigns would be useful in determining the average number backers needed for a successful campaign. A stacked column chart would provide a good visualization for this data.


