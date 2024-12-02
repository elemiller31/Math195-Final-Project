Texas Legislative Council
Research Division
Capitol Data Portal https://data.capitol.texas.gov

Election data are developed and compiled by the Research Division of the
Texas Legislative Council for redistricting purposes.


ELECTION DATA

The election data contained within this directory are derived from election
returns provided by the counties and the office of the secretary of state.

The United States Census Bureau published geographic units used for tabulation of
the 2020 Census population data in the 2020 TIGER/Line Shapefile.  The geographic
units, which remain constant throughout the decade, include counties, census tracts,
block groups, and blocks.

Election data is reported by election precincts, which frequently change and may
not conform to census geographical units.  Council staff work with the counties
throughout the decade to maintain a statewide precinct geographic database for each
election.  

Voting Tabulation Districts (VTDs), the census geographic equivalent of county
election precincts, are created for the purpose of relating 2020 Census population
data to election precinct data.  VTDs can differ from actual election precincts
because precincts do not always follow census geography.  The VTDs in the
redistricting database closely correspond to the 9,586 precincts in effect for the
2022 general election.  On the occasion that a precinct is in two noncontiguous pieces,
it is a suffixed VTD in the database.  For example, if precinct 0001 had two non-contiguous
areas, the corresponding VTD would be VTD 0001A and VTD 0001B.  If a 2022 general 
election precinct does not match any census geography, it is consolidated with an 
adjacent precinct and given that precinct's corresponding VTD number.

For more information, consult the Texas Redistricting Website: 
https://redistricting.capitol.texas.gov/publications.


The election data for all current and past elections in this directory are reported 
by 2022 general election VTDs, which are composed of 2020 Census blocks.

GIS users can join the election data to the 2022 general election VTDs Shapefile
located at https://data.capitol.texas.gov/dataset/vtds.  Use the
common field name 'VTDKEY' to join the data.



HOW TO USE THE DATA:

There are two comma-separated values (.csv) files for each election:
  - One file contains returns and has a file name reflecting the election year and type, 
    such as "2012_General_Election_Returns.csv".  

  -The second file contains voter registration (VR) and turnout (TO) data for each election, 
   and has a file name reflecting VR and TO, such as "2012_General_Election_VRTO.csv".

The returns files contain the following fields:

County (txt) - county name
FIPS (num) - county FIPS code
vtdkey (num) - Unique code used to join to geographic data.
VTD (txt) - VTD name (2022 General Election)
Office (txt) - office name
Name (txt) - candidate name
Party (txt) - party identifier
Incumbent (txt) - incumbent identifier
Votes (num) - election returns

The voter registration and turnout files contain the following fields:
County (txt) - county name
FIPS (num) - county FIPS code
VTD (txt) - VTD name (2022 General Election)
vtdkey (num) - Unique code used to join to geographic data.
TotalPop (num) - 2020 census total population
TotalVR (num) - voter registration (includes suspense and non-suspense VR)
SpanishSurnamePercent (txt) - percent Spanish surname voter registration
TotalTO (num) - turnout


Note 1:  Users of this data prior to 2010 may notice that the voter registration data 
has changed.  Before 2011, council election data reflected non-suspense voter 
registration only.  Beginning in 2011, council election data for all years reflects 
total voter registration, the sum of non-suspense and suspense voter registration.


Last modified on January, 20, 2023.