# Georgia

For images refer to the pdf report in the main branch.

## Background

Georgia passed their congressional districting map in 2021. However, in December of 2021, it was challenged as an unconstitutional partisan and racial gerrymandering, and in October, 2023, the court found the map in violation of the Voting Rights Act. They ordered the state to put into effect a new map by the end of December which would then be used in the 2024 election. The 2023 plan was a placeholder to address some of the problems with the 2021 plan so that the 2024 election would have a less problematic plan. While the court approved the new map, plaintiffs are still arguing that the Republican proposed 2023 map is unfair.

## Data

Since Georgia had two congressional districting plans since the 2020 census, I wanted to use both of them and analyze how gerrymandered they were compared to the Markov chain from a random district. I found shapefiles for both the 2021 and 2023 congressional districting maps from the Proposed Plans tab on the Georgia General Assembly website.

I used the Georgia 2022 U.S. Senate runoff election results from Redistricting Data Hub. Since results did not include precinct geometries, I joined the election data with the shapefile in the folder ga_2022_gen_st_prec from the 2022 General Senate Results to get the precinct geometries. Then, I joined race demographics at the block level from the 2020 Census Data which I joined with block shapefile data from Tiger/Shapefiles website, which I then aggregated up to the precinct level to then combine with the voting data. This provided me with a GeoDataFrame with precinct voting and demographic data for Georgia which I could use to run and analyze my Markov Chain.

## Analysis

To analyze partisanship in Georgia, we used the 2022 U.S. Senate Runoff Election results between Democrat Raphael Warnock and Republican Herschel Junior Walker. Using both the 2021 and 2023 plan and the votes from the 2022 Senate election, Democratic House candidates would have won in 5 districts while Republican candidates would have won in 9 districts. Furthermore, the 2021 plan had 3 Black majority districts and the 2023 plan had 4 Black majority districts.

Using a random walk starting at a random initial districting plan, we ran our chain for 10,000 steps to explore the state space of Georgia to find what districting plans were most likely. We found that 6 Democratic majority districts and 5 Black majority districts were most likely, however 5 Black majority districts were pretty close. Thus, our random walk seems to suggest that both plans were a racial and partisan gerrymander.

## Mixing Time

To ensure we ran our random walk for long enough, we compared the previous results to the distributions of results from random walk starting at both the 2021 and the 2023 plan.

Since the distribution for the districts across all three random walks is very similar, we argued that running our walk for 10,000 steps was sufficiently long.

We also compared the results from our random walk for 10,000 steps to a random walk for 20,000 steps that started at the same random initial districting plan. The distributions for both the 10,000 step and 20,000 step random walks were similar, suggesting that running our random walk for more steps would not affect the outcome.

## Limitations

One limitation in the analysis of Georgia is that we used voting data results from 2022 to predict what party voters would vote for in 2024. We are assuming voters' party preference would stay the same and are not taking into account how time or candidates could affect how a voter votes.

Furthermore, although our ensemble suggests that there should be 6 Democratic majority districts in Georgia, our ensemble’s second most likely scenario was that Georgia would have 5 Democratic districts. Therefore, we cannot claim outright that either map was a partisan gerrymander. Similarly, while the ensemble suggested that 5 Black majority districts was most likely, it did include 3 and 4 Black majority districts as possibilities. However, our ensemble does not have all the information.

## Conclusions

The ensemble analysis suggests that both districting maps in Georgia were partisan and racial gerrymanders, however we cannot conclude that as definitive. But for the purposes of our analysis, we will conclude that based on the ensemble analysis, in 2024, Georgia should have 6 Democratic districts (instead of the 5 districts that elected Democratic Representatives in 2024) as well as 5 Black majority districts. 
