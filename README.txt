Florida 2022 General Election Precinct Boundary and Election Results

## RDH Date Retrieval
12/20/23


## Sources
Elections results from [Florida Division of Elections](https://dos.myflorida.com/elections/data-statistics/elections-data/precinct-level-election-results/)

Precinct shapefiles for the following counties sourced from the respective county Supervisor of Elections: Alachua, Charlotte, Glades, Hillsborough, Palm Beach, Brevard, Citrus, Clay, Collier, Dade, Flagler, Lee, Marion, Nassau, Osceola, St. Lucie, Sumter, Escambia, Orange.

Precinct shapefiles for the following counties sourced from VEST's 2020 precinct shapefile: Baker, Bradford, Calhoun, DeSoto, Dixie, Franklin, Gadsden, Gilchrist, Gulf, Hamilton, Hardee, Highlands, Holmes, Jackson, Jefferson, Lafayette, Levy, Liberty, Madison, Martin, Monroe, Okaloosa, Okeechobee, Santa Rosa, Suwannee, Taylor, Union, Wakulla, Walton, Washington. 

Precinct shapefiles for the following counties sourced from a map compiled by RDH volunteer Sebastian Pojman: Bay, Broward, Columbia, Duval, Hendry, Hernando, Indian River, Lake, Leon, Manatee, Pasco, Pinellas*, Polk, Putnam, Sarasota, Seminole*, St. Johns, Volusia.

*These two counties are from a revised version of the map.


## Notes on Field Names (adapted from VEST):
Columns reporting votes generally follow the pattern: 
One example is:
G16PRERTRU
The first character is G for a general election, P for a primary, S for a special, and R for a runoff.
Characters 2 and 3 are the year of the election.*
Characters 4-6 represent the office type (see list below).
Character 7 represents the party of the candidate.
Characters 8-10 are the first three letters of the candidate's last name.

*To fit within the GIS 10 character limit for field names, the naming convention is slightly different for the State Legislature and US House of Representatives. All fields are listed below with definitions.

Office Codes Used:
A## - Constitutional Amendment 
ATG - Attorney General
CFO - Chief Financial Officer
COA - Commissioner of Agriculture
GOV - Governor
SCJ - Supreme Court Justice*
USS - U.S. Senate
CON## - U.S. Congress
SL###  - State Legislative Lower
SU##  - State Legislative Upper

Party Codes Used:
D - Democratic
R - Republican
L - Libertarian
G - Green
C - Constitution
N - No Party Affiliation

*SCJ races, which are nonpartisan, treated differently.
Y - Yes
N - No


## Fields
Field Name	Description
UNIQUE_ID	Unique ID for each precinct                                                                                                         
COUNTYFP	County FIP identifier
CNTY_CODE	Three-letter code for county name                                                                                                               
CNTY_NAME	Full county name                                                                                                                         
PREC_ID		Precinct ID number within county
POLL_LOC	Name of polling location

***fl_2022_gen_st_prec***
G22A1NO    Amendment No. 1: Limitation on Assessment of Real Property Used for Residential Purposes No for Rejection                     
G22A1YES   Amendment No. 1: Limitation on Assessment of Real Property Used for Residential Purposes Yes for Approval                     
G22A2NO    Amendment No. 2: Abolishing the Constitution Revision Commission No for Rejection                                             
G22A2YES   Amendment No. 2: Abolishing the Constitution Revision Commission Yes for Approval                                             
G22A3NO    Amendment No. 3: Additional Homestead Property Tax Exemption for Specified Critical Public Services Workforce No for Rejection
G22A3YES   Amendment No. 3: Additional Homestead Property Tax Exemption for Specified Critical Public Services Workforce Yes for Approval
G22ATGDAYA Attorney General Aramis Ayala                                                                                                 
G22ATGRMOO Attorney General Ashley Moody                                                                                                 
G22CFODHAT Adam Hattersley                                                                                       
G22CFOOWRI WriteinVotes                                                                                          
G22CFORPAT Jimmy Patronis                                                                                        
G22COADBLE Naomi Esther Blemur                                                                               
G22COARSIM Wilton Simpson                                                                                    
G22GOVDCRI Crist / Hernandez                                                                            
G22GOVLROO Roos / Rorabaugh                                                                             
G22GOVNGIM Gimenez / Gibson                                                                          
G22GOVOWRI WriteinVotes                                                                                 
G22GOVRDES DeSantis / Nuñez                                                                             
G22SCJNCAN Retention of Charles T. Canady No                                                                                             
G22SCJNCOU Retention of John D. Couriel No                                                                                               
G22SCJNGRO Retention of Jamie Grosshans No                                                                                               
G22SCJNLAB Retention of Jorge Labarga No                                                                                                 
G22SCJNPOL Retention of Ricky Polston No                                                                                                 
G22SCJYCAN Retention of Charles T. Canady Yes                                                                                            
G22SCJYCOU Retention of John D. Couriel Yes                                                                                              
G22SCJYGRO Retention of Jamie Grosshans Yes                                                                                              
G22SCJYLAB Retention of Jorge Labarga Yes                                                                                                
G22SCJYPOL Retention of Ricky Polston Yes                                                                                                
G22USSDDEM Val Demings                                                                                             
G22USSLMIS Dennis Misigoy                                                                                          
G22USSNGRA Steven B. Grant                                                                                      
G22USSNNGU Tuan TQ Nguyen                                                                                       
G22USSOWRI WriteinVotes                                                                                            
G22USSRRUB Marco Rubio

***fl_2022_gen_cong_prec***
CONG_DIST  Florida Congressional District 
GCON01DJON Rebekah Jones                                                                                      
GCON01RGAE Matt Gaetz                                                                                         
GCON02DLAW Al Lawson                                                                                          
GCON02RDUN Neal Dunn                                                                                          
GCON03DHAW Danielle Hawk                                                                                      
GCON03NBRO Linda S. Brooks                                                                                 
GCON03RCAM Kat Cammack                                                                                        
GCON04DHOL LaShonda "L.J." Holloway                                                                           
GCON04OWRI WriteinVotes                                                                                       
GCON04RBEA Aaron Bean                                                                                         
GCON06LHAN Joseph "Joe" Hannoush                                                                              
GCON06RWAL Michael Waltz                                                                                      
GCON07DGRE Karen Green                                                                                        
GCON07OWRI WriteinVotes                                                                                       
GCON07RMIL Cory Mills                                                                                         
GCON08DTER Joanne Terry                                                                                       
GCON08RPOS Bill Posey                                                                                         
GCON09DSOT Darren Soto                                                                                        
GCON09RMOO Scotty Moore                                                                                       
GCON10DFRO Maxwell Alejandro Frost                                                                            
GCON10NHOL Jason Holic                                                                                     
GCON10NJAI Usha Jain                                                                                       
GCON10RWIM Calvin B. Wimbish                                                                                  
GCON11DMUN Shante Munns                                                                                       
GCON11NPOR Kevin Porter                                                                                    
GCON11RWEB Daniel Webster                                                                                     
GCON12DWAL Kimberly Walker                                                                                    
GCON12OWRI WriteinVotes                                                                                       
GCON12RBIL Gus Michael Bilirakis                                                                              
GCON13DLYN Eric Lynn                                                                                          
GCON13LCRA Frank Craft                                                                                        
GCON13OWRI WriteinVotes                                                                                       
GCON13RLUN Anna Paulina Luna                                                                                  
GCON14DCAS Kathy Castor                                                                                       
GCON14RJUD James Judge                                                                                        
GCON15DCOH Alan M. Cohn                                                                                       
GCON15RLEE Laurel Lee                                                                                         
GCON16DSCH Jan Schneider                                                                                      
GCON16OWRI WriteinVotes                                                                                       
GCON16RBUC Vern Buchanan                                                                                      
GCON17DKAL Andrea Doria Kale                                                                                  
GCON17NMUR Theodore "Pink Tie" Murray                                                                      
GCON17RSTE Greg Steube                                                                                        
GCON18NHAY Keith R. Hayden Jr                                                                              
GCON18OWRI WriteinVotes                                                                                       
GCON18RFRA Scott Franklin                                                                                     
GCON19DBAN Cindy Banyai                                                                                       
GCON19OWRI WriteinVotes                                                                                       
GCON19RDON Byron Donalds                                                                                      
GCON20DCHE Sheila Cherfilus-McCormick                                                                         
GCON20RCLA Drew Montez Clark                                                                                  
GCON21DBAL Corinna Balderramos Robinson                                                                       
GCON21RMAS Brian Mast                                                                                         
GCON22DFRA Lois Frankel                                                                                       
GCON22RFRA Dan Franzese                                                                                       
GCON23DMOS Jared Moskowitz                                                                                    
GCON23NNAP Mark Napier                                                                                     
GCON23NSCO Christine Scott                                                                                 
GCON23RBUD Joe Budd                                                                                           
GCON24DWIL Frederica Wilson                                                                                   
GCON24RNAV Jesus G. Navarro                                                                                   
GCON25DSCH Debbie Wasserman Schultz                                                                           
GCON25RSPA Carla Spalding                                                                                     
GCON26DOLI Christine Alexandria Olivo                                                                         
GCON26RDIA Mario Diaz-Balart                                                                                  
GCON27DTAD Annette Taddeo                                                                                     
GCON27RSAL María Elvira Salazar                                                                               
GCON28DASE Robert Asencio                                                                                     
GCON28OWRI WriteinVotes                                                                                       
GCON28RGIM Carlos A. Gimenez

***fl_2022_gen_sldu_prec***
SLDU_DIST  Florida State Senate District 
GSU01DNIC  Charlie Nichols                                                                                                 
GSU01RBRO  Doug Broxson                                                                                                    
GSU02DZON  Carolynn Zonia                                                                                                  
GSU02RTRU  Jay Trumbull                                                                                                    
GSU03DAUS  Loranne Ausley                                                                                                  
GSU03RSIM  Corey Simon                                                                                                     
GSU04DSMI  Sharmin Smith                                                                                                   
GSU04RYAR  Clay Yarborough                                                                                                 
GSU05DDAV  Tracie Davis                                                                                                    
GSU05OWRI  WriteinVotes                                                                                                    
GSU05RKUM  Binod Kumar                                                                                                     
GSU08DWIL  Andrea Williams                                                                                                 
GSU08RWRI  Tommy A. Wright                                                                                                 
GSU09DLON  Rodney Long                                                                                                     
GSU09RPER  Keith Perry                                                                                                     
GSU10DGOF  Joy Goff-Marcil                                                                                                 
GSU10RBRO  Jason Brodeur                                                                                                   
GSU11GMOO  Brian Patrick Moore                                                                                             
GSU11RING  Blaise Ingoglia                                                                                                 
GSU12DDOK  Veysel Dokur                                                                                                    
GSU12RBUR  Colleen Burton                                                                                                  
GSU13DDUK  Stephanie L. Dukes                                                                                              
GSU13RBAX  Dennis Baxley                                                                                                   
GSU14DCRU  Janet Cruz                                                                                                      
GSU14RCOL  Jay Collins                                                                                                     
GSU16DROU  Darryl Ervin Rouson                                                                                             
GSU16RPAY  Christina B. Paylan                                                                                             
GSU17DSTE  Linda Stewart                                                                                                   
GSU17RDIX  Steve Dixon                                                                                                     
GSU18DORT  Eunic Ortiz                                                                                                     
GSU18RDIC  Nick DiCeglie                                                                                                   
GSU21DLIO  Amaro Lionheart                                                                                                 
GSU21RHOO  Ed Hooper                                                                                                       
GSU23DHAR  Mike Harvey                                                                                                     
GSU23RBUR  Danny Burgess                                                                                                   
GSU24DPOW  Bobby Powell Jr                                                                                                 
GSU24RANK  Eric P. Ankner                                                                                                  
GSU25DTOR  Victor M. Torres Jr                                                                                             
GSU25RVIV  Peter A. Vivaldi Jr                                                                                             
GSU26DBER  Lori Berman                                                                                                     
GSU26RBYE  Steve Byers                                                                                                     
GSU27DPRO  Christopher Proia                                                                                               
GSU27RALB  Ben Albritton Jr                                                                                                
GSU30DPOL  Tina Scott Polsky                                                                                               
GSU30RREI  William "Bill" Reicherter                                                                                       
GSU33OWRI  WriteinVotes                                                                                                    
GSU33RMAR  Jonathan Martin                                                                                                 
GSU36DPAC  Raquel Pacheco                                                                                                  
GSU36RGAR  Ileana Garcia                                                                                                   
GSU38DPER  Janelle Perez                                                                                                   
GSU38RCAL  Alexis Maria Calatayud

***fl_2022_gen_sldl_prec***
SLDL_DIST  Florida State House District    
GSL001DMAT Franscine C. Mathis                                                                                      
GSL001RSAL Michelle Salzman                                                                                         
GSL002DTAY Carollyn Rabeca Taylor                                                                                   
GSL002RAND Alex Andrade                                                                                             
GSL003OWRI WriteinVotes                                                                                             
GSL003RRUD Joel Rudman                                                                                              
GSL008DFRA Gallop P. Franklin                                                                                       
GSL008RBEN Curt Bender                                                                                              
GSL011DJON Cornelius Jones                                                                                          
GSL011RGAR Sam Garrison                                                                                             
GSL013DNIX Angie Nixon                                                                                              
GSL013NMAS LaCiara Masline                                                                                       
GSL015OWRI WriteinVotes                                                                                             
GSL015RBLA Dean Black                                                                                               
GSL016OWRI WriteinVotes                                                                                             
GSL016RMIC Kiyan Michael                                                                                            
GSL017DAND Michael Anderson                                                                                         
GSL017RBAK Jessica Baker                                                                                            
GSL019DMOR Adam Morley                                                                                              
GSL019RREN Paul Renner                                                                                              
GSL021DHAY Yvonne Hayes Hinson                                                                                      
GSL021RMER Hollye Merton                                                                                            
GSL022DPET Brandon Peters                                                                                           
GSL022RCLE Chuck Clemons                                                                                            
GSL025NHEL Banks Helfrich                                                                                        
GSL025RYAR Taylor Yarkosky                                                                                          
GSL026DKER Linda Kero                                                                                               
GSL026RTRU Keith Truenow                                                                                            
GSL028DNAV John Clifford Navarra                                                                                    
GSL028RLEE Tom Leek                                                                                                 
GSL029DKAR Rick Karl                                                                                                
GSL029RBAR Webster Barnaby                                                                                          
GSL030OWRI WriteinVotes                                                                                             
GSL030RTRA Chase Tramont                                                                                            
GSL033DYAN Anthony Yantz                                                                                            
GSL033RFIN Randy Fine                                                                                               
GSL034DGRE Karen Greb                                                                                               
GSL034RBRA Robert Brackett                                                                                          
GSL035DBAG Rishi Bagga                                                                                              
GSL035RHAW Fred Hawkins                                                                                             
GSL036DPOU Deborah Poulalion                                                                                        
GSL036RPLA Rachel Plakon                                                                                            
GSL037DSMI Carlos Guillermo Smith                                                                                   
GSL037RPLA Susan Plasencia                                                                                          
GSL038DHEN Sarah Henry                                                                                              
GSL038RSMI David Smith                                                                                              
GSL039DHUG Tiffany Hughes                                                                                           
GSL039RBAN Doug Bankson                                                                                             
GSL040DBRA LaVon Bracy Davis                                                                                        
GSL040RROB Nate Robertson                                                                                           
GSL041DANT Bruce H. Antone                                                                                          
GSL041GHAR Robin Denise Harris                                                                                      
GSL042DESK Anna V. Eskamani                                                                                         
GSL042RJAC Bonnie Jackson                                                                                           
GSL043DLOP Johanna Lopez                                                                                            
GSL043RWRI Christopher Wright                                                                                       
GSL045DBRA Allie Braswell                                                                                           
GSL045RAME Carolina Amesty                                                                                          
GSL046DARR Kristen Arrington                                                                                        
GSL046NRIV Ivan A. Rivera                                                                                        
GSL046RDEL Christian De La Torre                                                                                    
GSL047DNIE Anthony Nieves                                                                                           
GSL047RSTA Paula A. Stark                                                                                           
GSL052DMAR Ash Marwah                                                                                               
GSL052RTEM John Temple                                                                                              
GSL053DLAU Keith G. Laufenberg                                                                                      
GSL053RHOL Jeff Holcomb                                                                                             
GSL054DSTA Brian Staver                                                                                             
GSL054NOTW Ryan S. Otwell                                                                                        
GSL054RMAG Randy Maggard                                                                                            
GSL055CHAC Charles "C.J." Hacker Jr                                                                                
GSL055RSTE Kevin M. Steele                                                                                          
GSL058DFEN Bernard "Bernie" Fensterwald                                                                             
GSL058RBER Kimberly "Kim" Berfield                                                                                  
GSL059DDOU Dawn Douglas                                                                                             
GSL059RJAC Berny Jacques                                                                                            
GSL060DCRO Lindsay Cross                                                                                            
GSL060RHEN Audrey Henson                                                                                            
GSL061DWAR Janet Varnell Warwick                                                                                    
GSL061RCHA Linda Chaney                                                                                             
GSL062DRAY Michele K. Rayner                                                                                        
GSL062RBRO Jeremy M. Brown                                                                                          
GSL064DVAL Susan L. Valdés                                                                                          
GSL064RCRU Maura Cruz Lanz                                                                                          
GSL065DMCD Jen McDonald                                                                                             
GSL065RGON Karen Gonzalez Pittman                                                                                   
GSL066DTIL David Tillery                                                                                            
GSL066RKOS Traci Koster                                                                                             
GSL067DDRI Fentrice Driskell                                                                                        
GSL067RBON Lisette Bonano                                                                                           
GSL068DWRI Lorissa Wright                                                                                           
GSL068RMCC Lawrence McClure                                                                                         
GSL069DLEA Andrew Learned                                                                                           
GSL069RALV Daniel "Danny" Alvarez                                                                                   
GSL070DSAL Eleuterio "Junior" Salazar Jr                                                                            
GSL070RBEL Mike Beltran                                                                                             
GSL072DDAM Roberts Guy Dameus                                                                                       
GSL072RGRE Tommy Gregory                                                                                            
GSL073DREI Derek Reich                                                                                              
GSL073RMCF Fiona McFarland                                                                                          
GSL077DENG Eric Engelhart                                                                                           
GSL077RESP Tiffany Esposito                                                                                         
GSL078DSAP Howard Sapp                                                                                              
GSL078RPER Jenna Persons-Mulicka                                                                                    
GSL080DSCH Mitchel Schlayer                                                                                         
GSL080RBOT Adam Botana                                                                                              
GSL084DBLA Forest W. Blanton                                                                                        
GSL084RTRA Dana Lee Trabulsy                                                                                        
GSL085DTUC Curtis J. Tucker                                                                                         
GSL085ROVE Toby Overdorf                                                                                            
GSL086DDEN Raymond Denzel                                                                                           
GSL086RSNY John Snyder                                                                                              
GSL087DOST Sienna Osta                                                                                              
GSL087RCAR Mike Caruso                                                                                              
GSL088DEDM Jervonte "Tae" Edmonds                                                                                   
GSL088RSTE Roz Stevens                                                                                              
GSL089DSIL David Silvers                                                                                            
GSL089RZAP Daniel Judiel Zapata                                                                                     
GSL090DCAS Joseph "Joe" Casello                                                                                     
GSL090RFEI Keith G. Feit                                                                                            
GSL091DTHO Andy Thomson                                                                                             
GSL091RGOS Peggy Gossett-Seidman                                                                                    
GSL092DSKI Kelly Skidmore                                                                                           
GSL092RHER Dorcas Hernandez                                                                                         
GSL093DWAL Katherine M. Waldron                                                                                     
GSL093RBAN Saulis Banionis                                                                                          
GSL094DDAV Terence Davis                                                                                            
GSL094RROT Rick Roth                                                                                                
GSL096DDAL Dan Daley                                                                                                
GSL096RHAG Jenna Hague                                                                                              
GSL100DGON Linda Thompson Gonzalez                                                                                  
GSL100RLAM Chip LaMarca                                                                                             
GSL101DCAS Hillary Cassel                                                                                           
GSL101RSIL Guy Silla                                                                                                
GSL103DBAR Robin Bartleman                                                                                          
GSL103RNAV George Navarini                                                                                          
GSL105DWOO Marie Woodson                                                                                            
GSL105RPAR Vincent Parlatore                                                                                        
GSL106DLEO Jordan W. Leonard                                                                                        
GSL106RBAS Fabián Basabe                                                                                            
GSL113DD'A Alessandro "A.J." D'Amico                                                                                
GSL113RLOP Vicki Lopez                                                                                              
GSL114DBEN Adam Benna                                                                                               
GSL114RCAB Demi Busatta Cabrera                                                                                     
GSL115DDAV Christie Cantin Davis                                                                                    
GSL115RGAR Alina Garcia                                                                                             
GSL118DFAR Johnny Gonzalo Farias                                                                                    
GSL118RFER Juan Fernandez-Barquin                                                                                   
GSL119DGON Gabriel Gonzalez                                                                                         
GSL119RPOR Juan Carlos Porras                                                                                       
GSL120DGEN Adam Gentle                                                                                              
GSL120RMOO James "Jim" V. Mooney Jr           


## Election Results Processing Notes
Files were checked against separate statewide and countywide election result files from the [Florida Department of State Election Archive](https://results.elections.myflorida.com/Index.asp?ElectionDate=11/8/2022&DATAMODE=) for all races but the following: ['G22CFOOWRI', 'G22GOVOWRI', 'GCON12OWRI', 'GCON13OWRI', 'GCON16OWRI', 'GCON18OWRI', 'GCON19OWRI', 'GCON28OWRI', 'GCON04OWRI', 'GCON07OWRI', 'GSL015OWRI', 'GSL016OWRI', 'GSL003OWRI', 'GSL030OWRI', 'GSU33OWRI', 'GSU05OWRI','G22USSOWRI']. The election archive results had vote totals for particular candidates in some of these races, but we confirmed that the "OWRI" results contained results for more than just the particular candidates listed in the archive results, and as such did not match.

For the races we were able to check, totals matched in every county except for Miami-Dade and Seminole county. In Miami-Dade, there were two more total votes in the precinct-level results in the following races: GSL106RBAS and GSL106DLEO. Although the precinct-level file contained a file with recount election results for this file, the results summed to tens of thousands of votes higher than the official totals and as such were not used.

In Seminole County, the largest difference was 12 fewer votes in the precinct-level file for the G22SCJNGRO race. Full details can be found in the notebook linked below. It is not immediately clear why these differences exist.


## Precinct Boundary Processing Notes
Please note that although we produced this file to be as accurate as possible, we may come across additional information in the future which may require us to update this file.

Precinct boundaries for 30 of Florida's 67 counties are sourced from VEST's 2020 map. VEST data for those counties appeared to have no changes in the names or counts of precincts since the 2020 general election.

Precinct boundaries for 19 counties are sourced from county Supervisor of Elections offices. For six of those counties, RDH staff constructed precinct boundary maps from census block assignment files.

Precinct boundaries for 18 counties are sourced from the map compiled by RDH volunteer Sebastian Pojman. RDH staff verified these boundaries by comparing them to maps hosted online by each county, mostly in interactive or PDF forms that were not otherwise downloadable as GIS files.

The original Pojman map file included some duplicate precinct ID labels. RDH staff visually inspected shapes associated with those labels and determined which ones should be retained and dissolved together. The majority of duplicates were small geometries that overlapped other precinct areas. Such duplicates were removed.

Note: The revised version of the Pojman map addressed duplicates by dissolving all of them, rather than removing some. This caused some precinct boundaries to include erroneous, non-contiguous shapes. For this reason, RDH staff mostly used the original version. The revised version is used for two counties where substantial edits to the map improved accuracy.

Precinct IDs for some counties in the Pojman and VEST files did not match precinct IDs in RDH election results. In such cases, RDH staff manually created dictionaries that matched precincts using vote totals, polling location names, and/or visual inspection on Google Maps.

Precinct boundaries in all counties were visually checked against the L2 voter file. RDH staff overlayed the compiled precinct boundary map on top of a map of voters, represented as dots located at their registered home address and colored according to their 2022 general election precinct assignment. All boundaries appeared to encompass the correct set of voters. 

In instances when votes from the election results could not be matched to specific precincts, RDH allocated those votes proportionally to (a) precincts across the whole county or (b) precincts with shapes that likely contain those votes.  

Some precincts are split across Congressional, House of Representatives or State Senate Districts. In these cases, the precincts can be split into the particular areas contained in each district using a district shapefile and one can give the votes for the candidates in those particular districts to that district's portion of the precinct. This extra step makes block-level disaggregation and RPV analyses more accurate. For races outside of those particular districts, one does not know the proportion of votes to allot to each district-precinct chunk. As such, separate files are created to ensure the accuracy of votes. Because there were splits for Congress, House of Representatives and State Senate Districts, files for each of these levels, as well as for statewide elections, were created. 

In some cases, a precinct may have votes for multiple districts, but does not spatially intersect with all districts for which it contains votes. This could either be evidence that a precinct's boundaries are incorrect, or simply an instance in which a voter either voted or had their vote counted at the incorrect precinct. For the level-specific files mentioned above, we look into the precinct shapefiles and, unless we find a particular precinct boundary to change, these votes are dropped. For details on the exact number of votes dropped, please see the Jupyter Notebook linked below.

There is also a "fl_2022_gen_prec_no_splits" file, which contains all election results, but does not include a SLDL_DIST, SLDU_DIST or CONG_DIST column.

                                                                                                  
## Processing Steps
Visit the RDH GitHub and the processing script for precinct boundaries and election results [here](https://github.com/nonpartisan-redistricting-datahub/pber_collection/tree/main/FL/2022)

## Additional Notes
A full raw-from-source folder containing all of the input files used to construct this file can be made available upon request.

Please direct questions related to processing this dataset to info@redistrictingdatahub.org.
