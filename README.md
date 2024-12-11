# An Ensemble Analysis: How Gerrymandering Changed the 2024 Election
By Elena Miller and Anne Friedman

## Introduction

In the 2024 U.S. House of Representatives Election, the Republicans won 220 seats and the Democrats won 215 seats, securing the House for the Republicans. Currently, there are nine states with congressional districting plans in litigation, meaning current court cases are arguing that the maps are a racial or partisan gerrymander. Thus, we were curious if the election could have had a different outcome if these nine states had fair maps. We conducted an analysis to determine if the impact of these disputed districts could have changed control of Congress.

To do this, we used statewide elections for the Governor, U.S. Senator, and U.S. President to gauge voters' partisanship. To ensure that our process was similar across all nine states, we chose not to use U.S. House of Representative election data. This is because candidates tend to vary in quality and views across each district, meaning that a voter's choices in one election might not necessarily be their overall preference. Instead, a statewide election with more consistent candidates allows us to understand preferences across the entire population.

Additionally, we focused only on Democratic and Republican votes for the particular election we used. In no state was an independent candidate selected, so we did not feel it necessary to include that data in our analysis. After finding our data on election results and Census data, we downloaded shapefiles for the current congressional districting maps. We then compared each district with the Democratic and Republican votes to determine how many seats each party won in that state. Finally, we created a Markov Chain from various starting points (and running for various lengths) to find the most likely distribution of seats for each party. We concluded that this outcome would be the most likely outcome for each state if they had a ‘fair’ map. 

In this report, we will first detail our process and conclusions for each of the nine states: Georgia, Texas, Utah, South Carolina, North Carolina, Florida, Louisiana, Arkansas, and Alabama. For each state, we will provide a brief background of the litigation, our analysis of the Markov chain, an argument that the Markov Chain has reached its stationary distribution, some limitations of the data, and how a “fair” map would have changed the outcome of the 2024 US House of Representatives election.

## Conclusion

To reiterate, in the actual 2024 election, the Republicans won 220 seats in the U.S. House of Representatives, and the Democrats won 215 seats.

According to our Ensemble Analysis, Democrats might have won the House in the 2024 election. The Republican party would have lost three seats, reducing their number of seats to 217. Similarly, The Democratic party would have gained three seats, increasing their number of seats to 218. Since a party needs at least 218 seats to hold the majority, the Democratic Party would have held the majority. However, this claim does rely on our ensemble analysis being entirely accurate, which is something that we can not prove. 

In a future report, we would like to use the 2024 Election Data. Because we had to use 2020 and 2022 Election Data, there is some concern that voters’ preferences have shifted in the past two/four years. Similarly, we had to use data from the 2020 Census, which assumes that people have not moved in the past four years. Although there is no easy way to accurately fix the problem with our Census data, we can fix our problem with the Voting Data by simply using 2024 data. At the time of this report, the 2024 Election data was not out for most of the nine states, and to ensure consistency across states we elected not to use this data.


## Works Cited
### For All States:
Census Data: https://data.census.gov/

Block-To-Precinct Data: https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2022&layergroup=Blocks+%282020%29

Election Information:
https://www.theguardian.com/us-news/2024/dec/04/democrat-adam-gray-wins-california-house-election-against-republican-john-duarte

### Alabama:
Election Results: https://redistrictingdatahub.org/dataset/alabama-2022-general-election-precinct-level-results-and-boundaries/

Congressional Districts:
https://redistrictingdatahub.org/dataset/2021-alabama-congressional-districts-adopted-plan/
https://redistrictingdatahub.org/dataset/2023-alabama-congressional-districts-plan-approved/

Litigation Research:
https://thearp.org/litigation/singleton-v-merrill/
https://www.al.com/election/2024/11/after-defeat-alabama-republicans-look-to-revisit-states-congressional-map.html
https://www.npr.org/2024/04/15/1244164194/black-voters-representation-alabama-redistricting
https://apnews.com/article/supreme-court-redistricting-alabama-voting-rights-act-114ba2e144d903efc77ad31fe40ee47f

### Arkansas:
Election Results: https://redistrictingdatahub.org/dataset/arkansas-2020-general-election-results-disaggregated-to-the-2020-block/

Congressional Districts:
https://redistrictingdatahub.org/dataset/2021-arkansas-congressional-districts-2/
https://redistrictingdatahub.org/dataset/arkansas-congressional-districts-2011-to-2021/

Litigation Research:
https://www.naacpldf.org/press-release/ldf-advocates-for-arkansas-congressional-redistricting-lawsuit-to-go-to-trial/
https://arkansasadvocate.com/2024/12/02/three-judge-panel-hears-arguments-but-doesnt-rule-in-arkansas-redistricting-lawsuit/
https://www.npr.org/2024/07/04/nx-s1-5025758/voting-rights-act-arkansas-supreme-court-section-1983

### Georgia:

Election Results: 

Congressional Districts:

Litigation Research:
https://thearp.org/litigation/pendergrass-v-raffensperger/
https://thearp.org/litigation/georgia-state-conf-naacp-v-georgia/
https://thearp.org/litigation/common-cause-v-raffensperger/
https://apnews.com/article/georgia-redistricting-house-senate-congress-lucy-mcbath-9ab4476a3877656867fc8a46a14c95ee
https://www.wabe.org/georgias-ongoing-redistricting-challenge-explained/

### Florida:
Election Results: https://redistrictingdatahub.org/dataset/florida-2022-general-election-precinct-level-results-and-boundaries/

Congressional Districts: https://www.floridaredistricting.gov/

Litigation Research:
https://www.npr.org/2024/09/11/nx-s1-5106385/florida-redistricting-case-fair-districts
https://www.brennancenter.org/our-work/research-reports/redistricting-litigation-roundup-0
https://www.flsenate.gov/session/redistricting

### Louisiana:
Election Results: https://redistrictingdatahub.org/dataset/louisiana-2022-general-election-precinct-level-results/

Congressional Districts: https://redist.legis.la.gov/

Litigation Research:
https://lailluminator.com/2024/11/04/supreme-court-takes-up-challenge-to-louisiana-congressional-map/
https://www.scotusblog.com/2024/11/supreme-court-will-hear-case-on-second-majority-black-district-in-louisiana-redistricting/
https://www.cbsnews.com/news/supreme-court-to-hear-louisiana-congressional-map-case-two-majority-black-districts/
https://www.npr.org/2024/05/15/1250937356/supreme-court-louisiana-redistricting
### North Carolina: 
Election Results: https://redistrictingdatahub.org/dataset/north-carolina-2022-general-election-precinct-level-results-and-boundaries/

Congressional Districts: https://www.ncleg.gov/redistricting

Litigation Research:
https://apnews.com/article/north-carolina-congressional-redistricting-lawsuit-ba9e21540021c792e942ef4f166f02cc
https://www.brennancenter.org/our-work/research-reports/redistricting-litigation-roundup-0
https://www.carolinajournal.com/federal-nc-redistricting-lawsuits-officially-scheduled-for-june-2025-trial/
https://carolinapublicpress.org/66873/why-have-nc-congressional-districts-changed-for-2024/
https://www.cnn.com/2023/12/05/politics/north-carolina-congressional-map-lawsuit/index.html

### South Carolina:

Election Results: https://redistrictingdatahub.org/dataset/south-carolina-2022-general-election-precinct-level-results-and-boundaries/

Congressional Districts: https://redistricting.scsenate.gov/currentdistricts.html

Litigation Research: 
https://thearp.org/litigation/sc-state-conf-naacp-v-mcmaster/
https://www.aclusc.org/en/press-releases/aclu-and-lwv-file-lawsuit-against-partisan-gerrymandering-south-carolinas

### Texas:
Election Results: https://election.lab.ufl.edu/dataset/tx-2020-precinct-level-election-results/

Congressional Districts: https://data.capitol.texas.gov/dataset/planc2193

Litigation Research: 
https://thearp.org/litigation/?c=congressional-redistricting,texas https://redistricting.lls.edu/cases/?states%5B%5D=Texas&levels%5B%5D=Congress&sortby=-updated&page=1
https://www.texastribune.org/2022/11/08/ken-paxton-rochelle-garza-attorney-general/

### Utah:
Election Results: https://election.lab.ufl.edu/dataset/ut-2020-precinct-level-election-results/

Congressional Districts: https://citygate.utleg.gov/legdistricting/utah/comment_links#

Litigation Research: 
https://redistricting.lls.edu/case/lwv-of-utah-v-utah-state-legislature/
https://apnews.com/article/utah-supreme-court-redistricting-lawsuit-a3bc251ded9dfe4a75b48c79fece0a86
https://utahnewsdispatch.com/2024/07/11/gerrymandering-case-utah-supreme-court-rules-against-legislatures-ballot-initiative-override/
https://thearp.org/litigation/league-women-voters-utah-v-utah-state-legislature/




