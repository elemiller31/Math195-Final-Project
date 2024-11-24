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

***ga_2022_gen_cong_prec***
CONG_DIST  Georgia Congressional District             
GCON01DHER Wade Herring                               
GCON01RCAR Earl L. ""Buddy"" Carter                   
GCON02DBIS Sanford Bishop                             
GCON02RWES Chris West                                 
GCON03DALM Val Almonord                               
GCON03RFER Drew Ferguson                              
GCON04DJOH Henry C ""Hank"" Johnson Jr                
GCON04RCHA Jonathan Chavez                            
GCON05DWIL Nikema Williams                            
GCON05RZIM Christian Zimm                             
GCON06DCHR Bob Christian                              
GCON06RMCC Rich McCormick                             
GCON07DMCB Lucy McBath                                
GCON07RGON Mark Gonsalves                             
GCON08DBUT Darrius Butler                             
GCON08RSCO Austin Scott                               
GCON09DFOR Michael ""Mike"" Ford                      
GCON09RCLY Andrew Clyde                               
GCON10DJOH Tabitha Johnson-Green                      
GCON10RCOL Mike Collins                               
GCON11DDAZ Antonio Daza                               
GCON11RLOU Barry Loudermilk                           
GCON12DJOH Elizabeth ""Liz"" Johnson                  
GCON12RALL Rick W. Allen                              
GCON13DSCO David Scott                                
GCON13RGON Caesar Gonzales                            
GCON14DFLO Marcus Flowers                             
GCON14RGRE Marjorie Taylor Greene
 
***ga_2022_gen_sldl_prec*** 
SLDL_DIST  Georgia House of Representatives District
GSL001RCAM Mike Cameron                               
GSL002RTAR Steve Tarvin                               
GSL003RHOR Mitchell Horner                            
GSL004RCAR Kasey Carpenter                            
GSL005RBAR Matt Barton                                
GSL006RRID Jason T. Ridley                            
GSL007RRAL David Ralston                              
GSL008DKRI June Krise                                 
GSL008RGUN Stan Gunter                                
GSL009RWAD Will Wade                                  
GSL010RAND Victor E. Anderson                         
GSL011DHOL Kayla L. Hollifield                        
GSL011RJAS Rick Jasperse                              
GSL012RLUM Eddie Lumsden                              
GSL013RDEM Katie Dempsey                              
GSL014RSCO Mitchell Scoggins                          
GSL015RGAM Matthew Gambill                            
GSL016RKEL Trey Kelley                                
GSL017DMAR Sunshine Marshall                          
GSL017RMOM Martin Momtahan                            
GSL018DRHU Pat Rhudy                                  
GSL018RSMI Tyler Paul Smith                           
GSL019DCOY R.J. Coyle                                 
GSL019RGUL Joseph Gullett                             
GSL020RBYR Charlice Byrd                              
GSL021RTHO Brad Thomas                                
GSL022DHIL Stacee Lashone Hill                        
GSL022RRID Jordan Ridley                              
GSL023RBAL Mandi L Ballinger                          
GSL024DWAL Sydney Walker                              
GSL024RBAR Carter Barrett                             
GSL025DMEY Craig J. Meyer                             
GSL025RJON Todd Jones                                 
GSL026DHEL Matthew J. Helms                           
GSL026RMCD Lauren W. McDonald III                     
GSL027RHAW Lee Hawkins                                
GSL028DWOO Claudia Wood                               
GSL028RCOX Brent Cox                                  
GSL029DPAN Devin Pandy                                
GSL029RDUB Matt Dubnik                                
GSL030DFLO Kim Floria                                 
GSL030RMCC Derrick McCollum                           
GSL031RDUN Emory Dunahoo, Jr.                         
GSL032RERW Chris Erwin                                
GSL033RPOW Alan Powell                                
GSL034DCOK Dorothy Coker                              
GSL034RSEA Devan Seabaugh                             
GSL035DCAM Lisa Campbell                              
GSL035RTRI Robert Trim                                
GSL036DRYN James F. Ryner                             
GSL036REHR Ginny Ehrhart                              
GSL037DWIL Mary Frances Williams                      
GSL037RRED Marites ""Tess"" Redding                   
GSL038DWIL David Wilkerson                            
GSL039DCUM Terry Cummings                             
GSL039RANG Olivia Angel                               
GSL040DSTO Doug Stoner                                
GSL040RFON Fun Fong                                   
GSL041DSMI Michael Smith                              
GSL041RROD James Allen Rodi                           
GSL042DANU Teri Anulewicz                             
GSL043DADE Solomon Adesanya                           
GSL043RTIL Anna J. Tillman                            
GSL044DOYO Willie Mae Oyogoa                          
GSL044RPAR Don L. Parsons                             
GSL045DMCC Dustin McCormick                           
GSL045RCOO Sharon Cooper                              
GSL046DGAR Micheal Garza                              
GSL046RCAR John Carson                                
GSL047RJON Jan Jones                                  
GSL048DROB Mary Robichaux                             
GSL048RHIL Scott Hilton                               
GSL049DGIL Peggy Gillen                               
GSL049RMAR Charles E. ""Chuck"" Martin                
GSL050DAU  Michelle Au                                
GSL050RRED Narender Reddy                             
GSL051DPAN Esther Panitch                             
GSL051RKOR Peter Korman                               
GSL052DROB Shea Roberts                               
GSL052RAHR Wendy  Ahrenkiel                           
GSL053DCOF Kelly Coffman                              
GSL053RSIL Deborah Silcox                             
GSL054DHOL Betsy Holland                              
GSL054RBAI John Bailey                                
GSL055DWIL Inga Willis                                
GSL055RLEN Samuel S. Lenaeus                          
GSL056DMAI Mesha Mainor                               
GSL057DEVA Stacey Evans                               
GSL058DCAN Park Elizabeth Cannon                      
GSL059DOLA Phil Olaleye                               
GSL060DJON Sheila Jones                               
GSL061DBRU Roger Bruce                                
GSL062DMIL Tanya F. Miller                            
GSL063DSCH Kim Schofield                              
GSL064DEDW Montenia Edwards                           
GSL064RNEW Kimberly R. New                            
GSL065DTHO Mandisha A. Thomas                         
GSL065RHOR Jan Horne                                  
GSL066DALE Kimberly Alexander                         
GSL067DGLA Lydia Glaize                               
GSL067RAMI Marziyeh Marzi Amirizadeh                  
GSL068DNAG Tish Naghise                               
GSL068RMAT Stoney Mathis                              
GSL069DBAZ Debra Bazemore                             
GSL070DAND Calvin Louis Anderson, Jr.                 
GSL070RSMI Lynn Smith                                 
GSL071DOKA Afoma Eguh Okafor                          
GSL071RCOL J. Collins                                 
GSL072RHUD David Huddleston                           
GSL073RBON Josh Bonner                                
GSL074DHAR William Harris                             
GSL074RMAT Karen Mathiak                              
GSL075DGLA Mike Glanton                               
GSL075RASH Della Ashley                               
GSL076DSCO Sandra Givens Scott                        
GSL077DBUR Rhonda Burnough                            
GSL078DDOU Demetrius Douglas                          
GSL079DNEA Yasmin Neal                                
GSL080DTRA Long Tran                                  
GSL080RAND Brian Anderson                             
GSL081DHOL Scott Holcomb                              
GSL081RBEN Mary Williams Benefield                    
GSL082DOLI Mary Margaret Oliver                       
GSL082RMIL Jenine Milum                               
GSL083DLUP Karen Lupton                               
GSL083RBER Catherine Bernard                          
GSL084DCRA Omari Crawford                             
GSL085DDRE Karla Drenner                              
GSL086DBAR Imani Barnes                               
GSL086RKIN Lisa Y. Kinnemore                          
GSL087DDAV Viola Davis                                
GSL088DMIT Billy Mitchell                             
GSL088RFRE William Park Freeman                       
GSL089DEVA Becky Evans                                
GSL089RSHE Rick Sheppard                              
GSL090DDRA Saira Draper                               
GSL090RDIO Jodi Diodati                               
GSL091DMOO Angela Moore                               
GSL092DTAY Rhonda S. Taylor                           
GSL093DCAR Doreen Carter                              
GSL094DBEN Karen Bennett                              
GSL095DKEN Dar'Shun Kendrick                          
GSL095RDAW Dexter Dawston                             
GSL096DMAR Pedro ""Pete"" Marin                       
GSL096RLOW Daelen Lowry                               
GSL097DROM Ruwa Romman                                
GSL097RCHA John Chan                                  
GSL098DLIM Marvin Lim                                 
GSL099DDUG Om Duggal                                  
GSL099RREE Matt Reeves                                
GSL100DJAC Louisa Shell Jackson                       
GSL100RCLA David Clark                                
GSL101DKEN Gregg Kennard                              
GSL101RPRO Zach Procter                               
GSL102DOKO Gabe Okoye                                 
GSL102RHAR Wesley S. Harding                          
GSL103DANA Ernie Anaya                                
GSL103RHON Soo Hong                                   
GSL104DREI Patrick J. Reinert                         
GSL104REFS Chuck Efstration                           
GSL105DMUG Farooq Mughal                              
GSL105RDON Sandy Donatucci                            
GSL106DHUT Shelly Hutchinson                          
GSL106RWRE Preston A. Wren                            
GSL107DPAR Sam Park                                   
GSL107RCAO Hai Cao                                    
GSL108DCLA Jasmine Clark                              
GSL108RCRI Johnny Crist                               
GSL109DMCC Dewey L. McClain                           
GSL110DADE Segun Adeyina                              
GSL111DCOX Ryan Cox                                   
GSL111RMAR Reynaldo ""Rey"" Martinez                  
GSL112DREE Debbie Reed                                
GSL112RWIL Bruce Williamson                           
GSL113DHEN Sharon Henderson                           
GSL114DADA Malcolm Adams                              
GSL114RFLE Tim Fleming                                
GSL115DLEW Regina Lewis-Ward                          
GSL116DHOL El-Mahdi Holly                             
GSL116RBEN Bruce Bennington                           
GSL117DRUC Demetrius Rucker                           
GSL117RDAN Lauren Daniel                              
GSL118DBEL Sharonda Bell                              
GSL118RCRO Clint Crowe                                
GSL119RRAM Danny Rampey                               
GSL120DJOH Mokah Jasmine Johnson                      
GSL120RGAI Houston Gaines                             
GSL121DAUE Jeff Auerbach                              
GSL121RWIE Marcus A Wiedower                          
GSL122DFRY Spencer Frye                               
GSL123RLEV Rob Leverett                               
GSL124DHOW Kat Howkins                                
GSL124RRHO Trey Rhodes                                
GSL125RFLE Barry Fleming                              
GSL126DFRA Gloria Frazier                             
GSL126RHAR William C. Harris                          
GSL127RNEW Mark Newton                                
GSL128DJAC Mack Jackson                               
GSL129DHOW Henry ""Wayne"" Howard                     
GSL130DGLA Lynn Gladney                               
GSL130RSWE Dan Swenson                                
GSL131RLOT Jodi Lott                                  
GSL132DPRI Brian L. Prince                            
GSL133DWAL Hoganne Harrison Walton                    
GSL133RVAN Kenneth Vance                              
GSL134DDIC Anthony Dickson                            
GSL134RKNI David Knight                               
GSL135RCAM Beth Camp                                  
GSL136RJEN David Jenkins                              
GSL137DBUC Debbie G. Buckner                          
GSL137RRIC Justin Rickett                             
GSL138RSMI Vance Smith, Jr.                           
GSL139RSMI Richard H. Smith                           
GSL140DREE Tremaine Teddy Reese                       
GSL141DHUG Carolyn Hugley                             
GSL142DPAR Miriam Paris                               
GSL143DBEV James Beverly                              
GSL144DCON Nettie B. Conner                           
GSL144RWAS Dale Washburn                              
GSL145RDIC Robert Dickey                              
GSL146DDRI Courtney L. Driver                         
GSL146RBLA Shaw Blackmon                              
GSL147DPHI Ariel Phillips                             
GSL147RBAL Bethany Ballard                            
GSL148RWIL Noel Williams, Jr.                         
GSL149RMAT Danny Mathis                               
GSL150DBEN Patty Bentley                              
GSL151DBAR Joyce Barlow                               
GSL151RCHE Mike Cheokas                               
GSL152RYEA Bill Yearta                                
GSL153DSAM David Sampson                              
GSL153RTAY Tracy Taylor                               
GSL154DHAY John Hayes                                 
GSL154RGRE Gerald E. Greene                           
GSL155RHAT Matt Hatchett                              
GSL156DKIT Lethia J. Kittrell                         
GSL156RHAG Leesa Hagan                                
GSL157RWER William ""Bill"" Werkheiser                
GSL158DSMI Madeline Ryan Smith                        
GSL158RPAR Butch Parrish                              
GSL159RBUR Jon G. Burns                               
GSL160RFRA Lehman Franklin                            
GSL161DBAR Margo Barbee                               
GSL161RHIT Bill Hitchens                              
GSL162DGIL Carl Wayne Gilliard                        
GSL163DWES Anne Allen Westbrook                       
GSL164DTHO Marcus Thompson                            
GSL164RSTE Ron Stephens                               
GSL165DJAC Edna Jackson                               
GSL166RPET Jesse Petrea                               
GSL167RDEL Buddy DeLoach                              
GSL168DWIL Al Williams                                
GSL169DBRO Mickey Brockington                         
GSL169RPIR Clay Pirkle                                
GSL170RHOU Penny Houston                              
GSL171RCAM Joe Campbell                               
GSL172RWAT Sam Watson                                 
GSL173DSR  Keith L. Jenkins Sr                        
GSL173RTAY Darlene Taylor                             
GSL174RCOR John L. Corbett                            
GSL175RLAH John Lahood                                
GSL176RBUR James Burchett                             
GSL177DSHA Dexter L. Sharper                          
GSL178RMEE Steven Meeks                               
GSL179RTOW Rick Townsend                              
GSL180RSAI Steven Sainz         

***ga_2022_gen_sldu_prec*** 
SLDU_DIST  Georgia State Senate District                                 
GSU01DJON  James ""Jay"" Jones                        
GSU01RWAT  Ben Watson                                 
GSU02DMAL  Derek Mallow                               
GSU02RYOU  Clinton Young                              
GSU03RHOD  Mike Hodges                                
GSU04RHIC  Billy Hickman                              
GSU05DRAH  Sheikh Rahman                              
GSU06DEST  Jason Esteves                              
GSU06RGLA  Fred Glass                                 
GSU07DISL  Nabilah Islam                              
GSU07RMCK  Josh McKay                                 
GSU08RGOO  Russ Goodman                               
GSU09DMER  Nikki Merritt                              
GSU10DJON  Emanuel D. Jones                           
GSU11RBUR  Dean Burke                                 
GSU12DSIM  Freddie Powell Sims                        
GSU13RSUM  Carden H. Summers                          
GSU14DMCL  Josh McLaurin                              
GSU14RHAU  Liz Hausmann                               
GSU15DHAR  Ed Harbison                                
GSU16DDUB  Pingke Dubignon                            
GSU16RHAR  Marty Harbin                               
GSU17DMOR  Kacy D. Morgan                             
GSU17RSTR  Brian Strickland                           
GSU18DBEN  Chris Benton                               
GSU18RKEN  John F. Kennedy                            
GSU19DMOO  Michael ""Buckle"" Moore                   
GSU19RTIL  Blake Tillery                              
GSU20RWAL  Larry Walker                               
GSU21RBEA  Brandon Beach                              
GSU22DJON  Harold V. Jones II                         
GSU22RDAN  Andrew Danielson                           
GSU23RBUR  Max Burns                                  
GSU24RAND  Lee Anderson                               
GSU25DROD  Valerie Rodgers                            
GSU25RWIL  Ricky ""Rick"" Williams                    
GSU26DLUC  David E. Lucas, Sr.                        
GSU27DBIN  Brent Binion                               
GSU27RDOL  Greg Dolezal                               
GSU28RBRA  Matt Brass                                 
GSU29DWRI  Ellen Wright                               
GSU29RROB  Randy Robertson                            
GSU30RDUG  Mike Dugan                                 
GSU31RANA  Jason Anavitarte                           
GSU32DBEN  Sylvia L. Bennett                          
GSU32RKIR  Kay Kirkpatrick                            
GSU33DRHE  Michael Rhett                              
GSU34DSEA  Valencia M. Seay                           
GSU34RSMI  Thomas ""Tommy"" Smith                     
GSU35DJAM  Donzella James                             
GSU36DORR  Nan Orrock                                 
GSU37DPAR  Vanessa Parker                             
GSU37RSET  Ed Setzler                                 
GSU38DTAT  Horacena Tate                              
GSU39DHAL  Sonya Halpern                              
GSU40DHAR  Sally Harrell                              
GSU40RMCD  Austin McDonald                            
GSU41DJAC  Kim Jackson                                
GSU41RJON  Jayre Jones                                
GSU42DPAR  Elena Parent                               
GSU43DAND  Tonya P. Anderson                          
GSU43RWIL  Melanie Williams                           
GSU44DDAV  Gail Davenport                             
GSU45DJON  Matielyn Jones                             
GSU45RDIX  Clint Dixon                                
GSU46DFER  Andrew Ferguson                            
GSU46RCOW  Bill Cowsert                               
GSU47DSCO  Conolus Scott, Jr.                         
GSU47RGIN  Frank Ginn                                 
GSU48DUDD  Josh Uddin                                 
GSU48RSTI  Shawn Still                                
GSU49DCOO  Jody Cooley                                
GSU49RECH  Shelly Echols                              
GSU50DWIL  Paulette Williams                          
GSU50RHAT  Bo Hatchett                                
GSU51RGOO  Steve Gooch                                
GSU52RHUF  Chuck Hufstetler                           
GSU53RMOO  Colton Moore                               
GSU54RPAY  Chuck Payne                                
GSU55DBUT  Gloria S. Butler                           
GSU56DTHO  Patrick Thompson                           
GSU56RALB  John Albers

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
