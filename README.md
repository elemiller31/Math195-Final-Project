# Alabama
(for images, please see the pdf report.)
## Background:
Alabama initially created a Congressional Districting plan, following the 2020 Census, that ensured one Black-majority district. However, this was immediately taken to court over the Voting Rights Act, arguing that Alabama failed to create a second Black-majority district that could have been made. In February of 2022, the Supreme Court issued a stay, allowing the original map to be used in the 2022 election.

Following the 2022 election, the Supreme Court ruled that the initial plan was illegal, as it violated the Second Amendment of the Voting Rights Act. Alabama has pushed back on this, arguing that two minority-majority districts would also be a racial gerrymander. Alabama was then allowed to make a new map but failed to create a second Black-majority district. The Court then stepped in, creating a temporary map to be used in the 2024 election with two Black-majority districts. 

Currently, the State Legislature is figuring out its next steps. They are still awaiting the final decision from the Courts over whether their second drawn map was illegal. Regardless of the decision, it is almost certain that a new map will be utilized in the 2026 elections. 

Objective: This analysis aims to determine whether there is evidence that Alabama racially gerrymandered its congressional districts in the 2022 plan. 
Data:
As detailed above, I focused on two different Congressional Districting Plans enacted by Alabama: the plan used before the 2022 election and the plan used in both the 2022 and 2024 elections.
 
I collected the precinct dataset from Redistricting Data Hub, which had collected the precinct-level 2022 election results from the Alabama Secretary of State.

I then combined this precinct voting dataset with the two congressional districting plans. I found Shapefiles for each of the plans from the Redistricting Data Hub.

After combining those shapefiles into a new GeoDataFrame, I combined it with the Census Data. The Census Data, provided by the US Census Bureau, is in Block form. I first had to join the Census Data to a Shapefile with Block to Precinct matching (from the 2022 TIGER/Line Shapefiles Website), then aggregate the block census data up to the precinct level. 
Finally, I combine the aggregated precinct census data with the precinct voting and congressional districting data. This allowed me to have one Geodataframe with all the necessary information to conduct my analysis. 

## Analysis:
According to the Ensemble Analysis, 0 districts should have a black minority-majority (greater than 40%). I conducted a ReCom random walk from the original plan (for 10,000 and 20,000 steps), the adopted plan (for 10,000 steps), and a random plan (for 10,000 steps). All four of these had majority of plans with zero minority-majority Black districts.

Most Likely # of Black Minority-Majority Districts in Alabama, from a Random Plan

To examine this further, I also created a box-and-whiskers plot of the Black population percentage, which shows that having one black minority-majority district would be an outlier. 

Percentage of Black People per District in Alabama, from a Random Plan 
(Red = 2022 Plan; Green = 2024 Plan)

Although this court case was regarding racial gerrymandering, I wanted to examine how a Markov Chain random walk on the map of Arkansas would impact the number of Democratic districts. Every plan recommended 0 Democratic districts, with 1 also being a valid but unlikely choice. In the 2022 plan, there was one Democratic district. In the 2024 plan, this was increased to two Democratic districts. If we were to modify the 2024 election results based on the most likely outcome of the ensemble, two Democratic districts would flip to Republican, thus losing two Democratic seats in the House.
## Mixing Time:
I ran multiple different random walks, with various starting plans and running lengths, to ensure that our ensemble was completely mixed. For each random walk, I created a box-and-whiskers plot detailing the percentage of Democratic votes in each district. I have included the box-and-whiskers plot for all five runs. Because I got very similar results between all four, it concludes that the Markov Chain is close to stationary at 10,000 steps. 

## Limitations:
Although the most likely possibility in our ensemble is to have no minority-majority districts, this does not mean that having one is a sign of racial gerrymandering. As discussed above, one minority-majority district was also a possibility. Additionally, there may be inconsistencies in our data or how we create the ensemble that would reduce the likelihood of a minority-majority district occurring. Similarly as discussed in Florida and Louisiana, there is also the question (and ongoing debate) of whether a minority-majority district should be formed because it can be formed, or because it is the most likely occurrence.
## Conclusion:
There is not enough evidence to suggest racial gerrymandering when considering the Ensemble Analysis, but our initial ensemble suggests that two minority-majority districts are not a common occurrence. When considering the change in plans from 2022 to 2024, we see a new minority-majority district formed.

For purposes of our analysis, we can conclude that creating a plan based on the ensemble would decrease the number of Democratic districts in Alabama by two.
