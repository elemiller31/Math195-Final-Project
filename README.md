# Utah

For images see pdf report on main brainch.

## Background

In November of 2021, Utah passed their congressional districting plan following the 2020 census. In March of 2022, the map was challenged as a partisan gerrymander against Democrats. The challenge is based on the claim that Republican legislators cracked Salt Lake County, a democratic leaning county. In the graphic representing the distribution of Democratic and Republican Voting Precincts, we can see that there is a blue clump of voters representing Democratic voters near the top, which is Salt Lake County. However, in the second graphic, we see that this county is split by all four districts.

## Data

The shapefile for the 2021 congressional districts was labeled “CONGRESS ENROLLED HB2004” under the Congress Tab on the Utah Legislative Redistricting Committee website. 

I used the 2020 U.S. Presidential Election results from the University of Florida Election Lab. Then, I joined race demographics at the block level from the 2020 Census Data which I joined with block shapefile data from Tiger/Shapefiles website, which I then aggregated up to the precinct level to then combine with the voting data. This provided me with a GeoDataFrame with precinct voting and demographic data for Utah which I could use to run and analyze my Markov Chain. 

## Analysis

To analyze partisanship in Utah, we used the 2020 U.S. Presidential Election results between Democrat Joe Biden and Republican Donald Trump. Using the 2021 plan and the votes from the 2020 Presidential election, Democratic House candidates would have won in 0 districts while Republican candidates would have won in all 4 districts. 

Using a random walk starting at a random initial districting plan, we ran our chain for 10,000 steps to explore the state space of Utah to find what districting plans were most likely. We found that the 2021 had 1 Democratic majority district, suggesting the 2021 plan was a partisan gerrymander.

## Mixing Time

To ensure we ran our random walk for long enough, we compared the previous results to the distributions of results from a random walk starting at the 2021 plan. Below are box and whisker plots showing the outcome. 

Since the distribution for the districts for both random walks was very similar, we argued that running our walk for 10,000 steps was sufficiently long.

We also compared the results from our random walk for 10,000 steps to a random walk for 20,000 steps that started at the same random initial districting plan. The distributions for both the 10,000 step and 20,000 step random walks were similar, suggesting that running our random walk for more steps would not affect the outcome.

## Limitations

One limitation was that we used 2020 Presidential Data to predict voters' party preference in 2024. We were unable to use data from the 2022 Midterm elections since the U.S. Senate election was between Republican Mike Lee and Independent Evan McMullin, and we wanted to analyze Republican and Democrat voting likelihood. There were no other state-wide elections in 2022, so we had to go back to 2020. We had the option for Governor, Attorney General, or Presidential election, and we decided to use the Presidential Election because it was the most important.

Another limitation is that our ensembles do not have all the information.While they suggested that 1 Democratic district was most likely, a couple of plans did have 0 Democratic districts.

## Conclusion
The ensemble analysis suggests that the districting plan in Utah was a partisan gerrymander, however we cannot conclude that as definitive. But for the purposes of our analysis, we will conclude that based on the ensemble analysis, in 2024, Utah should have elected 1 Democratic Representative instead of none.
