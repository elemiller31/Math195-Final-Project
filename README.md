# South Carolina

## Background

In 2021, South Carolina passed their congressional districting plan following the 2020 census. In October of 2021, the South Carolina National Association for the Advancement of Colored People (NAACP)  filed a lawsuit saying that Congressional District 1 of the plan was a racial gerrymander. However, the case was dismissed with prejudice Aug 2024. Shortly before it was dismissed, in July, 2024, a new case was brought forth by the Women League of Voters of South Carolina claiming that the plan was a partisan gerrymander.

The graphic on the left represents the distribution of Democratic and Republican voters with bluer shapes meaning the precinct has more Democratic voters. Meanwhile, the graphic in the middle represents the distribution of the Black population in South Carolina by precincts with the more yellow representing a higher population of Black individuals.

## Data

I downloaded the congressional district plan shapefile from the South Carolina Redistricting 2021 Senate Judiciary Committee website. It is the plan S.865 as passed by the S.C. General Assembly and signed by Governor McMaster.

I used the 2022 U.S. Senate Election results from the Redistricting Data Hub. Then, I joined race demographics at the block level from the 2020 Census Data which I joined with block shapefile data from Tiger/Shapefiles website, which I aggregated up to the precinct level to combine with the voting data. This provided me with a GeoDataFrame with precinct voting and demographic data for South Carolina which I could use to run and analyze my Markov Chain.

## Analysis

To analyze partisanship in South Carolina, we used the 2022 U.S. Senate Election results between Democrat Krystle Matthews and Republican Tim Scott. Using the 2021 plan and the votes from the 2022 Senate election, Democratic House candidates would have won in 1 district while Republican candidates would have won in 6 districts. Furthermore, the 2021 plan had 1 Black majority district.

Using a random walk starting at a random initial districting plan, we ran our chain for 10,000 steps to explore the state space of South Carolina to find what districting plans were most likely. We found that 0 Democratic majority districts and 0 Black majority districts were most likely. Thus, our random walk seems to suggest that the plan was not a partisan gerrymander against the Democratic voting population or a racial gerrymander against the Black population.

## Mixing Time

To ensure we ran our random walk for long enough, we compared the previous results to the distributions of results from the random walk starting at both the 2021. Below are box and whisker plots showing the outcome. 

Since the distribution for the districts across all three random walks is very similar, we argued that running our walk for 10,000 steps was sufficiently long.

We also compared the results from our random walk for 10,000 steps to a random walk for 20,000 steps that started at the same random initial districting plan. The distributions for both the 10,000-step and 20,000-step random walks were similar, suggesting that running our random walk for more steps would not affect the outcome.

## Limitations

One limitation in our predictions was that we used data from 2022 to predict voter party preference two years later. We are assuming voters' party preference would stay the same and are not taking into account how time or candidates could affect how a voter votes.

Furthermore, although our ensemble suggests that there should be 0 Democratic majority districts in South Carolina, our ensemble did suggest that 1 Democratic district was feasible. Similarly, while the ensemble suggested that 0 Black majority districts was most likely, it did include 1 and even 2 Black majority districts as possibilities. However, our ensemble does not have all the information so if it had all information, it could have a different distribution of most likely plans.

## Conclusion

The ensemble analysis suggests that the districting plan in South Carolina was not a partisan and racial gerrymander. For the purposes of our analysis, we will conclude that based on the ensemble analysis, in 2024, South Carolina should have 0 Democratic districts (instead of the 1 district that elected a Democratic Representative in 2024) as well as 0 Black majority districts. 
