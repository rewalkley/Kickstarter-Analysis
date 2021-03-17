# Kickstarter-Analysis

## Overview of Project
The purpose of this project is to help Loise compare her Kickstarter campaign to similar campaigns of different dates and funding goals.

## Analysis and Challenges
In order to properly analyze the campaigns, I first needed to breakdown the data to graphically show which theater campaigns were successful and why. 

### Theater Outcomes by Launch Date
First, I needed to know the theater campaigns' outcomes were based on their launch date. To do this, I had to break out the Parent Category from the Category and Subcategory column from the data set in order to filter on Theater campaigns only. Then, in order to determine the Launch Date, I needed to add a formula in a new column that converted the Unix Timestamp to a readable date. This result allowed me to graphically represent the total Theater Campaigns that were successful, failed or canceled by month in which they were launched: ![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/80076110/111409571-34e3c400-86a5-11eb-8cb4-d5d75b659406.png)

### Outcomes Based on Goals
Next, I needed to understand the outcome of the plays campaigns, based on their goal amount. In order to achieve this, I needed to create a new tab to list out the plays campaigns in various goal ranges, from Less than 1000 to Greater than 50000 in ranges of 5000, by number successful/failed/canceled: [Outcomes Based on Goals.zip](https://github.com/rewalkley/Kickstarter-Analysis/files/6153624/Outcomes.Based.on.Goals.zip)
 Further, the percentage of each outcome based on the total of each outcome by the total number of projects was found using SUM and division formulas. This produced a pivot chart that graphically depicts the Outcomes Based on Goals:![Outcomes_vs_Goals](https://user-images.githubusercontent.com/80076110/111410192-46799b80-86a6-11eb-9755-d2b5b5163ed7.png)

### Challenges
One particular challenge I ran into was the conditional formatting of the Percentage Funded column in the dataset. Following the directions to use a 2-scale color scheme with red for the lowest value and blue for the highest value, the result had all cells, no matter the number, highlighted red. I could not figure out how to fix this issue, so I began to play around with the formatting options until I found by substituting the Minimum and Maximum types from Lowest and Highest Value with percentile, I was able to get the same result as per the instructions.

## Results
1. By glancing at the Theater Outcomes by Launch Date graph, one can conclude that the number of successful theater campaigns is significantly greater than failed/canceled campaigns; the only month where successful campaigns is not more than both failed and canceled combined is December. Another conclusion noted when reviewing the graph is that the number of successful campaigns is greater in the middle of the year vs the beginning and end of the calendar year.
2. From the Outcomes Based on Goals data, I can attest that the highest liklihood of success occurs the lower the goal amount is for the campaign. 
3. However, this graph does not tell the whole story, as the total number of campaigns is skewed heavily towards the smallest ranges. 
4. It may be helpful to chart a 4th series on a secondary access showing the total number of campaigns for each range on the Outcomes Based on Goals graph. Another helpful option for Louise may be to graphically depict which campaigns had the highest number of backers by goal amount in the theater subactegory.
