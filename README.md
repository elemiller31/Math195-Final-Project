# Georgia

We will be analyzing the congressional district maps in Georgia followwing the 2020 census. Currently Georgia's congressional map is in litigation so we want to examine how that could have effected the 2024 U.S. House election. We will be looking at their 2021 plan which was used for the 2022 election and then a new 2023 plan which was used in the 2024 election. The 2023 plan was a placeholder to fix some of the issues with the 2021 so the 2024 election would have a less problematic map.

Both maps in litigation for partisan and racial gerrymandering. I got shapefiles for the 2021 and 2023 (which was used in the 2024 elections) congressional districting maps from the Proposed Plans tab on [Georgia General Assembly website](https://www.legis.ga.gov/joint-office/reapportionment).

We want to determine what party would have won the election for the U.S. House of Representative in each of the 14 districts for each of the two maps we have for Georgia. However, instead of using House candidates, we will be using 2020 U.S. Senate candidates because those were elected across the whole state. Thus, we will be using the Senate election as a placeholder for the House election because in the next party, once we move the congressional district boundary using a random walk, the candidates for the House would change. We are assuming voters would vote by party so we will use a statewide election where there were two candidates, one from each party, to determine how each voters would vote in a new House election.

Since the 2022 U.S. Senate election led to a runoff election, we will be using the runoff election results from [Redistricting Data Hub](https://redistrictingdatahub.org/dataset/georgia-2022-runoff-election-precinct-level-results/). I then joined these results with the shapefile in the folder `ga_2022_gen_st_prec` from the [2022 General Senate Results](https://redistrictingdatahub.org/dataset/georgia-2022-general-election-precinct-level-results-and-boundaries/) because the runoff election did not include precinct geometries.

Then, I added used race demographic data at the block level from the [2020 Census Data](https://data.census.gov/table/DECENNIALPL2020.P1?q=P1&g=040XX00US13$1000000) which I joined with block shapefile data from [Tiger/Shapefiles website](https://www.census.gov/cgi-bin/geo/shapefiles/index.php).

After joining all the data together and dealing with NaN values, I analyzed a random walk starting at a random initial plan. The walk showed that 6 democratic districts is most likely to occur as seen below. However, both 2021 and 2023 had 5 democratic districts, so it seems like the plans were also partisanly gerrymandered.

[]('/graphics/random-init-democrat-likelihood.png')

For black majority districts, I found that 4 districts is most likely but 5 districts is super close as seen below. Meanwhile, there were 3 black majority districts in the 2021 plan and 4 black majority districts in 2023's plan. So it seems like the 2021 was definently racially gerrymandered, however, the 2023 could go either way since the ensemble demonstrated that 4 black-majority districts was basically as likely as 5 districts.

[]('/graphics/rand-initi-black-maj.png')

To confirm that I ran the random walk for long enough, I ran a random walk from both the 2021 plan and the 2023 plan to compare their results to the random walk from a random initial plan. Below is a boxplot comparing the black population across districts from all three random walks as well as a boxplot comparing the democratic voter population across districts.

[]('/black-pop-all-rws.png')

[]('/dem-dist-all-rws.png')

The distribution for each random walk at each district looks similar, so the random walks ran for enough time.

I also ran a random walk from the same random initial plan but for 20,000 steps instead of 10,000 steps. The boxplots comparing the population distributions are below.

[]('/bpop-steps.png')

[]('/dem-steps.png')

Since the distributions are similar between the 10,000 step and 20,000 step random walk, I condlude the random walk with 10,000 steps from which I did my analysis ran for long enough and explored the state space fully.


Information on court cases:
- https://thearp.org/litigation/pendergrass-v-raffensperger/
- https://thearp.org/litigation/georgia-state-conf-naacp-v-georgia/
- https://thearp.org/litigation/common-cause-v-raffensperger/
- https://apnews.com/article/georgia-redistricting-house-senate-congress-lucy-mcbath-9ab4476a3877656867fc8a46a14c95ee
