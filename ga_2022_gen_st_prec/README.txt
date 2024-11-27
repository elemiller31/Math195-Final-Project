Georgia 2022 General Election Precinct Boundary and Election Results

## RDH Date Retrieval
05/31/23

## Sources
The RDH retrieved 2022 general election precinct-level results from the Georgia Secretary of State [website] (https://results.enr.clarityelections.com/GA/115465/web.307039/#/summary). The RDH navigated to each county's election results page and clicked "Detail XML", to get the results at the precinct level.

Precinct shapefile primarily from the [Legislative and Congressional Reapportionment Office of the Georgia General Assembly](https://www.legis.ga.gov/joint-office/reapportionment) ["Statewide Voting Precincts (2022)"](https://www.legis.ga.gov/api/document/docs/default-source/reapportionment-document-library/ga-precincts2022-shape.zip?sfvrsn=7844a3b6_2). Modifications were made to precinct boundaries after consulting a 2022 Georgia Voterfile via L2 retrieved from the state on 2/2/2023. Lamar and Liberty county precinct data is sourced directly from the respective counties. That and additional changes are detailed below:

Appling: Edits made to precincts '1C', '3C', '4D', '5B' based on voterfile
Calhoun: Edits made to precincts 'EDISON', 'EDISON-ARLINGTON', 'LEARY', 'MORGAN' based on voterfile
Chatham: Ten precincts split by municipal boundary lines for Garden City and Savannah to match election results. The smaller of the two "7-11C Savannah Fire Station 14" precincts was combined with "8-18C Savannah First 7th Day Adv Church".
Cherokee: Edits made to precincts 'BOOTH' and 'ROSECREEK' based on voterfile
Dooly: Edits made to precincts 'LILLY', 'PINEHURST', and 'VIENNA' based on voterfile
Douglas: Edits made to precincts 'EPHESUS BAPTIST CHURCH', 'MIRROR LAKE ELEMENTARY' based on voterfile
Fulton: Added precinct "121-SS07D" using county map (https://www.fultoncountyga.gov/-/media/Departments/IT_GIS/Printable-Maps/2022-Maps/VotingPrecinctsNorth_ep_v2.ashx)
Gilmer: Edits made to precincts 'CARTECAY', 'MOUNTAINTOWN', 'ROY ROAD', 'TAILS CREEK' based on voterfile
Habersham: Added the "City of Baldwin" precinct by intersecting municipal boundary with Habersham South precinct
Hancock: Edits made to precincts COURTHOUSE', 'DEVEREUX FIRE', 'SECOND BEULAH', 'SECOND DARRIEN', 'WARREN CHAPEL', 'YOUTH CENTER' based on voterfile
Haralson: Edits made to 'BEREA-STEADMAN' and 'LITTLE CREEK' based on voterfile
Jones: Edits made to 'ETHRIDGE', 'GRAY' based on voterfile
Lamar: Precincts sourced from precinct information on County Commission and Schoolboard map 
Liberty: Precincts sourced from county shapefile (https://libertycountyga.maps.arcgis.com/apps/webappviewer/index.html?id=0adfbb2fe1c044ecab18fb405c96939f)
Lincoln: Edits made to precincts 'FAITH TEMPLE OF LINCOLN', 'LINCOLN CENTER', 'LINCOLN CLUB HOUSE', 'MARTINS CROSSROAD', and 'TABERNACLE' based on voterfile
Long: Edits made to precincts 'ALMA FLOURNOY', 'BREADS CREEK', 'FAITH BAPTIST ANNEX', 'NORTH LUDOWICI', 'RYE PATCH_OAK DALE', 'SOUTH LUDOWICI', 'TIBET' based on voterfile
Macon: Edits made to precincts 'IDEAL','MARSHALLVILLE','MONTEZUMA #4','MONTEZUMA #5','OGLETHORPE' based on voterfile 
McIntosh: Edits made to precincts 'CRESCENT', 'DARIEN', 'NORTH DARIEN', 'SOUTH NEWPORT' based on voterfile
Pickens: Edits made to precincts 'APPALACHIAN', 'SHARPTOP', 'TALKING ROCK', 'YELLOW CREEK' based on voterfile
Worth: Edits made to precincts 'BRIDGEBORO', 'COUNTY LINE', 'POULAN', 'SYLVESTER EAST' based on voterfile


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
A## - Constitutional Amendment 
AGR - Commissioner of Agriculture
ATG - Attorney General
GOV - Governor
INS - Commissioner Of Insurance
LAB - Commissioner Of Labor
LTG - Lieutenant Governor
RF# - Statewide Referendum
SOS - Secretary Of State
SUP - State School Superintendent
USS - U.S. Senate
CON## - U.S. Congress
SL###  - State Legislative Lower
SU##  - State Legislative Upper

## Fields:
Field Name Description
UNIQUE_ID  Unique ID for each precinct                
COUNTYFP   County FIP identifier                      
county     County Name                                
precinct   Precinct Name    

***ga_2022_gen_st_prec*** 
G22A01NO   No Constitutional Amendment #1              
G22A01YES  Yes / Sí Proposed Constitutional Amendment 1
G22A02NO   No Constitutional Amendment #2              
G22A02YES  Yes / Sí Proposed Constitutional Amendment 2
G22AGRDHEM Nakita Hemingway                           
G22AGRLRAU David Raudabaugh                           
G22AGRRHAR Tyler Harper                               
G22ATGDJOR Jennifer ""Jen"" Jordan                    
G22ATGLCOW Martin Cowen                               
G22ATGRCAR Chris Carr                                 
G22GOVDABR Stacey Abrams                              
G22GOVLHAZ Shane Hazel                                
G22GOVRKEM Brian Kemp                                 
G22INSDROB Janice Laws Robinson                       
G22INSRKIN John King                                  
G22LABDBOD William ""Will"" Boddie, Jr                
G22LABLAND Emily Anderson                             
G22LABRTHO Bruce Thompson                             
G22LTGDBAI Charlie Bailey                             
G22LTGLGRA Ryan Graham                                
G22LTGRJON Burt Jones                                 
G22RFANO   No Proposed Statewide Referendum 1          
G22RFAYES  Yes / Sí Proposed Statewide Referendum 1    
G22RFBNO   No Proposed Statewide Referendum 2          
G22RFBYES  Yes / Sí Proposed Statewide Referendum 2    
G22SOSDNGU Bee Nguyen                                 
G22SOSLMET Ted Metz                                   
G22SOSRRAF Brad Raffensperger                         
G22SUPDSEA Alisha Thomas Searcy                       
G22SUPRWOO Richard Woods                              
G22USSDWAR Raphael Warnock                            
G22USSLOLI Chase Oliver                               
G22USSRWAL Herschel Junior Walker  
  

## Processing Steps
Visit the RDH GitHub and the processing script for this code [here](https://github.com/nonpartisan-redistricting-datahub/pber_collection).

## Additional Notes
Files were checked against separate statewide and countywide election result files also available from the Georgia Secretary of State. Results matched exactly except for differences in the following races (G22A01NO, G22A01YES, G22A02NO, G22A02YES, G22RFBNO, G22RFBYES) in Emanuel County. For these races in Emanuel County, the statewide and countywide election result files we compared against contained no votes.

Please note that although we produced this file to be as accurate as possible, we may come across additional information in the future which may require us to update this file.

A handful of changes were made to the statewide voting precincts file. Initially, there were 12 precincts with election results that did not appear in the precinct shapefile. 10 of these precincts were in Chatham County and created by intersecting existing precincts with municipal boundaries. The other two precincts were "SS07D" in Fulton County and "CITY OF BALDWIN" in Habersham County. The precinct in Fulton was created by hand from looking at a precinct map. The City of Baldwin precinct was confirmed by a news article and created by taking the intersection of an existing precinct and a municipal boundary.

Some precincts are split across Congressional, House of Representatives or State Senate Districts. In these cases, the precincts can be split into the particular areas contained in each district using a district shapefile and one can give the votes for the candidates in those particular districts to that district's portion of the precinct. This extra step makes block-level disaggregation and RPV analyses more accurate. For races outside of those particular districts, one does not know the proportion of votes to allot to each district-precinct chunk. As such, separate files are created to ensure the accuracy of votes. Because there were splits for Congress, House of Representatives and State Senate Districts, files for each of these levels, as well as for statewide elections, were created. 

In some cases, a precinct may have votes for multiple districts, but does not spatially intersect with all districts for which it contains votes. This could either be evidence that a precinct's boundaries are incorrect, or simply an instance in which a voter either voted or had their vote counted at the incorrect precinct. For the level-specific files mentioned above, we look into the precinct shapefiles and, unless we find a particular precinct boundary to change, these votes are dropped. For details on the exact number of votes dropped, please see the Jupyter Notebook linked above.

There is also a "ga_2022_gen_prec_no_splits" file, which contains all election results, but does not include a SLDL_DIST, SLDU_DIST or CONG_DIST column.

Modifications using the voterfile in Cherokee, Lincoln, Long, Pickens and Worth counties were compared against precinct files available from the county. In these instances, changes based on the voterfile were kept in place as it appeared that the county's information was not updated. In the other counties where changes based on the voterfile were made, precinct files from the county were not available. 

The file can be joined against the 2022 Georgia Precinct file linked above to compare the changes above.


Please direct questions related to processing this dataset to info@redistrictingdatahub.org.
