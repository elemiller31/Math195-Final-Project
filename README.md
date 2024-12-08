# North Carolina

**Background:**
After the 2020 Census, the North Carolina Legislature created a new political districting map. This map created 3 likely Democratic districts and 11 likely Republican districts. This plan was immediately taken to court over the idea that it was a political gerrymander due to North Carolina state law, which prevented the right to fair maps. The North Carolina Supreme Court then agreed, stating that the maps were illegal and must be redrawn. Further, they required that a temporary map be drawn by the Courts to be used in the 2022 election. This new map increased the number of likely Democratic districts to 7, providing a fair split of districts to each party. 

After the 2022 elections, the North Carolina Supreme Court was shifted from a Democratic-majority (that had ruled earlier) to a Republican-majority. They then overturned the previous ruling, arguing that partisan gerrymandering was not something for the courts to consider, and thus allowing the North Carolina legislation to do whatever they would like. 
This led to the current plan, used in the 2024 elections. This plan was expected to have 3 likely Democratic districts and 11 likely Republican districts. In a surprise to the state, an additional district voted for a Democratic district, bringing the total to 4 Democratic Representatives and 10 Republican Representatives. 

**Objective:** This analysis aims to determine whether there is evidence that North Carolina politically gerrymandered their Congressional Districts in 2020. 

**Data:**
I focused on three different Congressional Districting Plans enacted by North Carolina: the original plan (never used in an election), the court-created temporary plan (used in the 2022 election), and the current plan (used in the 2024 election).
 
I collected the precinct dataset from Redistricting Data Hub, which had collected the precinct-level 2022 election results and boundaries from the North Carolina State Board of Elections. 

I then combined this precinct voting dataset with the three congressional districting plans. I found Shapefiles for each of the plans from the North Carolina General Assembly's Redistricting website.

After combining those shapefiles together into a new GeoDataFrame, I combined it with the Census Data. The Census Data, provided by the US Census Bureau, is in Block form. I first had to join the Census Data to a Shapefile with Block to Precinct matching (from the 2022 TIGER/Line Shapefiles Website), then aggregate the block census data up to the precinct level. 
Finally, I combine the aggregated precinct census data with the precinct voting and congressional districting data. This allowed me to have one Geodataframe with all the necessary information to conduct my analysis. 

**Analysis:**
According to the Ensemble Analysis, 5 districts should have a Democratic Majority. I conducted a ReCom random walk from the Adopted plan (for 10,000 and 20,000 steps), the Temporary plan (for 10,000 steps), and a random plan (for 10,000 steps). All four of these had a majority of plans with 5 democratic-majority districts. 4 and 6 districts were also likely, whereas 3 and 7 were possible but not likely. 

If we were to use the ensemble recommendations in the 2024 election, North Carolina would have an additional Democratic district. In the 2024 General Elections, North Carolina elected the Democratic district in 4 out of the 14 districts. However, our ensemble recommends 5 Democratic districts as the most common. Therefore, a new plan based on our ensemble would flip one Republican seat to a Democratic seat

**Mixing Time:**
I ran multiple different random walks, with various starting plans and running lengths, to ensure that our ensemble was completely mixed. For each random walk, I created a box-and-whiskers plot detailing the percentage of Democratic votes in each district. I have included the box-and-whiskers plot for all four runs. Because I got very similar results between all four, it concludes that the Markov Chain is close to stationary at 10,000 steps. 

**Limitations:**
Although the Ensemble plan recommends five Democratic seats, electing four does not mean that there is a political gerrymander. Our ensemble analysis shows that although five seats are the most likely, four seats are still a possible (and somewhat likely) outcome. Therefore, we can not conclude that a political gerrymander occurred in North Carolina in the adopted plan.

Further, we do not have sufficient evidence that the original plan was also a political gerrymander. As noted above, the possibility of having 3 seats did appear. Although it was unlikely, it is much more likely than one or two Democratic seats. In addition, we are not sure that we have all the information. Because we were using data from the 2022 election, we do not know how individual votes changed in the 2024 election. 

**Conclusion:**
Although there is evidence to suspect political gerrymandering, there is not clear and convincing evidence that political gerrymandering occurred in North Carolina. Because we are unsure if our random walk has all the necessary information, along with the fact that we did see some plans with three democratic districts, we can not conclude that there was an obvious gerrymander. 

However, for purposes of our analysis, we can conclude that creating a plan based on the ensemble would increase the number of Democratic districts in North Carolina by one.



