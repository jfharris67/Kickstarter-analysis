# Kickstarting with Excel

## Overview of Project
An analysis of theatre and play campaigns in relation to their launch dates and funding goals.

### Purpose

Louise is close to achieving her goal of $10,000 for her play "Fever." She is interested in knowing how other campaigns went based on their funding goals and launch dates.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

Using a previous analysis, I performed the additional analysis below, paying particular attention to theatre launch dates.

I created a new column in the Kickstarter worksheet labeled "Years." For this column, I used the YEAR() function in this column to extract the year from the "Date Created Conversion" column. I created a pivot table filtering the columns by "successful," "failed," and "canceled." I filtered the parent category by "Theatre." I then created a line pivot chart (below).
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/114355199/204607091-6c2545c1-43ed-401f-9c3e-3b260eda5a4c.png)


### Analysis of Outcomes Based on Goals

Within the worksheet labeled "Outcomes Based on Goals," I created columns, Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, and Percentage Canceled. For the "Goal" column, I created several dollar amounts ranges to group the projects by their goal amount. I used the COUNTIFS() function to populate the "Number Successful," "Number Failed," and "Number Canceled" columns using criteria based on the "Goal" column and "Subcategory" based on "Plays." The "Total Projects" column is the sum of successful, failed, and canceled projects.
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/114355199/204840415-16d252cf-1c9b-43e3-a8f8-103a82df174e.png)
### Challenges and Difficulties Encountered
The biggest challenge I encountered was identifying the subcategory "Plays" based on the launch date. Further analysis was performed to identify success rates for this subcategory. Seeing this project was for a play, I wanted to do a deeper dive in case the overall theatre category was giving a false analysis.

## Results

- What are two conclusions you can draw about the Outcomes based on the Launch Date?
	- The most popular month for a theatre launch date would be May, followed by June, then July.
	- The best month of the year to launch, according to success rate, would be May. Out of 166 theater launches, 67% were successful. June would be the next best month with a success rate of 65%, followed by July and April with 63%.
	- Looking at the subcategory of "plays" may be more appropriate; the best month to launch would be June. Out of 188 launches, 70% were successful. November, May, and March had a 69% success rate.

- What can you conclude about the Outcomes based on Goals?
	- The highest success rate is campaigning with a goal of less than $1000, achieving 76%. Kickstarter, with a goal between $1000 and $5000, had a slightly less success rate of 73%. Considering the goal for this project is $10,000, the data indicate a success rate of 54%.

- What are some limitations of this dataset?
	- It would have been nice to see revenue and costs generated. I am sure Louise has taken this into account when figuring out her goal, but revenue and cost could also provide her some insight if the overall success of the campaign would align with other plays.
	- It would have been nice to have visibility into what each backer pledged. Looking at the mean, median and mode could have helped us identify outliers. For example, some campaigns could have big donations from a few individuals, which may not be the case with other campaigns. The good news, Louise is close to reaching her goal anyway.

- What are some other possible tables and or graphs that we could create?
	- Further defining the subcategory "plays" based on the launch date. Considering just the parent category may hide a better analysis that would be more appropriate for "plays."
	- Further analysis by year and country could give us more insights.
