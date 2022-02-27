# Kickstarting with Excel

## Overview of Project
Kickstarter is a platform, which uses crowdfunding to fund creative projects. This project examines global Kickstarter campaigns from 2009 to 2017 and aims to uncover trends related to specific factors that make a project's campaign successful.

### Purpose
The purpose of this project to to gain insights on how different campaigns, fared in relation to their launch dates and their funding goals can aid Louise in planning her own fundraising campaign. 

## Analysis and Challenges
Before proceeding with the analysis, the dataset needed to be further organized by breaking down the “category and subcategory” column in the worksheet, which groups the parent category with its subcategory. By creating separate columns, a more detailed analysis could be conducted. Additionally, the deadline and launched at column (Column I & J) were used to calculate the date each campaign was created and ended. Finally, the date created conversion column was used to indicate the year of the campaign in column U.

[Kickstarter Challenge]

### Analysis of Outcomes Based on Launch Date
The focus of this analysis is to analyze the outcomes (successful, failed and canceled) of theater campaigns, based on their launch date. In order to do this, the Kickstarter dataset needed to be further organized by creating a “years” column as aforementioned. The year was extracted from the “date created conversion” column, which indicates the year the campaign was launched. A pivot table was then created with the entire Kickstarter data set, by customizing the fields to include filters with “parent category” and “years,” rows with “date created conversion” and columns and values with “outcomes”. By setting up these fields, the pivot chart can then be filtered by removing the outcomes of live campaigns, changing the rows to only show the months of the year and filtering the parent category to show data for “theater” only. To visualize the data from the pivot table, a line chart with markers was created to show the relationship between theater campaign outcomes based on their launch month.

![Resources/Theater_Outcomes_vs_Launch](/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The focus of this analysis is to analyze the percentage of successful, failed and canceled plays within a range of the funding goal amounts. In order to do this a table needed to be created on a new sheet within the Kickstarter MS Excel workbook. The table aims to capture the outcomes based on campaign funding goals, which are broken down in to 12 groupings, ranging from less than $1,000 up to greater than $50,000. he COUNTIFS function was then used to obtain the outcome and goal data for the “plays” subcategory, to determine the number of successful, failed and canceled campaigns based off the corresponding funding goal. With this data, the total number of successful, failed and canceled campaigns could easily be calculated by using the SUM() function. Upon calculating the percentage of successful, failed and canceled projects, a line chart was created to visualize the data. The X-axis noted the funding goal ranges and the Y-axis indicated the percentages of successful, failed and canceled campaigns.

![Resources/Outcomes_vs_Goals](/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
The main challenge I encountered while working on this project was solidifying the COUNTIFS() formula to use for the different goal ranges. The invalidity of the original formulas I was using kept resulting in "0" values and thus affecting the supplemental line chart. I was able to fix this error by utilizing Google resources and stumbled upon a YouTube video that helped explain parameters and arguments of the function. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date? The success rate of launching theater campaigns are highest May followed by June. There is a steady decline in the success rate of launched campaigns between October to December and an increase in failures between September and October.

- What can you conclude about the Outcomes based on Goals? The rate of success is higher for campaigns with a funding goal that is less than $5,000. Campaigns with a funding goal of less than a $1,000 up to $4,999 had a success rate ranging from 72.66% - 75.81%, while campaigns with higher funding goals didn’t have nearly as high of a success rate.

- What are some limitations of this dataset? One limitation of the dataset includes the lack of data past 2017. Additionally, including more data points may allow for an increase in data points specific to plays, which is another limitation of the dataset. This would provide more information and allow to better analyze trends related to Louise's fundraising campaign. 

- What are some other possible tables and/or graphs that we could create? 
