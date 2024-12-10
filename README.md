# Texas

For images see pdf report on main branch

## Background

Following the 2020 census, Texas passed their new congressional districting plan on October 25, 2021. However, it was quickly brought to court for numerous litigation claims that it was a racial gerrymander against Black and Latino voters. 

## Data

Since Texas has only had one districting plan put into place following the 2020 census, I wanted to compare that one to a Markov chain from a random districting plan. I used the congressional map shapefile from the Capitol Data Portal for the Texas Legislative Council. 

I used the 2020 U.S. Presidential Election results from the University of Florida Election Lab. Then, I joined race demographics at the block level from the 2020 Census Data which I joined with block shapefile data from Tiger/Shapefiles website, which I then aggregated up to the precinct level to then combine with the voting data. This provided me with a GeoDataFrame with precinct voting and demographic data for Texas which I could use to run and analyze my Markov Chain.

## Analysis

To analyze partisanship in Texas, we used the 2020 U.S. Presidential Election results between Democrat Joe Biden and Republican Donald Trump. Using the 2021 plan and the votes from the 2020 Presidential election, Democratic House candidates would have won in 13 districts while Republican candidates would have won in 25 districts. Furthermore, the 2021 plan had 1 Black majority district and 14 Hispanic majority districts.

Using a random walk starting at a random initial districting plan, we ran our chain for 20,000 steps to explore the state space of Texas to find what districting plans were most likely. We found that 18 Democratic majority districts, 0 Black majority districts, and 16 Hispanic majority districts were most likely. Thus, our random walk seems to suggest that both plans were a racial gerrymander against Hispanic and Latino voters and a partisan gerrymander.

## Mixing Time
To ensure we ran our random walk for long enough, we compared the previous results to the distributions of results from random walk starting at the 2021. Below are box and whisker plots showing the outcome. 

Since Texas has so many districts, it is a bit challenging to read the plots. However, we can see the two random walks have similar distributions though not the same or as close as we saw for Georgia. Thus, I think that running our walk for 20,000 steps was not sufficiently long.

Moreover, we also compared the results from our random walk for 20,000 steps to a random walk for 30,000 steps that started at the same random initial districting plan. The distributions for the 30,000 step random walk were a bit different from the distribution of the 20,000, corroborating the belief that the random walk had not yet converged at 20,000 steps and that we should have run it for longer. 

## Limitations

One limitation in our predictions was that we used data from 2020 to predict voter party preference four years later. While there was no U.S. Senate election in 2022, there were both elections for Governor and Attorney General, which are statewide elections. However, we decided not to use the 2022 Attorney General race between Republican Ken Paxton and Democrat Rochelle Garza because Paxton has faced security fraud charges and is being investigated by the FBI. This election did not seem like a normal one, and we wanted more conventional election candidates to best predict how voters would vote. We were going to use the results for the 2022 Governor election, but we were only able to find the results by VTDs or by blocks. The VTDs didn’t join nicely to the 2020 census VTDs because they changed and the block data set took too long to load, which is why we had to resort to the 2020 Presidential Election results.

Another effect on our results could be from not running the random walk for long enough. When I ran the random walk for 10,000 steps, it was clear it had not explored all the state space as the distributions for the two different starting points (a random districting plan and the 2021 one) were different. However, even when we ran from 20,000 steps, we still see some difference between the distributions suggesting that we need to run our random walk for 30,000 or more steps to get a reasonable distribution of results.

This could have affected the distribution of Democratic, Black, and Hispanic majority districts our ensemble believes in most likely. The ensemble states that 18 Democratic majority districts, 0 Black majority districts, and 16 Hispanic majority districts were most likely. However there were plans in the distribution that had 13 Democratic districts, 1 Black majority district, and 14 Hispanic majority districts. Another reason that we cannot take the most likely outcome as the truth is that our ensemble does not have all the information. For those reasons, we cannot definitively claim that the 2021 plan was a gerrymander.

## Conclusions

Our ensemble analysis suggests that the districting plan in Texas was gerrymandered, however we cannot conclude that as definitive. But for the purposes of our analysis, we will conclude that based on the ensemble analysis, in 2024, Texas should have had 18 Democratic districts (instead of the 13 districts that elected Democratic Representatives in 2024) as well as 0 Black majority districts and 14 Hispanic majority districts. 
