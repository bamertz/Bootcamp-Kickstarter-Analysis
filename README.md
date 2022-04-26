# Kickstarting with Excel

## Overview of Project

### Purpose

Analyzed Kickstarter campaign data to help Louise understand and visualize how different campaigns fared in relation to their launch dates and their funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

After constructing the graph “Theater Outcomes Based on Launch Date” one can determine the months that offer the greatest opportunity for successful campaigns. May, June, and July appear to be the most successful months with success rates of 67%, 65%, and 63% respectively. The least successful month is December with a 47% success rate.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/103224405/165211943-6047342b-e2ce-4ef0-909a-2b6d19730559.png)

### Analysis of Outcomes Based on Goals

After constructing the graph “Outcomes Based on Goal,” one can determine that the greatest opportunity for a play’s successful fundraising campaign is when its goal is less than $1000 at %76 and 73% at less than $5000. The next best range for a play’s successful fundraising campaign falls between $35,000 and $45,000 at 67%. The least successful range for a play’s fundraising campaign is greater than $45,000.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/103224405/165211942-eabf25ad-3e70-4ccd-afb9-a61bb57646e5.png)

### Challenges and Difficulties Encountered

While I was working on the Outcomes Based on Goal chart, I was double checking my work by summing the total in the “Number Successful” column `=SUM(B2:B13)` with a COUNTIFS statement `=COUNTIFS(Kickstarter!$F:$F,"successful",Kickstarter!$O:$O,"plays")`by
just counting how many plays were successful and the two values were not adding up. I knew these numbers needed to be equal since it was accounting for every number from zero to infinity. My chart also didn’t match the one on the module. I discovered that I had only less than `<`or greater than `<`, but not less than or equal to `<=` or greater than or equal to `>=` in my equations. Once I put those in, everything checked out. 

## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?

1.	May is the most successful month to launch a theater fundraising campaign.

2.	December is the least successful month to launch a theater fundraising campaign.

### What can you conclude about the Outcomes based on Goals?

1.	The most successful play fundraisers occur when the goal is less than $1000, less than $5000, or between $35000 and $45000.

### What are some limitations of this dataset?

1.	A limitation of this dataset is that the cities of these backers is not listed. Apart from 2 campaigns, there are less than 9000 backers for every campaign. Given how large each country is, it would be beneficial to know if the backers are localized to specific cities within each country. This would make it easier to advertise each Kickstarter campaign. 

2.	Another limitation of this dataset is that we cannot see how many people clicked or viewed each campaign. It would be helpful to know what the percentage of people who donated vs viewed each campaign. Additionally, adding descriptive and selective categories that say why or why they didn’t donate would be helpful.

### What are some other possible tables and/or graphs that we could create?

1.	Creating tables or graphs to show which locations of play campaigns are the most successful. 

2.	Creating tables or graphs to show which locations of theater outcomes are the most successful. 
