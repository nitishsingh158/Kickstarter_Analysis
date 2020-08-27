# Analysis of Kikstarter Campaigns

### Overview of Project
The project analyses Kickstarter data from 2010 to 2017 to finds trends and patterns for launching a successful funding campaign for theater plays. 
### Purpose
The purpose for this analyses is to help individuals who are interested in launching a funding campaign for theater plays on Kickstarter. This analysis provides statistics and insights that can be used to make decisions related to funding amounts, launch dates, launch periods to launch a potentially successful campaign.  
### Analysis and Challenges
This analysis was completed using Microsoft Excel and so in order to work with the tool, one needs to download the spreadsheet `Kickstarter_Challenge.xlsx` from this repository and open that in a spreadhsheet processing tool.

#### Analysis Methodology
1. Outcomes Based on Launch Date
The first analysis looks at the outcomes of the kickstarter theater campaings based on the laucnh data or more specifically by the launch month. The objective is to see if there are any visible trends when it comes to lauching a succesful theater play campaign. In order to complete the analysis:
a. The dates in the data set were converted from UNIX timestamp to short data type and the year and month was extracted from each date. 
b. Next, the entire kickstarter dataset was selected in a pivot table with the following selections:
   -`Parent Category` and `Years` as the filter.
   -`outcomes` in the columns and values
   -`Years` in the row labels, adjust the row labels settings so that instead of showing the data per year the data is showed for each month.
c. Next, filter the data based on the 'theater' parent category and plot the resulting pivot table.

2. Outcomes Based on Goals
The second analysis looks at the outcomes of the kickstarter theater based on the funding goals for the campaigns. To get a better insight into the trends, the goal data was distributed into 11 bins of equal intervals starting from 'less than $1,000' and going to '$50,000 and above'. In order to complete the analysis:
a. Create bin intervals starting from $1,000 and incrmenting by $4,999 goin all the way upto $50,000. 
b. Next, use the `COUNTIF` function to find out total number of successful, failed and canceled projects for each bin range.
c. Next, calculate the percentage of successful, failed and canceled projects for each bin range.
d. Plot the percentage successful, failed and canceled data for each bin in a line chart. 

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

![alt text]resources/Outcomes_vs_Goals.png
- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create? 
