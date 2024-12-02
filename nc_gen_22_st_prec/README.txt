North Carolina 2022 General Election Precinct-Level Results and Boundaries

## RDH Date Retrieval
03/15/2023

## RDH Update Date
09/14/2023

## Sources
[North Carolina State Board of Elections Election results file:](https://www.ncsbe.gov/results-data/election-results/historical-election-results-data)
[North Carolina State Board of Elections Precinct Boundary File:](https://s3.amazonaws.com/dl.ncsbe.gov/PrecinctMaps/SBE_PRECINCTS_20220831.zip)

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
IA## - Intermediate appellate court Seat ##
SSC## - State Supreme Court Associate Justice Seat ##
USS - U.S. Senate
CON## - U.S. Congress District ##
SL###  - State Legislative Lower District ###
SU##  - State Legislative Upper District ##


Party Codes Used:
D - Democratic
G - Green
L - Libertarian
O - Other / Write In Votes
R - Republican


## Fields:
Field Name Description
      
***standard across files***      
UNIQUE_ID  Unique precinct-identifier combining county and precinct names    
COUNTYFP   State County FIPS code                                                
COUNTYNM   County name  
PRECINCT   County precinct identifier
*insert file-specific columns*
geometry   geospatial geometry 

***nc_gen_22_st_prec.shp***
G22USSDBEA Cheri Beasley, US SENATE                                              
G22USSGHOH Matthew Hoh, US SENATE                                                
G22USSLBRA Shannon W. Bray, US SENATE                                            
G22USSOWRI Write-In (Miscellaneous), US SENATE                                   
G22USSRBUD Ted Budd, US SENATE  
GSSC03DINM Lucy Inman, NC SUPREME COURT ASSOCIATE JUSTICE SEAT 03                
GSSC03RDIE Richard Dietz, NC SUPREME COURT ASSOCIATE JUSTICE SEAT 03             
GSSC05DERV Sam J. Ervin IV, NC SUPREME COURT ASSOCIATE JUSTICE SEAT 05           
GSSC05RALL Trey Allen, NC SUPREME COURT ASSOCIATE JUSTICE SEAT 05    
GSAC08DTHO  Carolyn Jennings Thompson, NC COURT OF APPEALS JUDGE SEAT 08          
GSAC08RFLO  Julee Tate Flood, NC COURT OF APPEALS JUDGE SEAT 08                   
GSAC09DSAL  Brad A. Salmon, NC COURT OF APPEALS JUDGE SEAT 09                     
GSAC09RSTR  Donna Stroud, NC COURT OF APPEALS JUDGE SEAT 09                       
GSAC10DADA  Gale Murray Adams, NC COURT OF APPEALS JUDGE SEAT 10                  
GSAC10RTYS  John M. Tyson, NC COURT OF APPEALS JUDGE SEAT 10                      
GSAC11DJAC  Darren Jackson, NC COURT OF APPEALS JUDGE SEAT 11 
GSAC11RSTA  Michael J. Stading, NC COURT OF APPEALS JUDGE SEAT 11 

***nc_gen_22_cong_prec.shp***
CONG_DIST  Congressional District
GCON01DDAV Don Davis, US HOUSE OF REPRESENTATIVES DISTRICT 01                    
GCON01RSMI Sandy Smith, US HOUSE OF REPRESENTATIVES DISTRICT 01                  
GCON02DROS Deborah K. Ross, US HOUSE OF REPRESENTATIVES DISTRICT 02              
GCON02RVIL Christine E. Villaverde, US HOUSE OF REPRESENTATIVES DISTRICT 02      
GCON03DGAS Barbara D. Gaskins, US HOUSE OF REPRESENTATIVES DISTRICT 03           
GCON03RMUR Greg Murphy, US HOUSE OF REPRESENTATIVES DISTRICT 03                  
GCON04DFOU Valerie P. Foushee, US HOUSE OF REPRESENTATIVES DISTRICT 04           
GCON04RGEE Courtney Geels, US HOUSE OF REPRESENTATIVES DISTRICT 04               
GCON05DPAR Kyle Parrish, US HOUSE OF REPRESENTATIVES DISTRICT 05                 
GCON05RFOX Virginia Foxx, US HOUSE OF REPRESENTATIVES DISTRICT 05                
GCON06DMAN Kathy Manning, US HOUSE OF REPRESENTATIVES DISTRICT 06                
GCON06LWAT Thomas Watercott, US HOUSE OF REPRESENTATIVES DISTRICT 06             
GCON06RCAS Christian Castelli, US HOUSE OF REPRESENTATIVES DISTRICT 06           
GCON07DGRA Charles Graham, US HOUSE OF REPRESENTATIVES DISTRICT 07               
GCON07RROU David Rouzer, US HOUSE OF REPRESENTATIVES DISTRICT 07                 
GCON08DHUF Scott Huffman, US HOUSE OF REPRESENTATIVES DISTRICT 08                
GCON08RBIS Dan Bishop, US HOUSE OF REPRESENTATIVES DISTRICT 08                   
GCON09DCLA Ben Clark, US HOUSE OF REPRESENTATIVES DISTRICT 09                    
GCON09RHUD Richard Hudson, US HOUSE OF REPRESENTATIVES DISTRICT 09               
GCON10DGEN Pam Genant, US HOUSE OF REPRESENTATIVES DISTRICT 10                   
GCON10OWRI Write-In (Miscellaneous), US HOUSE OF REPRESENTATIVES DISTRICT 10     
GCON10RMCH Patrick McHenry, US HOUSE OF REPRESENTATIVES DISTRICT 10              
GCON11DBEA Jasmine Beach-Ferrara, US HOUSE OF REPRESENTATIVES DISTRICT 11        
GCON11LCOA David Adam Coatney, US HOUSE OF REPRESENTATIVES DISTRICT 11           
GCON11REDW Chuck Edwards, US HOUSE OF REPRESENTATIVES DISTRICT 11                
GCON12DADA Alma S. Adams, US HOUSE OF REPRESENTATIVES DISTRICT 12                
GCON12RLEE Tyler Lee, US HOUSE OF REPRESENTATIVES DISTRICT 12                    
GCON13DNIC Wiley Nickel, US HOUSE OF REPRESENTATIVES DISTRICT 13                 
GCON13RHIN Bo Hines, US HOUSE OF REPRESENTATIVES DISTRICT 13                     
GCON14DJAC Jeff Jackson, US HOUSE OF REPRESENTATIVES DISTRICT 14                 
GCON14RHAR Pat Harrigan, US HOUSE OF REPRESENTATIVES DISTRICT 14                 
                   
***nc_gen_22_sldl_prec.shp***   
SLDL_DIST  State House District
GSL001RGOO Edward C. Goodwin, NC HOUSE OF REPRESENTATIVES DISTRICT 001           
GSL002DJEF Ray Jeffers, NC HOUSE OF REPRESENTATIVES DISTRICT 002                 
GSL002LBEL Gavin Bell, NC HOUSE OF REPRESENTATIVES DISTRICT 002                  
GSL002RYAR Larry Yarborough, NC HOUSE OF REPRESENTATIVES DISTRICT 002            
GSL003RTYS Steve Tyson, NC HOUSE OF REPRESENTATIVES DISTRICT 003                 
GSL004DBOY Wesley L. Boykin, NC HOUSE OF REPRESENTATIVES DISTRICT 004            
GSL004RDIX Jimmy Dixon, NC HOUSE OF REPRESENTATIVES DISTRICT 004                 
GSL005DIII Howard Hunter III, NC HOUSE OF REPRESENTATIVES DISTRICT 005           
GSL005RWAR Bill Ward, NC HOUSE OF REPRESENTATIVES DISTRICT 005                   
GSL006DJOH Kiara Johnson, NC HOUSE OF REPRESENTATIVES DISTRICT 006               
GSL006RPIK Joe Pike, NC HOUSE OF REPRESENTATIVES DISTRICT 006                    
GSL007RWIN Matthew Winslow, NC HOUSE OF REPRESENTATIVES DISTRICT 007             
GSL008DBRO Gloristine Brown, NC HOUSE OF REPRESENTATIVES DISTRICT 008            
GSL008RVIN Charles (Drock) Vincent, NC HOUSE OF REPRESENTATIVES DISTRICT 008     
GSL009DFAR Brian Farkas, NC HOUSE OF REPRESENTATIVES DISTRICT 009                
GSL009RREE Timothy Reeder, NC HOUSE OF REPRESENTATIVES DISTRICT 009              
GSL010RBEL John Bell, NC HOUSE OF REPRESENTATIVES DISTRICT 010                   
GSL011DDAH Allison A. Dahle, NC HOUSE OF REPRESENTATIVES DISTRICT 011            
GSL012DWIL Lillie Williams, NC HOUSE OF REPRESENTATIVES DISTRICT 012             
GSL012RHUM Chris Humphrey, NC HOUSE OF REPRESENTATIVES DISTRICT 012              
GSL013DTOM Katie Tomberlin, NC HOUSE OF REPRESENTATIVES DISTRICT 013             
GSL013RCAI Celeste Cairns, NC HOUSE OF REPRESENTATIVES DISTRICT 013              
GSL014DJOH Isaiah (Ike) Johnson, NC HOUSE OF REPRESENTATIVES DISTRICT 014        
GSL014RCLE George G. Cleveland, NC HOUSE OF REPRESENTATIVES DISTRICT 014         
GSL015DSCH Christopher Schulte, NC HOUSE OF REPRESENTATIVES DISTRICT 015         
GSL015RSHE Phillip Shepard, NC HOUSE OF REPRESENTATIVES DISTRICT 015             
GSL016RSMI Carson Smith, NC HOUSE OF REPRESENTATIVES DISTRICT 016                
GSL017DTER Eric Terashima, NC HOUSE OF REPRESENTATIVES DISTRICT 017              
GSL017RILE Frank Iler, NC HOUSE OF REPRESENTATIVES DISTRICT 017                  
GSL018DBUT Deb Butler, NC HOUSE OF REPRESENTATIVES DISTRICT 018                  
GSL018RHIN John Hinnant, NC HOUSE OF REPRESENTATIVES DISTRICT 018                
GSL019RMIL Charlie Miller, NC HOUSE OF REPRESENTATIVES DISTRICT 019              
GSL020DDEL Amy Block DeLoach, NC HOUSE OF REPRESENTATIVES DISTRICT 020           
GSL020RDAV Ted Davis, Jr., NC HOUSE OF REPRESENTATIVES DISTRICT 020              
GSL021DLIU Ya Liu, NC HOUSE OF REPRESENTATIVES DISTRICT 021                      
GSL021LMOR Joshua Morris, NC HOUSE OF REPRESENTATIVES DISTRICT 021               
GSL021RFAL Gerard Falzon, NC HOUSE OF REPRESENTATIVES DISTRICT 021               
GSL022RBRI William Brisson, NC HOUSE OF REPRESENTATIVES DISTRICT 022             
GSL023DWIL Shelly Willingham, NC HOUSE OF REPRESENTATIVES DISTRICT 023           
GSL023RPRO James Crowell Proctor, NC HOUSE OF REPRESENTATIVES DISTRICT 023       
GSL024DCOO Linda Cooper-Suggs, NC HOUSE OF REPRESENTATIVES DISTRICT 024          
GSL024RFON Ken Fontenot, NC HOUSE OF REPRESENTATIVES DISTRICT 024                
GSL025DGAI James D. Gailliard, NC HOUSE OF REPRESENTATIVES DISTRICT 025          
GSL025LTAY Nick Taylor, NC HOUSE OF REPRESENTATIVES DISTRICT 025                 
GSL025RCHE Allen Chesser, NC HOUSE OF REPRESENTATIVES DISTRICT 025               
GSL026DBEN Linda Bennett, NC HOUSE OF REPRESENTATIVES DISTRICT 026               
GSL026RWHI Donna McDowell White, NC HOUSE OF REPRESENTATIVES DISTRICT 026        
GSL027DWRA Michael H. Wray, NC HOUSE OF REPRESENTATIVES DISTRICT 027             
GSL027RTRI Wes Tripp, NC HOUSE OF REPRESENTATIVES DISTRICT 027                   
GSL028DMAY Wendy Ella May, NC HOUSE OF REPRESENTATIVES DISTRICT 028              
GSL028RSTR Larry C. Strickland, NC HOUSE OF REPRESENTATIVES DISTRICT 028         
GSL029DALS Vernetta Alston, NC HOUSE OF REPRESENTATIVES DISTRICT 029             
GSL030DMOR Marcia Morey, NC HOUSE OF REPRESENTATIVES DISTRICT 030                
GSL030LMEI Guy Meilleur, NC HOUSE OF REPRESENTATIVES DISTRICT 030                
GSL030RANT William G. Antico, NC HOUSE OF REPRESENTATIVES DISTRICT 030           
GSL031DHAW Zack Hawkins, NC HOUSE OF REPRESENTATIVES DISTRICT 031                
GSL031LHAU Sean Haugh, NC HOUSE OF REPRESENTATIVES DISTRICT 031                  
GSL032DGAR Terry Garrison, NC HOUSE OF REPRESENTATIVES DISTRICT 032              
GSL032RSOS Frank Sossamon, NC HOUSE OF REPRESENTATIVES DISTRICT 032              
GSL033DGIL Rosa U. Gill, NC HOUSE OF REPRESENTATIVES DISTRICT 033                
GSL033LCOS Chris Costello, NC HOUSE OF REPRESENTATIVES DISTRICT 033              
GSL033RDIN Stephanie Dingee, NC HOUSE OF REPRESENTATIVES DISTRICT 033            
GSL034DLON Tim Longest, NC HOUSE OF REPRESENTATIVES DISTRICT 034                 
GSL034LMCD Kat McDonald, NC HOUSE OF REPRESENTATIVES DISTRICT 034                
GSL034RSES Ashley Seshul, NC HOUSE OF REPRESENTATIVES DISTRICT 034               
GSL035DEVE Terence Everitt, NC HOUSE OF REPRESENTATIVES DISTRICT 035             
GSL035LSER Joseph Serio, NC HOUSE OF REPRESENTATIVES DISTRICT 035                
GSL035RCAN Fred Von Canon, NC HOUSE OF REPRESENTATIVES DISTRICT 035              
GSL036DHAE Julie von Haefen, NC HOUSE OF REPRESENTATIVES DISTRICT 036            
GSL036LWAR Kyle Ward, NC HOUSE OF REPRESENTATIVES DISTRICT 036                   
GSL036RHAR John Harris, NC HOUSE OF REPRESENTATIVES DISTRICT 036                 
GSL037DKEL Christine Kelly, NC HOUSE OF REPRESENTATIVES DISTRICT 037             
GSL037LROB Christopher Robinson, NC HOUSE OF REPRESENTATIVES DISTRICT 037        
GSL037RPAR Erin Pare, NC HOUSE OF REPRESENTATIVES DISTRICT 037                   
GSL038DJON Abe Jones, NC HOUSE OF REPRESENTATIVES DISTRICT 038                   
GSL038LMIZ Christopher Mizelle, NC HOUSE OF REPRESENTATIVES DISTRICT 038         
GSL039DROB James A. Roberson, NC HOUSE OF REPRESENTATIVES DISTRICT 039           
GSL039RJON Greg Jones, NC HOUSE OF REPRESENTATIVES DISTRICT 039                  
GSL040DJOH Joe John, NC HOUSE OF REPRESENTATIVES DISTRICT 040                    
GSL040LNEL Michael Nelson, NC HOUSE OF REPRESENTATIVES DISTRICT 040              
GSL040RAVI Marilyn Avila, NC HOUSE OF REPRESENTATIVES DISTRICT 040               
GSL041DCER Maria Cervania, NC HOUSE OF REPRESENTATIVES DISTRICT 041              
GSL041LTER Kevin Terrett, NC HOUSE OF REPRESENTATIVES DISTRICT 041               
GSL041RFOR Bruce K. Forster, NC HOUSE OF REPRESENTATIVES DISTRICT 041            
GSL042DLUC Marvin W. Lucas, NC HOUSE OF REPRESENTATIVES DISTRICT 042             
GSL042RCAR Gloria Carrasco, NC HOUSE OF REPRESENTATIVES DISTRICT 042             
GSL043DFLO Elmer Floyd, NC HOUSE OF REPRESENTATIVES DISTRICT 043                 
GSL043RWHE Diane Wheatley, NC HOUSE OF REPRESENTATIVES DISTRICT 043              
GSL044DSMI Charles Smith, NC HOUSE OF REPRESENTATIVES DISTRICT 044               
GSL045DJAC Frances Jackson, NC HOUSE OF REPRESENTATIVES DISTRICT 045             
GSL045RCHA Susan Chapman, NC HOUSE OF REPRESENTATIVES DISTRICT 045               
GSL046RJON Brenden H. Jones, NC HOUSE OF REPRESENTATIVES DISTRICT 046            
GSL047DTOW Charles Townsend, NC HOUSE OF REPRESENTATIVES DISTRICT 047            
GSL047RLOW Jarrod Lowery, NC HOUSE OF REPRESENTATIVES DISTRICT 047               
GSL048DPIE Garland E. Pierce, NC HOUSE OF REPRESENTATIVES DISTRICT 048           
GSL048RSWA Melissa Swarbrick, NC HOUSE OF REPRESENTATIVES DISTRICT 048           
GSL049DBAL Cynthia Ball, NC HOUSE OF REPRESENTATIVES DISTRICT 049                
GSL049LOAK Michael Oakes, NC HOUSE OF REPRESENTATIVES DISTRICT 049               
GSL049RROB David Robertson, NC HOUSE OF REPRESENTATIVES DISTRICT 049             
GSL050DPRI Renee Price, NC HOUSE OF REPRESENTATIVES DISTRICT 050                 
GSL050RLOP Charles Lopez, NC HOUSE OF REPRESENTATIVES DISTRICT 050               
GSL051DHAL Malcolm Hall, NC HOUSE OF REPRESENTATIVES DISTRICT 051                
GSL051RSAU John Sauls, NC HOUSE OF REPRESENTATIVES DISTRICT 051                  
GSL052RMOS Ben Moss, NC HOUSE OF REPRESENTATIVES DISTRICT 052                    
GSL053DTHU Kevin G. Thurman, NC HOUSE OF REPRESENTATIVES DISTRICT 053            
GSL053RPEN Howard Penny, Jr., NC HOUSE OF REPRESENTATIVES DISTRICT 053           
GSL054DREI Robert T. Reives, NC HOUSE OF REPRESENTATIVES DISTRICT 054            
GSL054RPET Walter Petty, NC HOUSE OF REPRESENTATIVES DISTRICT 054                
GSL055RBRO Mark Brody, NC HOUSE OF REPRESENTATIVES DISTRICT 055                  
GSL056DBUA Allen Buansi, NC HOUSE OF REPRESENTATIVES DISTRICT 056                
GSL057DCLE Ashton Clemmons, NC HOUSE OF REPRESENTATIVES DISTRICT 057             
GSL057RBAR Michelle C. Bardsley, NC HOUSE OF REPRESENTATIVES DISTRICT 057        
GSL058DQUI Amos Quick, NC HOUSE OF REPRESENTATIVES DISTRICT 058                  
GSL058RSMI Chrissy Smith, NC HOUSE OF REPRESENTATIVES DISTRICT 058               
GSL059DYOU Sherrie Young, NC HOUSE OF REPRESENTATIVES DISTRICT 059               
GSL059RHAR Jon Hardister, NC HOUSE OF REPRESENTATIVES DISTRICT 059               
GSL060DBRO Cecil Brockman, NC HOUSE OF REPRESENTATIVES DISTRICT 060              
GSL060RBLA Bob Blasingame, NC HOUSE OF REPRESENTATIVES DISTRICT 060              
GSL061DHAR Mary Price (Pricey) Harrison, NC HOUSE OF REPRESENTATIVES DISTRICT 061
GSL062DGRA Brandon Gray, NC HOUSE OF REPRESENTATIVES DISTRICT 062                
GSL062RFAI John Faircloth, NC HOUSE OF REPRESENTATIVES DISTRICT 062              
GSL063DHUR Ricky Hurtado, NC HOUSE OF REPRESENTATIVES DISTRICT 063               
GSL063RROS Stephen Ross, NC HOUSE OF REPRESENTATIVES DISTRICT 063                
GSL064DOSB Ron Osborne, NC HOUSE OF REPRESENTATIVES DISTRICT 064                 
GSL064RRID Dennis Riddell, NC HOUSE OF REPRESENTATIVES DISTRICT 064              
GSL065DDON Jay Donecker, NC HOUSE OF REPRESENTATIVES DISTRICT 065                
GSL065RPYR Reece Pyrtle, NC HOUSE OF REPRESENTATIVES DISTRICT 065                
GSL066DCRA Sarah Crawford, NC HOUSE OF REPRESENTATIVES DISTRICT 066              
GSL066LPEN Micao Penaflor, NC HOUSE OF REPRESENTATIVES DISTRICT 066              
GSL066RSHO Ives Brizuela de Sholar, NC HOUSE OF REPRESENTATIVES DISTRICT 066     
GSL067RSAS Wayne Sasser, NC HOUSE OF REPRESENTATIVES DISTRICT 067                
GSL068RWIL David Willis, NC HOUSE OF REPRESENTATIVES DISTRICT 068                
GSL069DCOU Leigh Coulter, NC HOUSE OF REPRESENTATIVES DISTRICT 069               
GSL069RARP Dean Arp, NC HOUSE OF REPRESENTATIVES DISTRICT 069                    
GSL070DSCO Susan Lee (Susie) Scott, NC HOUSE OF REPRESENTATIVES DISTRICT 070     
GSL070RBIG Brian Biggs, NC HOUSE OF REPRESENTATIVES DISTRICT 070                 
GSL071DBRO Kanika Brown, NC HOUSE OF REPRESENTATIVES DISTRICT 071                
GSL072DBAK Amber M. Baker, NC HOUSE OF REPRESENTATIVES DISTRICT 072              
GSL072RSTA Shelton Stallworthy, NC HOUSE OF REPRESENTATIVES DISTRICT 072         
GSL073DSTA Diamond Staton-Williams, NC HOUSE OF REPRESENTATIVES DISTRICT 073     
GSL073RECH Brian Echevarria, NC HOUSE OF REPRESENTATIVES DISTRICT 073            
GSL074DDAY Carla Catalan Day, NC HOUSE OF REPRESENTATIVES DISTRICT 074           
GSL074RZEN Jeff Zenger, NC HOUSE OF REPRESENTATIVES DISTRICT 074                 
GSL075RLAM Donny C. Lambeth, NC HOUSE OF REPRESENTATIVES DISTRICT 075            
GSL076RWAR Harry Warren, NC HOUSE OF REPRESENTATIVES DISTRICT 076                
GSL077RHOW Julia C. Howard, NC HOUSE OF REPRESENTATIVES DISTRICT 077             
GSL078DDAV Erik Davis, NC HOUSE OF REPRESENTATIVES DISTRICT 078                  
GSL078RJAC Neal Jackson, NC HOUSE OF REPRESENTATIVES DISTRICT 078                
GSL079RKID Keith Kidwell, NC HOUSE OF REPRESENTATIVES DISTRICT 079               
GSL080DMIL Dennis S. Miller, NC HOUSE OF REPRESENTATIVES DISTRICT 080            
GSL080RWAT Sam Watford, NC HOUSE OF REPRESENTATIVES DISTRICT 080                 
GSL081DWAT Joe Watkins, NC HOUSE OF REPRESENTATIVES DISTRICT 081                 
GSL081RPOT Larry W. Potts, NC HOUSE OF REPRESENTATIVES DISTRICT 081              
GSL082RBAK Kristin Baker, NC HOUSE OF REPRESENTATIVES DISTRICT 082               
GSL083RCRU Kevin Crutchfield, NC HOUSE OF REPRESENTATIVES DISTRICT 083           
GSL084RMCN Jeffrey C. McNeely, NC HOUSE OF REPRESENTATIVES DISTRICT 084          
GSL085DCOR Robert Cordle, NC HOUSE OF REPRESENTATIVES DISTRICT 085               
GSL085RGRE Dudley Greene, NC HOUSE OF REPRESENTATIVES DISTRICT 085               
GSL086RBLA Hugh Blackwell, NC HOUSE OF REPRESENTATIVES DISTRICT 086              
GSL087DKIR Barbara Kirby, NC HOUSE OF REPRESENTATIVES DISTRICT 087               
GSL087RHAL Destin Hall, NC HOUSE OF REPRESENTATIVES DISTRICT 087                 
GSL088DBEL Mary Belk, NC HOUSE OF REPRESENTATIVES DISTRICT 088                   
GSL088RPEA Anne Marie Peacock, NC HOUSE OF REPRESENTATIVES DISTRICT 088          
GSL089RSET Mitchell Smith Setzer, NC HOUSE OF REPRESENTATIVES DISTRICT 089       
GSL090RSTE Sarah Stevens, NC HOUSE OF REPRESENTATIVES DISTRICT 090               
GSL091RHAL Kyle Hall, NC HOUSE OF REPRESENTATIVES DISTRICT 091                   
GSL092DBRO Terry Brown, NC HOUSE OF REPRESENTATIVES DISTRICT 092                 
GSL092RROB Mario J. Robinson, Sr., NC HOUSE OF REPRESENTATIVES DISTRICT 092      
GSL093DMAS Ben Massey, NC HOUSE OF REPRESENTATIVES DISTRICT 093                  
GSL093RPIC Ray Pickett, NC HOUSE OF REPRESENTATIVES DISTRICT 093                 
GSL094DHUB Chuck Hubbard, NC HOUSE OF REPRESENTATIVES DISTRICT 094               
GSL094RELM Jeffrey Elmore, NC HOUSE OF REPRESENTATIVES DISTRICT 094              
GSL095DKOT Amanda B. Kotis, NC HOUSE OF REPRESENTATIVES DISTRICT 095             
GSL095RMIL Grey Mills, NC HOUSE OF REPRESENTATIVES DISTRICT 095                  
GSL096RADA Jay Adams, NC HOUSE OF REPRESENTATIVES DISTRICT 096                   
GSL097RSAI Jason R. Saine, NC HOUSE OF REPRESENTATIVES DISTRICT 097              
GSL098DCLA Christy Clark, NC HOUSE OF REPRESENTATIVES DISTRICT 098               
GSL098RBRA John R. Bradford III, NC HOUSE OF REPRESENTATIVES DISTRICT 098        
GSL099DMAJ Nasif Majeed, NC HOUSE OF REPRESENTATIVES DISTRICT 099                
GSL099RAND Michael Anderson, NC HOUSE OF REPRESENTATIVES DISTRICT 099            
GSL100DAUT John Autry, NC HOUSE OF REPRESENTATIVES DISTRICT 100                  
GSL101DLOG Carolyn G. Logan, NC HOUSE OF REPRESENTATIVES DISTRICT 101            
GSL101RMAU Steve Mauney, NC HOUSE OF REPRESENTATIVES DISTRICT 101                
GSL102DCAR Becky Carney, NC HOUSE OF REPRESENTATIVES DISTRICT 102                
GSL102RCLE Cynthia Eleanor Clementi, NC HOUSE OF REPRESENTATIVES DISTRICT 102    
GSL103DBUD Laura Budd, NC HOUSE OF REPRESENTATIVES DISTRICT 103                  
GSL103RBRA Bill Brawley, NC HOUSE OF REPRESENTATIVES DISTRICT 103                
GSL104DLOF Brandon Lofton, NC HOUSE OF REPRESENTATIVES DISTRICT 104              
GSL104RPOM Don Pomeroy, NC HOUSE OF REPRESENTATIVES DISTRICT 104                 
GSL105DHAR Wesley Harris, NC HOUSE OF REPRESENTATIVES DISTRICT 105               
GSL105RNID Joshua Niday, NC HOUSE OF REPRESENTATIVES DISTRICT 105                
GSL106DCUN Carla Cunningham, NC HOUSE OF REPRESENTATIVES DISTRICT 106            
GSL106RHEN Karen Henning, NC HOUSE OF REPRESENTATIVES DISTRICT 106               
GSL107DALE Kelly Alexander, NC HOUSE OF REPRESENTATIVES DISTRICT 107             
GSL107RCOO Mark Alan Cook, NC HOUSE OF REPRESENTATIVES DISTRICT 107              
GSL108RTOR John A. Torbett, NC HOUSE OF REPRESENTATIVES DISTRICT 108             
GSL109DHUG Eric Hughes, NC HOUSE OF REPRESENTATIVES DISTRICT 109                 
GSL109RLOF Donnie Loftis, NC HOUSE OF REPRESENTATIVES DISTRICT 109               
GSL110RHAS Kelly Hastings, NC HOUSE OF REPRESENTATIVES DISTRICT 110              
GSL111RMOO Tim Moore, NC HOUSE OF REPRESENTATIVES DISTRICT 111                   
GSL112DCOT Tricia Cotham, NC HOUSE OF REPRESENTATIVES DISTRICT 112               
GSL112RLON Tony Long, NC HOUSE OF REPRESENTATIVES DISTRICT 112                   
GSL113RJOH Jake Johnson, NC HOUSE OF REPRESENTATIVES DISTRICT 113                
GSL114DAGE J. Eric Ager, NC HOUSE OF REPRESENTATIVES DISTRICT 114                
GSL114RPIT Everett D. Pittillo, NC HOUSE OF REPRESENTATIVES DISTRICT 114         
GSL115DPRA Lindsey Prather, NC HOUSE OF REPRESENTATIVES DISTRICT 115             
GSL115RBHA Pratik Bhakta, NC HOUSE OF REPRESENTATIVES DISTRICT 115               
GSL116DRUD Caleb Rudow, NC HOUSE OF REPRESENTATIVES DISTRICT 116                 
GSL116RROS Mollie Rose, NC HOUSE OF REPRESENTATIVES DISTRICT 116                 
GSL117DOSH Michael Greer O'Shea, NC HOUSE OF REPRESENTATIVES DISTRICT 117        
GSL117RBAL Jennifer Capps Balkcom, NC HOUSE OF REPRESENTATIVES DISTRICT 117      
GSL118DREM Josh Remillard, NC HOUSE OF REPRESENTATIVES DISTRICT 118              
GSL118RPLE Mark Pless, NC HOUSE OF REPRESENTATIVES DISTRICT 118                  
GSL119DPLA Al Platt, NC HOUSE OF REPRESENTATIVES DISTRICT 119                    
GSL119RCLA Mike Clampitt, NC HOUSE OF REPRESENTATIVES DISTRICT 119               
GSL120RGIL Karl E. Gillespie, NC HOUSE OF REPRESENTATIVES DISTRICT 120           

***nc_gen_22_sldu_prec.shp***
SLDU_DIST  State Senate District
GSU01RSAN  Norman W. Sanderson, NC STATE SENATE DISTRICT 01                      
GSU02RPER  Jim Perry, NC STATE SENATE DISTRICT 02                                
GSU03DJOR  Valerie Jordan, NC STATE SENATE DISTRICT 03                           
GSU03RHAN  Bobby Hanig, NC STATE SENATE DISTRICT 03                              
GSU04DFIT  Milton F. (Toby) Fitch, NC STATE SENATE DISTRICT 04                   
GSU04RNEW  Buck Newton, NC STATE SENATE DISTRICT 04                              
GSU05DSMI  Kandie D. Smith, NC STATE SENATE DISTRICT 05                          
GSU05RKOZ  Karen Kozel, NC STATE SENATE DISTRICT 05                              
GSU06RLAZ  Michael A. Lazzara, NC STATE SENATE DISTRICT 06                       
GSU07DMOR  Marcia Morgan, NC STATE SENATE DISTRICT 07                            
GSU07RLEE  Michael Lee, NC STATE SENATE DISTRICT 07                              
GSU08RRAB  Bill Rabon, NC STATE SENATE DISTRICT 08                               
GSU09RJAC  Brent Jackson, NC STATE SENATE DISTRICT 09                            
GSU10DCOH  Gettys Cohen, Jr., NC STATE SENATE DISTRICT 10                        
GSU10RSAW  Benton Sawrey, NC STATE SENATE DISTRICT 10                            
GSU11DSPE  Mark Speed, NC STATE SENATE DISTRICT 11                               
GSU11RBAR  Lisa Stone Barnes, NC STATE SENATE DISTRICT 11                        
GSU12DCHA  Richard Chapman, NC STATE SENATE DISTRICT 12                          
GSU12RBUR  Jim Burgin, NC STATE SENATE DISTRICT 12                               
GSU13DGRA  Lisa Grafstein, NC STATE SENATE DISTRICT 13                           
GSU13LMUN  Michael C. Munger, NC STATE SENATE DISTRICT 13                        
GSU13RBAN  David Bankert, NC STATE SENATE DISTRICT 13                            
GSU14DBLU  Dan Blue, NC STATE SENATE DISTRICT 14                                 
GSU14LLAS  Matthew Laszacs, NC STATE SENATE DISTRICT 14                          
GSU14RBAK  Chris Baker, NC STATE SENATE DISTRICT 14                              
GSU15DCHA  Jay J. Chaudhuri, NC STATE SENATE DISTRICT 15                         
GSU15LBRO  Sammie Brooks, NC STATE SENATE DISTRICT 15                            
GSU15RPRI  Emanuela Prister, NC STATE SENATE DISTRICT 15                         
GSU16DADC  Gale Adcock, NC STATE SENATE DISTRICT 16                              
GSU16GTRU  Michael Trudeau, NC STATE SENATE DISTRICT 16                          
GSU16LWAT  Dee Watson, NC STATE SENATE DISTRICT 16                               
GSU16RPOW  James Powers, NC STATE SENATE DISTRICT 16                             
GSU17DBAT  Mrs. Sydney Batch, NC STATE SENATE DISTRICT 17                        
GSU17LBOW  Patrick J. Bowersox, NC STATE SENATE DISTRICT 17                      
GSU17RCAV  Mark Cavaliero, NC STATE SENATE DISTRICT 17                           
GSU18DBOD  Mary Wills Bode, NC STATE SENATE DISTRICT 18                          
GSU18LBRO  Ryan Brown, NC STATE SENATE DISTRICT 18                               
GSU18RSYK  E. C. Sykes, NC STATE SENATE DISTRICT 18                              
GSU19DAPP  Val Applewhite, NC STATE SENATE DISTRICT 19                           
GSU19RMER  Wesley Meredith, NC STATE SENATE DISTRICT 19                          
GSU20DMUR  Natalie S. Murdock, NC STATE SENATE DISTRICT 20                       
GSU20RREE  Alvin Reed, NC STATE SENATE DISTRICT 20                               
GSU21DMCN  Frank McNeill, NC STATE SENATE DISTRICT 21                            
GSU21RMCI  Tom McInnis, NC STATE SENATE DISTRICT 21                              
GSU22DWOO  Mike Woodard, NC STATE SENATE DISTRICT 22                             
GSU22LUBI  Ray Ubinger, NC STATE SENATE DISTRICT 22                              
GSU22RCOL  Larry Coleman, NC STATE SENATE DISTRICT 22                            
GSU23DMEY  Graig R. Meyer, NC STATE SENATE DISTRICT 23                           
GSU23RWOO  Landon Woods, NC STATE SENATE DISTRICT 23                             
GSU24DGIB  Darrel (BJ) Gibson, Jr., NC STATE SENATE DISTRICT 24                  
GSU24RBRI  Danny Earl Britt, Jr., NC STATE SENATE DISTRICT 24                    
GSU25DEWI  Sean C. Ewing, NC STATE SENATE DISTRICT 25                            
GSU25RGAL  Amy Scott Galey, NC STATE SENATE DISTRICT 25                          
GSU26OWRI  Write-In (Miscellaneous), NC STATE SENATE DISTRICT 26                 
GSU26RBER  Philip E. (Phil) Berger, NC STATE SENATE DISTRICT 26                  
GSU27DGAR  Michael Garrett, NC STATE SENATE DISTRICT 27                          
GSU27RSES  Richard (Josh) Sessoms, NC STATE SENATE DISTRICT 27                   
GSU28DROB  Gladys A. Robinson, NC STATE SENATE DISTRICT 28                       
GSU28RSCH  Paul Schumacher, NC STATE SENATE DISTRICT 28                          
GSU29DCRU  Brooke Crump, NC STATE SENATE DISTRICT 29                             
GSU29RCRA  David (Dave) Craven, Jr., NC STATE SENATE DISTRICT 29                 
GSU30DJOH  Monique D. Johnson, NC STATE SENATE DISTRICT 30                       
GSU30RJAR  Steve Jarvis, NC STATE SENATE DISTRICT 30                             
GSU31RKRA  Joyce Krawiec, NC STATE SENATE DISTRICT 31                            
GSU32DLOW  Paul Lowe, Jr., NC STATE SENATE DISTRICT 32                           
GSU32RWAR  George K. Ware, NC STATE SENATE DISTRICT 32                           
GSU33DHOR  Tangela (Lucy Horne) Morgan, NC STATE SENATE DISTRICT 33              
GSU33RFOR  Carl Ford, NC STATE SENATE DISTRICT 33                                
GSU34DSAN  Keshia Sandidge, NC STATE SENATE DISTRICT 34                          
GSU34RNEW  Paul R. Newton, NC STATE SENATE DISTRICT 34                           
GSU35RJOH  Todd Johnson, NC STATE SENATE DISTRICT 35                             
GSU36RSET  Eddie Settle, NC STATE SENATE DISTRICT 36                             
GSU37RSAW  Vickie Sawyer, NC STATE SENATE DISTRICT 37                            
GSU38DMOH  Mujtaba A. Mohammed, NC STATE SENATE DISTRICT 38                      
GSU39DSAL  DeAndrea Salvador, NC STATE SENATE DISTRICT 39                        
GSU39RROB  Mark Robeson, NC STATE SENATE DISTRICT 39                             
GSU40DWAD  Joyce Waddell, NC STATE SENATE DISTRICT 40                            
GSU40RSHI  Bobbie Shields, NC STATE SENATE DISTRICT 40                           
GSU41DMAR  Natasha Marcus, NC STATE SENATE DISTRICT 41                           
GSU41RLEO  Bonni Leone, NC STATE SENATE DISTRICT 41                              
GSU42DHUN  Rachel Hunt, NC STATE SENATE DISTRICT 42                              
GSU42RRUS  Cheryl Russo, NC STATE SENATE DISTRICT 42                             
GSU43ROVE  Brad Overcash, NC STATE SENATE DISTRICT 43                            
GSU44RALE  Ted Alexander, NC STATE SENATE DISTRICT 44                            
GSU45RPRO  Dean Proctor, NC STATE SENATE DISTRICT 45                             
GSU46DMAR  Billy Martin, NC STATE SENATE DISTRICT 46                             
GSU46RDAN  Warren Daniel, NC STATE SENATE DISTRICT 46                            
GSU47RHIS  Ralph Hise, NC STATE SENATE DISTRICT 47                               
GSU48DCAR  Jay Carey, NC STATE SENATE DISTRICT 48                                
GSU48RMOF  Tim Moffitt, NC STATE SENATE DISTRICT 48                              
GSU49DMAY  Julie Mayfield, NC STATE SENATE DISTRICT 49                           
GSU49RAND  John Anderson, NC STATE SENATE DISTRICT 49                            
GSU50DMCC  Karen Burnette McCracken, NC STATE SENATE DISTRICT 50                 
GSU50RCOR  Kevin Corbin, NC STATE SENATE DISTRICT 50                                   
                          
                                                   
## Processing Steps
Visit the RDH GitHub and the processing script for this code [here](https://github.com/nonpartisan-redistricting-datahub/pber_collection)

## Additional Notes

North Carolina provides "sorted" and "unsorted" results - one file where absentee and one-stop votes are assigned to the correct precincts, with noise then injected for anonymity, and one where no noise is injected, but those results are reported at the county-level. For this file we combined the two - using the sorted for counties impacted and unsorted for non-impacted counties. 

Precincts 01-07A, 07-07A and CV-Carolina did not appear in the NCSBE-provided shapefile, but were in the election results. The RDH pulled these shapes from the 2020 precinct boundary file provided by VEST (https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/K7760H)

For the Congressional, state lower and state upper files, our assigned districts are compared against the official maps. The differences are plotted in the various notebooks. Because we do not split precincts by district when no votes occur, we do not expect the assignments to match exactly, but they should be very close.

Please direct questions related to processing this dataset to info@redistrictingdatahub.org.
