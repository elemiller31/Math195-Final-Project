Louisiana 2022 General Election Precinct Boundaries and Election Results

## RDH Date Retrieval
07/11/23

## Sources
The RDH retrieved 2022 general election results from the Louisiana Secretary of State. General election results are available [here](https://voterportal.sos.la.gov/static/2022-11-08). Precinct shapefiles are from the Louisiana Legislative Redistricting [website](https://redist.legis.la.gov/default_ShapeFiles2020).

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
A# - Constitutional Amendment 
USS - U.S. Senate
CON## - U.S. Congress
SU##  - State Legislative Upper (pre-2021 redistricting cycle)

## Fields:
Field Name Description
UNIQUE_ID  Unique ID for each precinct              
COUNTYFP   County FIP identifier                    
Parish     Parish Name                              
Precinct   Precinct Name                            
CONG_DIST  Congressional District                   
SLDU_DIST  State Senate District (pre-2021 redistricting cycle)                 
G22A1NO    NO-:-CA No. 1              
G22A1YES   YES-:-CA No. 1             
G22A2NO    NO-:-CA No. 2              
G22A2YES   YES-:-CA No. 2             
G22A3NO    NO-:-CA No. 3              
G22A3YES   YES-:-CA No. 3             
G22A4NO    NO-:-CA No. 4              
G22A4YES   YES-:-CA No. 4             
G22A5NO    NO-:-CA No. 5              
G22A5YES   YES-:-CA No. 5             
G22A6NO    NO-:-CA No. 6              
G22A6YES   YES-:-CA No. 6             
G22A7NO    NO-:-CA No. 7              
G22A7YES   YES-:-CA No. 7             
G22A8NO    NO-:-CA No. 8              
G22A8YES   YES-:-CA No. 8             
G22USSDCHA Gary Chambers, Jr.         
G22USSDMEN MV "Vinny" Mendoza         
G22USSDMIX "Luke" Mixon               
G22USSDROD Salvador P. Rodriguez      
G22USSDSTE Syrita Steib               
G22USSIMCM Bradley McMorris           
G22USSLSIG Aaron C. Sigler            
G22USSNBIL Beryl A. Billiot           
G22USSNOLS W. Thomas La Fontaine Olson
G22USSOJOH "Xan" John                 
G22USSOWEN Thomas Wenn                
G22USSRGRA Devin Lance Graham         
G22USSRKEN John Kennedy               
GCON01DDAR Katie Darling              
GCON01LKEA Howard Kearney             
GCON01RSCA Steve Scalise              
GCON02DCAR Troy A. Carter             
GCON02RLUX "Dan" Lux                  
GCON03DLEB Tia LeBrun                 
GCON03DOLI Lessie OliviaLeblanc       
GCON03IWIG Gloria R. Wiggins          
GCON03LMCL Guy McLendon               
GCON03RHIG Clay Higgins               
GCON03RHOG Holden Hoggatt             
GCON03RPAY Thomas "Lane" Payne, Jr.   
GCON03RSHA Jacob "Jake" Shaheen       
GCON05DDAN Oscar "Omar" Dantzler      
GCON05DHUF Walter Earl Huff           
GCON05RGUI Allen Guillory             
GCON05RLET Julia Letlow               
GCON05RPUL Hunter Pullen              
GCON06LCRA Rufus Holt Craig, Jr.      
GCON06RBEL Brian Belzer               
GCON06RGRA Garret Graves              
SSU05DDUP  Royce Duplessis            
SSU05DLAN  Mandie Landry              
SSU17DLAC  Jeremy S. LaCombe          
SSU17RKLE  Caleb Seth Kleinpeter      
SSU17RROU  Kirk Rousset               
          
## Processing Steps
Visit the RDH GitHub and the processing script for this code [here](https://github.com/nonpartisan-redistricting-datahub/pber_collection)

## Additional Notes
Please note the slight change to the naming convention to differentiate between Tia LeBrun and Lessie Olivia Leblanc. Statewide election result totals for each race were compared against those results available at the statewide level on the Louisiana Secretary of State [website](https://voterportal.sos.la.gov/static/2022-11-08). Statewide totals matched across all races.

Ascension, Assumption, Bossier, Caddo, East Baton Rouge, Lafourche, Rapides, St. Charles, and Terrebonne parishes break down election results in at least some precincts by the last name of voters. These precincts are combined so the results can be joined to a shapefile.

The race for Congressional District 4 was uncontested and as such, no precincts in that district contain congressional votes. Any precincts without Congressional votes have been assigned a Congressional district using the geometries of the districts and precincts. The State Senate results in this election were special elections on the pre-redistricting boundaries for two seats, 5 and 17. All precincts without votes for these races have an "SLDL_DIST" value of "N/A".

Please direct questions related to processing this dataset to info@redistrictingdatahub.org.
