# Kickstarter-Analysis

## Overview of Project
The purpose of this project is to help Loise compare her Kickstarter campaign to similar campaigns of different dates and funding goals.

## Analysis and Challenges
In order to properly analyze the campaigns, I first needed to breakdown the data to graphically show which theater campaigns were successful and why. 

### Theater Outcomes by Launch Date
First, I needed to know which campaigns were successful based on their launch date. To do this, I had to break out the Parent Category from the Category and Subcategory column from the data set in order to filter on Theater campaigns only. Then, in order to determine the Launch Date, I needed to add a formula in a new column that converted the Unix Timestamp to a readable date. This result allowed me to graphically represent the total Theater Campaigns that were successful, failed or canceled by month in which they were launched:



