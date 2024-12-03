Georgia 2022 Runoff Election Precinct-Level Results

## RDH Date Retrieval
01/31/23

## Sources
The RDH retrieved 2022 runoff election precinct-level results from the Georgia Secretary of State [website] (https://results.enr.clarityelections.com/GA/116564/web.307039/#/summary). The RDH navigated to each county's election results page and clicked "Detail XML", to get the results at the precinct level.

## Notes on Field Names (adapted from VEST):
Columns reporting votes generally follow the pattern: 
One example is:
G16PREDCLI
The first character is G for a general election, P for a primary, S for a special, and R for a runoff.
Characters 2 and 3 are the year of the election.*
Characters 4-6 represent the office type (see list below).
Character 7 represents the party of the candidate.
Characters 8-10 are the first three letters of the candidate's last name.

*To fit within the GIS 10 character limit for field names, the naming convention is slightly different for the State Legislature and US House of Representatives. All fields are listed below with definitions.

Office Codes Used:
USS - U.S. Senate


## Fields:
Field Name Description
UNIQUE_ID  Unique ID for each precinct                
COUNTYFP   County FIP identifier                      
county     County Name                                
precinct   Precinct Name
R22USSDWAR Raphael Warnock                            
R22USSRWAL Herschel Junior Walker                      
                             

## Processing Steps
Visit the RDH GitHub and the processing script for this code [here](https://github.com/nonpartisan-redistricting-datahub/pber_collection)

## Additional Notes
Files were checked against separate statewide and countywide election result files also available from the Georgia Secretary of State. Results matched exactly.

Please direct questions related to processing this dataset to info@redistrictingdatahub.org.
