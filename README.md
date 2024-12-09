# Arkansas
## Background:
After the 2020 Census, Arkansas's new plan divided up the state into four Congressional Districts. This plan contained all likely Republican districts and no minority-majority districts. This plan was then challenged for cracking Black voters in Pulaski County. Originally kept together, this new districting plan divided southeast Little Rock into three different districts. 

Although the defendants argue that no plan can be made with a minority-majority district, the plaintiffs are continuing with the lawsuit. They argue that even a 30 or 40% black population will allow a greater influence on the chosen representative. 

This map was allowed to be used in both the 2022 and 2024 elections. The lawsuit is ongoing, as a three-panel judge just finished listening to both parties. A decision on next steps is expected in the Spring, but the case is not expected to be concluded until later. 

Objective: This analysis aims to determine whether there is evidence that Arkansas racially gerrymandered its Congressional Districts in the 2022 and 2024 plans. 
## Data:
I focused on two different Congressional Districting Plans enacted by Arkansas, as detailed above: the plan used before the 2022 election and the plan used in both the 2022 and 2024 elections.
 
I collected the precinct dataset from Redistricting Data Hub, which had collected the precinct-level 2020 election results from the Voting and Election Science Team and boundaries from the Redistricting Data Hub.

I then combined this precinct voting dataset with the two congressional districting plans. I found Shapefiles for each of the plans from the Redistricting Data Hub.

After combining those shapefiles into a new GeoDataFrame, I combined it with the Census Data. The Census Data, provided by the US Census Bureau, is in Block form. I first had to join the Census Data to a Shapefile with Block to Precinct matching (from the 2022 TIGER/Line Shapefiles Website), then aggregate the block census data up to the precinct level. 
Finally, I combine the aggregated precinct census data with the precinct voting and congressional districting data. This allowed me to have one Geodataframe with all the necessary information to conduct my analysis. 

## Analysis:
According to the Ensemble Analysis, 0 districts should have a black minority-majority (greater than 40%). I conducted a ReCom random walk from the Adopted plan (for 10,000 and 20,000 steps) and a random plan (for 10,000 steps). All three of these had all plans with zero minority-majority Black districts.

To examine this further, I also created a box-and-whiskers plot of the Black population percentage, which shows that having one black minority-majority district would be an outlier. 

Although this court case was regarding racial gerrymandering, I wanted to examine how a Markov Chain random walk on the map of Arkansas would impact the number of Democratic districts. Every plan recommended 0 Democratic districts, with 1 also being a valid (albeit unlikely) choice. In the 2022 and 2024 Plans, there were zero Democratic districts. If we were to modify the 2024 election results based on the ensemble, no seats would change.
## Mixing Time:
I ran multiple different random walks, with various starting plans and running lengths, to ensure that our ensemble was completely mixed. For each random walk, I created a box-and-whiskers plot detailing the percentage of Democratic votes in each district. I have included the box-and-whiskers plot for all five runs. Because I got very similar results between all four, it concludes that the Markov Chain is close to stationary at 10,000 steps. 

## Limitations:
Arkansas only released the 2022 General Election results by county, not precinct. Because a finer level of detail was necessary for our ensemble, I instead had to use the Presidential election data from 2020. At the time of analysis, this data is now four years old. Therefore, it is hard to believe that Arkansas voters have remained the same in the past four years. 

Although I have continued with the analysis, the results can not be considered accurate due to this data discrepancy. As many other states have been analyzed using 2022 data, we can not conclude that the results should be the same between 2020 and 2022 data. 
## Conclusion:
There is no evidence to suggest that racial gerrymandering occurred when Arkansas enacted its Congressional Districting plan. However, this claim is subject to limitations regarding the availability of 2022 data, and the necessity to use 2020 data. 

For our analysis, we can conclude that creating a plan based on the ensemble would keep Arkansas's number of seats in the House the same.

