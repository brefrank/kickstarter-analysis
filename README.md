# Kickstarting with Excel

## Overview of Project

Using data from our Kickstarter Challenge spreadsheet, a visualization of theater campaign outcomes based on launch dates and play funding goals has been created. The goal of this project was to gain a better understanding of how other plays compared to Louise’s play 'Fever'.

[Kickstarter_Challenge.xlsx](https://github.com/brefrank/kickstarter-analysis/files/7157197/Kickstarter_Challenge.xlsx)

### Analysis of Outcomes Based on Launch Date

To gather an understanding of how launch dates affected theater campaign outcomes, a pivot table and line chart was created from data within the 'Kickstarter' tab of our 'Kickstarter Challenge' spreadsheet. To start, the pivot table was filtered to show only theater data and sorted into three groups by month. Data on each campaign had been documented over an 8 year spread, 2009-2017. Using this information, these three groups of successful, failed, and cancelled, provided summarized data on which months would be best to start a campaign. 

As you can see from the chart below, May had the highest campaign success. More details on individual quantities can be found on the third tab, 'Theater Outcomes by Launch Date'.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/90646961/133155798-5654bb44-ceb8-4a9d-a8ae-6d3cefab3dc4.png)

### Analysis of Outcomes Based on Goals

Next, a table was created to calculate percentages of success, failure, and canceled campaigns relative to the monetary goals set for individual plays within the theater umbrella. To gather this information, COUNTIFS formulas were used to populate our table data by goal range and outcome and the converted into percentage. 

For example, the amount of successful plays with a goal amount between $1000 and $4999 was calculated with the following formula:
=COUNTIFS(Kickstarter!D:D, ">=1000", Kickstarter!F:F, "failed", Kickstarter!D:D, "<=4999", Kickstarter!Q:Q, "plays")
The result of 388 successful plays was then converted to a perccentage by dividing 388 by total plays with goals between $1000 and $4999 and multiplying by 100. More details on value calculation can be viewed on the second tab of our Kickstarter spreadsheet. 

Below is a line graph of our calculated data. Since there werent any cancelled plays in our data set, the successful and failing lines are directly proportional. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/90646961/133854389-8b5fe018-240e-42e7-9c38-a17ccafc264f.png)

### Challenges and Difficulties Encountered

Although there was a lot of sorting and editing of equations involved, this data set was not particularly challenging to manipulate. If we expanded the data involved and asked more specific questions, the difficulty level would increase.

## Results

By looking at success and failure rates by launch date and goal amount, a few conclusions can be made. Because successful theater campains increased drastically between April and May, it is easy to see that they would be the best months to launch a play. Outcome data based on goal amounts was a bit more scattered. Goals less than $1000 had the highest success rate, showing us that it is best to stay below that $1000 mark when choosing a fundraising foal. The success rates then declined fairly steadily until hitting the $30,000 goal - briefly going up again between $30,000 and $44,999 and then shooting down to 0. 

Louise's choice to release 'Fever' during a decline in successful launches, despite having a reasonable  monetary goal, had likely contributed heavily to it's failure. Combining our result sets tells us that if Louise would have started fundraising about a month earlier, she most likely would have been successful in reaching her goal. 

Because our outcomes by launch date data includes all theater groups such as music and spaces, we can not be entirely conclusive without a bit more data. Should we need a bit more certainty, our next task will be to further filter down 'Theater Outcomes by Launch Date' results into each subcategory.   
