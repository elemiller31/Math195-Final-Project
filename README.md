# Florida
## Background:
After the 2020 Census, the Florida legislature proposed two districting plans for the US Congressional Districts. The primary plan, H00C8109, was put forward, but a secondary plan, H00C8015, was also proposed in case the first plan was invalidated. This invalidation would have occurred over Congressional District 5. Before 2020, this district was a primarily-Black district. The primary plan is argued to have cracked the Black voters into two different districts, therefore invalidating their ability to have a meaningful say. 

After both of these plans (the primary and secondary) were proposed, the Florida governor vetoed these plans. Instead, he created a Special Session of the Florida Legislature to create a new map, P000C0109. It was during this session that the official map, used in both the 2022 and 2024 elections, was created. 

Shortly after, plaintiffs took this case to court, arguing that it was a racial gerrymander. Florida has a “Fair Districts Amendment”, which forbids racial gerrymandering. To note, in 2012, the Supreme Court ruled that if a minority-majority district already exists, a state legislature can not dismantle this district. However, the Florida District Court of Appeals did not apply this reasoning, instead stating that maintaining a minority-majority district would require a non-geographically compact district. 

This case is currently in the hands of the Florida Supreme Court to decide whether the District Court of Appeals properly applied the legislation over the plan. In the meantime, P000C0109 continues to be used. 

Objective: This analysis aims to determine whether there is evidence that Florida racially gerrymandered their Congressional Districts in 2020. 
## Data:
I focused on three different Congressional Districting Plans enacted by Florida, as detailed above: H00C8109 (the primary proposal), H00C8015 (the secondary plan), and P000C0109 (the current plan used in both the 2022 and 2024 election).
 
I collected the precinct dataset from Redistricting Data Hub, which had collected the precinct-level 2022 election results and boundaries from the Florida Division of Elections. 

I then combined this precinct voting dataset with the three congressional districting plans. I found Shapefiles for each of the plans from the NEED TO FILL IN

After combining those shapefiles into a new GeoDataFrame, I combined it with the Census Data. The Census Data, provided by the US Census Bureau, is in Block form. I first had to join the Census Data to a Shapefile with Block to Precinct matching (from the 2022 TIGER/Line Shapefiles Website), then aggregate the block census data up to the precinct level. 
Finally, I combine the aggregated precinct census data with the precinct voting and congressional districting data. This allowed me to have one Geodataframe with all the necessary information to conduct my analysis. 

## Analysis:
According to the Ensemble Analysis, 0 districts should have a black minority-majority (greater than 40%). I conducted a ReCom random walk from the Adopted plan (for 10,000 steps), the Original plan (for 10,000 and 20,000 steps), and two different random plans (for 10,000 steps). All five of these had a majority of plans with zero minority-majority Black districts. Each of these plans did have the possibility of one black minority-majority district, but this was not likely.

To examine this further, I also created a box-and-whiskers plot of the Black population percentage, which shows that having a black minority-majority district would be an outlier. 

Although this court case was regarding racial gerrymandering, I wanted to examine how a Markov Chain random walk on the map of Florida would impact the number of Democratic districts. Every plan recommended 7 Democratic districts, with 5, 6, 8, and 9 also being a valid choice. In all of the plans put forth by the Florida legislature, there are 8 Democratic districts. Therefore, if we were to use the ensemble recommendations in the 2024 election, one seat would flip to a Republican seat from a Democratic seat. 

## Mixing Time:
I ran multiple different random walks, with various starting plans and running lengths, to ensure that our ensemble was completely mixed. For each random walk, I created a box-and-whiskers plot detailing the percentage of Democratic votes in each district. I have included the box-and-whiskers plot for all five runs. Because I got very similar results between all four, it concludes that the Markov Chain is close to stationary at 10,000 steps. 

## Limitations:
The first limitation in this analysis occurred in the set-up of the map, as I had to connect certain precincts to others by hand. As Florida is on the water, there are many islands. To run the ensemble analysis, I had to manually create edges, or connections, between these islands and the closest mainland precinct. To do this, I found precinct-level maps for each county that contained an unconnected island and visually identified the closest precinct. Although I did this to the best of my ability, I might have connected these precincts in different ways than the plans did and thus added a limitation to this analysis.

Although our Ensemble does not recommend having a Black minority-majority district, this does not mean that there shouldn’t be one. One of the current contentions in the Political Districting landscape is overforming minority-majority districts. Should there be a requirement to form a minority-majority district if it is possible, even if it is not likely? Although the Supreme Court recently ruled that the answer to that question should be yes, it is taking some time for this ruling to be applied universally. In addition, it is not clear whether the circumstances have to be the same, meaning that some lower courts are still ruling with an answer of no to that question. In this ensemble, we do not emphasize forming minority-majority districts, thus effectively answering no to this question. 

Although the Ensemble plan recommends seven Democratic seats, electing eight does not mean that there is a political gerrymander. Similar to the discussion in the paragraph above, requiring the formation of a minority-majority district would most likely lead to an additional Democratic seat. Additionally, although seven was the most likely, eight was not impossible. This means that eight Democratic seats is not unreasonable, and therefore can’t be automatically ruled as a political gerrymander.
## Conclusion:
There is no evidence to suspect racial gerrymandering when considering the Ensemble Analysis. However, this does not mean that there is no evidence. When considering the changes in districts from pre-2020 Congressional Districts and the new plans, it is clear that one minority-majority district was broken up. However, is this evidence to prove that racial gerrymandering occurred? And if so, why is it not reflected in our ensemble analysis? These are active questions to consider in a future research project. 

For purposes of our analysis, we can conclude that creating a plan based on the ensemble would decrease the number of Democratic districts in Florida by one.
