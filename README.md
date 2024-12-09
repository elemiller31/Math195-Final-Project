# Louisiana
## Background:
Louisiana first enacted a plan with one Black majority district. This districting plan was reminiscent of the plan used before the 2020 Census. However, one-third of the state's population is Black, meaning that only one minority-majority district out of six congressional districts is not an accurate representation of the Louisiana population. This map was used in the 2022 General Election.

However, the map was challenged for failing to make a second Black-majority district. The Supreme Court ruled that Louisiana must make a new map with two Black-majority districts before the 2024 Election. Although they complied, the second district they created was extremely long and narrow (and not geographically compact) because they wanted to keep certain Republican representatives in office. 

This case is still in litigation, as a court ruled that the new plan is a racial gerrymander. This court argues that race was a consideration in making the new districting plan, and thus is a racial gerrymander. The Supreme Court has agreed to hear the case, and a decision is expected in 2025.

Objective: This analysis aims to determine whether there is evidence that Louisiana racially gerrymandered its Congressional Districts in the 2022 and 2024 plans. 
## Data:
I focused on two different Congressional Districting Plans enacted by Louisiana, as detailed above: the plan used in the 2022 election and the plan used in the 2024 election.
 
I collected the precinct dataset from Redistricting Data Hub, which had collected the precinct-level 2022 election results and boundaries from the Louisiana Secretary of State. 

I then combined this precinct voting dataset with the two congressional districting plans. I found Shapefiles for each of the plans from the Louisiana Redistricting Website.

After combining those shapefiles into a new GeoDataFrame, I combined it with the Census Data. The Census Data, provided by the US Census Bureau, is in Block form. I first had to join the Census Data to a Shapefile with Block to Precinct matching (from the 2022 TIGER/Line Shapefiles Website), then aggregate the block census data up to the precinct level. 
Finally, I combine the aggregated precinct census data with the precinct voting and congressional districting data. This allowed me to have one Geodataframe with all the necessary information to conduct my analysis. 

## Analysis:
According to the Ensemble Analysis, 0 districts should have a black minority-majority (greater than 40%). I conducted a ReCom random walk from the Original plan (for 20,000 and 40,000 steps) and two different random plans (for 20,000 steps). All five of these had a majority of plans with zero minority-majority Black districts. Each of these plans did have the possibility of one black minority-majority district, but this was not as likely.

To examine this further, I also created a box-and-whiskers plot of the Black population percentage, which shows that having either one or two black minority-majority districts would be an outlier. 

Although this court case was regarding racial gerrymandering, I wanted to examine how a Markov Chain random walk on the map of Louisiana would impact the number of Democratic districts. Every plan recommended 1 Democratic district, with 0 also being a valid choice. In the 2022 Plan, there was one Democratic district. In the 2024 Plan, there were two Democratic districts. If we were to modify the 2024 election results based on the ensemble, one Democratic seat would be flipped to Republican. 
## Mixing Time:
I ran multiple different random walks, with various starting plans and running lengths, to ensure that our ensemble was completely mixed. For each random walk, I created a box-and-whiskers plot detailing the percentage of Democratic votes in each district. I have included the box-and-whiskers plot for all five runs. Because I got very similar results between all four, it concludes that the Markov Chain is close to stationary at 10,000 steps. 

## Limitations:
Although the most likely possibility in our ensemble is to have no minority-majority districts, this does not mean that having one or two is a sign of racially gerrymandering. As discussed above, one minority-majority district was also a possibility. Additionally, there may be inconsistencies in our data or how we create the ensemble that would reduce the likelihood of a minority-majority district occurring. Similarly as discussed in Florida, there is also the question (and ongoing debate) of whether a minority-majority district should be formed because it can be formed, or because it is the most likely occurrence.
## Conclusion:
There is not enough evidence to suggest racial gerrymandering when considering the Ensemble Analysis, but our initial ensemble suggests that two minority-majority districts is not a common occurrence. When considering the change in plans from 2022 to 2024, we see a new minority-majority district formed that is not geographically compact. 

For purposes of our analysis, we can conclude that creating a plan based on the ensemble would decrease the number of Democratic districts in Louisiana by one.
