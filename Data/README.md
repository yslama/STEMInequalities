# Data 
Data dictionary

RT         1      
    Record Type			
           H .Housing Record or Group Quarters Unit

SERIALNO   7      
    Housing unit/GQ person serial number    
           0000001..9999999 .Unique identifier

DIVISION   1      
    Division code
           0 .Puerto Rico
           1 .New England (Northeast region)
           2 .Middle Atlantic (Northeast region)
           3 .East North Central (Midwest region)
           4 .West North Central (Midwest region)
           5 .South Atlantic (South region)       
           6 .East South Central (South region)
           7 .West South Central (South Region)
           8 .Mountain (West region)
           9 .Pacific (West region)

PUMA       5      
    Public use microdata area code (PUMA) based on 2010 Census definition          
           00100..70301 .Public use microdata area codes
           		 
Note: Public use microdata areas (PUMAs) designate areas of 100,000 or more population.  Use with ST for unique code.

REGION     1      
    Region code
           1 .Northeast
           2 .Midwest
           3 .South
           4 .West
           9 .Puerto Rico

ST         2      
    State Code
           01 .Alabama/AL                              
           02 .Alaska/AK                               
           04 .Arizona/AZ                              
           05 .Arkansas/AR                             
           06 .California/CA                           
           08 .Colorado/CO                             
           09 .Connecticut/CT                          
           10 .Delaware/DE                             
           11 .District of Columbia/DC                 
           12 .Florida/FL                              
           13 .Georgia/GA                              
           15 .Hawaii/HI                               
           16 .Idaho/ID                                
           17 .Illinois/IL                             
           18 .Indiana/IN                              
           19 .Iowa/IA
           20 .Kansas/KS                               
           21 .Kentucky/KY                             
           22 .Louisiana/LA                            
           23 .Maine/ME                                
           24 .Maryland/MD                             
           25 .Massachusetts/MA                        
           26 .Michigan/MI                             
           27 .Minnesota/MN                            
           28 .Mississippi/MS                          
           29 .Missouri/MO                             
           30 .Montana/MT                              
           31 .Nebraska/NE                             
           32 .Nevada/NV                               
           33 .New Hampshire/NH                        
           34 .New Jersey/NJ                           
           35 .New Mexico/NM                           
           36 .New York/NY                             
           37 .North Carolina/NC                       
           38 .North Dakota/ND                         
           39 .Ohio/OH                                 
           40 .Oklahoma/OK                             
           41 .Oregon/OR                               
           42 .Pennsylvania/PA                         
           44 .Rhode Island/RI                         
           45 .South Carolina/SC                       
           46 .South Dakota/SD                         
           47 .Tennessee/TN                            
           48 .Texas/TX                                
           49 .Utah/UT                                 
           50 .Vermont/VT                              
           51 .Virginia/VA                             
           53 .Washington/WA                           
           54 .West Virginia/WV                        
           55 .Wisconsin/WI                            
           56 .Wyoming/WY                              
           72 .Puerto Rico/PR

ADJHSG     7      
Adjustment factor for housing dollar amounts (6 implied decimal places)
           1000000 .2013 factor (1.000000)

Note: The value of ADJHSG inflation-adjusts reported housing costs to 2013 dollars and applies to variables CONP, ELEP, FULP, GASP, GRNTP, INSP, MHP, MRGP, SMOCP, RNTP, SMP, and WATP in the housing record. ADJHSG does not apply to AGS and TAXP because they are categorical variables that should not be inflation-adjusted. ADJHSG does not apply to VALP. 


ADJINC     7      
Adjustment factor for income and earnings dollar amounts (6 implied decimal places)
           1007549 .2013 factor (1.007549)

Note: The value of ADJINC inflation-adjusts reported income to 2013 dollars.  ADJINC applies to variables FINCP and HINCP in the housing record, and variables INTP, OIP, PAP, PERNP, PINCP, RETP, SEMP, SSIP, SSP, and WAGP in the person record. 

WGTP       5      
    Housing Weight  
                 0000 .Group Quarters place holder record 
         00001..09999 .Integer weight of housing unit

NP         2      
    Number of person records following this housing record
               00 .Vacant unit
               01 .One person record (one person in household or  
                  .any person in group quarters)
           02..20 .Number of person records (number of persons in
                  .household)

TYPE       1      
    Type of unit              
           1 .Housing unit      
           2 .Institutional group quarters
           3 .Noninstitutional group quarters

ACCESS     1      
    Access to the Internet
           b .N/A (GQ)
           1 .Yes, with subscription to an Internet service
           2 .Yes, without a subscription to an Internet service
           3 .No Internet access at this house, apartment, or mobile home

ACR        1      
    Lot size            
           b .N/A (GQ/not a one-family house or mobile home)
           1 .House on less than one acre
           2 .House on one to less than ten acres 
           3 .House on ten or more acres

AGS        1         
    Sales of Agriculture Products (Yearly sales)
           b .N/A (GQ/vacant/not a one family house 
             .or mobile home/less than 1 acre)
           1 .None
           2 .$    1 - $  999
           3 .$ 1000 - $ 2499
           4 .$ 2500 - $ 4999
           5 .$ 5000 - $ 9999
           6 .$10000+  

Note: no adjustment factor is applied to AGS.

BATH       1      
    Bathtub or shower
           b .N/A (GQ)
           1 .Yes
           2 .No

BDSP       2     
    Number of bedrooms
               bb .N/A (GQ)
           00..99 .0 to 99 bedrooms (Top-coded)

BLD        2      
    Units in structure
           bb .N/A (GQ)
           01 .Mobile home or trailer
           02 .One-family house detached
           03 .One-family house attached
           04 .2 Apartments
           05 .3-4 Apartments
           06 .5-9 Apartments
           07 .10-19 Apartments
           08 .20-49 Apartments
           09 .50 or more apartments
           10 .Boat, RV, van, etc.

BROADBND   1      
    Mobile broadband plan
           b .N/A (GQ)
           1 .Yes
           2 .No

BUS        1      
    Business or medical office on property
           b .N/A (GQ/not a one-family house or mobile home)
           1 .Yes
           2 .No

COMPOTHX   1      
    Other computer equipment
           b .N/A (GQ)
           1 .Yes
           2 .No

CONP       4      
    Condo fee (monthly amount)
                 bbbb .N/A (GQ/vacant/not owned or being
                      .bought)
                 0000 .Not condo
           0001..9999 .$1 - $9999 (Rounded and top-coded)
                             
Note: Use ADJHSG to adjust CONP to constant dollars.

DIALUP     1      
    Dial-up service
           b .N/A (GQ)
           1 .Yes
           2 .No

DSL        1      
    DSL service
           b .N/A (GQ)
           1 .Yes
           2 .No

ELEP       3      
    Electricity (monthly cost)
                bbb .N/A (GQ/vacant)
                001 .Included in rent or in condo fee
                002 .No charge or electricity not used
           003..999 .$3 to $999 (Rounded and top-coded)
               
Note: Use ADJHSG to adjust ELEP values 3 and over to constant dollars.

FIBEROP    1      
    Fiber-optic Internet service
           b .N/A (GQ)
           1 .Yes
           2 .No

FS         1
    Yearly food stamp/Supplemental Nutrition Assistance Program recipiency
           b .N/A (vacant)
           1 .Yes
           2 .No

FULP       4      
    Fuel cost(yearly cost for fuels other than gas and electricity)
                 bbbb .N/A (GQ/vacant)
                 0001 .Included in rent or in condo fee
                 0002 .No charge or these fuels not used
           0003..9999 .$3 to $9999 (Rounded and top-coded)

Note: Use ADJHSG to adjust FULP values 3 and over to constant dollars.

GASP       3      
    Gas (monthly cost)
                bbb .N/A (GQ/vacant)                   
                001 .Included in rent or in condo fee
                002 .Included in electricity payment
                003 .No charge or gas not used
           004..999 .$4 to $999 (Rounded and top-coded)

Note: Use ADJHSG to adjust GASP values 4 and over to constant dollars.

HANDHELD   1      
    Handheld computer
           b .N/A (GQ)
           1 .Yes
           2 .No

HFL        1      
    House heating fuel
           b .N/A (GQ/vacant)
           1 .Utility gas 
           2 .Bottled, tank, or LP gas
           3 .Electricity
           4 .Fuel oil, kerosene, etc.
           5 .Coal or coke
           6 .Wood
           7 .Solar energy
           8 .Other fuel
           9 .No fuel used

INSP       5      
    Fire/hazard/flood insurance (yearly amount)
                  bbbbb .N/A (GQ/vacant/not owned or being bought)
                  00000 .None
           00001..10000 .$1 to $10000 (Rounded and top-coded)

Note: Use ADJHSG to adjust INSP to constant dollars.

LAPTOP     1      
    Laptop, desktop, or notebook computer
           b .N/A (GQ)
           1 .Yes
           2 .No

MHP        5      
    Mobile home costs (yearly amount)
                  bbbbb .N/A (GQ/vacant/not owned or being bought/
                        .not mobile home)
     	          00000 .None
           00001..99999 .$1 to $99999 (Rounded and top-coded)
                
Note: Use ADJHSG to adjust MHP to constant dollars.

MODEM      1      
    Cable Internet service
           b .N/A (GQ)
           1 .Yes
           2 .No

MRGI       1      
    First mortgage payment includes fire/hazard/flood insurance
           b .N/A (GQ/vacant/not owned or being bought/not mortgaged)
           1 .Yes, insurance included in payment
           2 .No, insurance paid separately or no insurance

MRGP       5      
    First mortgage payment (monthly amount)
           bbbbb .N/A (GQ/vacant/not owned or being bought/not 
                 .mortgaged)                          
           00001..99999 .$1 to $99999 (Rounded and top-coded)
                
Note: Use ADJHSG to adjust MRGP to constant dollars.

MRGT       1      
    First mortgage payment includes real estate taxes
           b .N/A (GQ/vacant/not owned or being bought/not mortgaged)
           1 .Yes, taxes included in payment
           2 .No, taxes paid separately or taxes not required

MRGX       1      
    First mortgage status
           b .N/A (GQ/vacant/not owned or being bought)
           1 .Mortgage, deed of trust, or similar debt
           2 .Contract to purchase
           3 .None

OTHSVCEX   1      
    Other Internet service
           b .N/A (GQ)
           1 .Yes
           2 .No

REFR       1      
    Refrigerator
           b .N/A (GQ)
           1 .Yes
           2 .No

RMSP       2
    Number of Rooms
               bb .N/A (GQ)
           00..99 .Rooms (Top-coded)

RNTM       1      
    Meals included in rent
           b .N/A (GQ/not a rental unit/occupied without rent payment)
           1 .Yes
           2 .No

RNTP       5      
    Monthly rent
                  bbbbb .N/A (GQ/not a rental unit/occupied without rent
                        .payment)               
           00001..99999 .$1 to $99999 (Rounded and top-coded)

Note: Use ADJHSG to adjust RNTP to constant dollars.

RWAT       1      
    Hot and cold running water
           b .N/A (GQ)
           1 .Yes
           2 .No
	   9. Case is from Puerto Rico, RWAT not applicable

RWATPR     1
    Running water
           b .N/A (GQ)
           1 .Yes
           2 .No
	   9. Case is from the United States, RWATPR not applicable

SATELLITE  1      
    Satellite Internet service
           b .N/A (GQ)
           1 .Yes
           2 .No

SINK       1      
    Sink with a faucet
           b .N/A (GQ)
           1 .Yes
           2 .No

SMP        5      
    Total payment on all second and junior mortgages and home equity loans 
    (monthly amount)
                  bbbbb .N/A (GQ/vacant/not owned or being bought/
                        ./no second or junior mortgages or home equity loans)
           00001..99999 .$1 to $99999 (Rounded and top-coded)

Note: Use ADJHSG to adjust SMP to constant dollars.
       
STOV	   1
    Stove or range
           b .N/A (GQ)
           1 .Yes
           2 .No

TEL        1      
    Telephone 
           b .N/A (GQ/vacant)
           1 .Yes
           2 .No

TEN	   1
    Tenure
           b .N/A  (GQ/vacant)
           1 .Owned with mortgage or loan (include home equity loans)
           2 .Owned free and clear
           3 .Rented
           4 .Occupied without payment of rent

TOIL       1
    Flush toilet
           b .N/A (GQ)
           1 .Yes
           2 .No

VACS       1      
    Vacancy status
           b .N/A (GQ/occupied)
           1 .For rent
           2 .Rented, not occupied
           3 .For sale only
           4 .Sold, not occupied
           5 .For seasonal/recreational/occasional use
           6 .For migrant workers
           7 .Other vacant

VALP       7
    Property value
                    bbbbbbb .N/A (GQ/vacant units, except ”for-sale-only“ and 
                            .”sold, not occupied”/not owned or being bought)
           0000001..9999999 .$1 to $9999999 (Rounded and top-coded)

VEH        1      
    Vehicles (1 ton or less) available
           b .N/A (GQ/vacant)
           0 .No vehicles
           1 .1 vehicle
           2 .2 vehicles
           3 .3 vehicles
           4 .4 vehicles
           5 .5 vehicles
           6 .6 or more vehicles

WATP       4      
    Water (yearly cost)
                 bbbb .N/A (GQ/vacant)
                 0001 .Included in rent or in condo fee
                 0002 .No charge
           0003..9999 .$3 to $9999 (Rounded and top-coded)
                
Note: Use ADJHSG to adjust WATP values 3 and over to constant dollars.

YBL        2
    When structure first built
           bb .N/A (GQ)
           01 .1939 or earlier
           02 .1940 to 1949
           03 .1950 to 1959
           04 .1960 to 1969
           05 .1970 to 1979
           06 .1980 to 1989
           07 .1990 to 1999
           08 .2000 to 2004
           09 .2005
           10 .2006
           11 .2007
           12 .2008
           13 .2009
           14 .2010
	   15 .2011
	   16 .2012
           17 .2013

FES        1      
    Family type and employment status    
           b .N/A (GQ/vacant/not a family)
           1 .Married-couple family: Husband and wife in LF
           2 .Married-couple family: Husband in labor force, wife
             .not in LF
           3 .Married-couple family: Husband not in LF,
             .wife in LF
           4 .Married-couple family: Neither husband nor wife in
             .LF
           5 .Other family: Male householder, no wife present, in
             .LF
           6 .Other family: Male householder, no wife present, 
             .not in LF
           7 .Other family: Female householder, no husband
             .present, in LF
           8 .Other family: Female householder, no husband     
             .present, not in LF    

FINCP      9
    Family income (past 12 months)
                      bbbbbbbbb .N/A(GQ/vacant)   
                      000000000 .No family income
                      -00059999 .Loss of -$59,999 or more
           -00000001..-00059998 .Loss of $1 to -$59,998
                      000000001 .$1 or Break even
           000000002..999999999 .Total family income in dollars (Components 
                                .are rounded) 

Note: Use ADJINC to adjust FINCP to constant dollars.

FPARC      1      
    Family presence and age of related children
           b .N/A (GQ/vacant/not a family)
           1 .With related children under 5 years only
           2 .With related children 5 to 17 years only
           3 .With related children under 5 years and 5 to 17 years
           4 .No related children

GRNTP      5      
    Gross rent (monthly amount)
                  bbbbb .N/A (GQ/vacant/not a rental unit/occupied without
                        .rent payment)
           00001..99999 .$1 - $99999 (Components are rounded)

Note: Use ADJHSG to adjust GRNTP to constant dollars.

GRPIP      3      
    Gross rent as a percentage of household income past 12 months   
                bbb .N/A (GQ/vacant/not a rental unit/occupied without         
                    .rent payment/no household income)
           001..100 .1% to 100%
                101 .101% or more

HHL        1
    Household language
           b .N/A (GQ/vacant)                     
           1 .English only
           2 .Spanish
           3 .Other Indo-European languages
           4 .Asian and Pacific Island languages
           5 .Other language 

HHT        1      
    Household/family type
           b .N/A (GQ/vacant)
           1 .Married couple household 
           2 .Other family household:Male householder, no wife present
           3 .Other family household:Female householder, no husband present 
           4 .Nonfamily household:Male householder:Living alone
           5 .Nonfamily household:Male householder:Not living alone 
           6 .Nonfamily household:Female householder:Living alone
           7 .Nonfamily household:Female householder:Not living alone

HINCP      9      
    Household income (past 12 months)
                      bbbbbbbbb .N/A(GQ/vacant)
                      000000000 .No household income
                      -00059999 .Loss of -$59,999 or more
           -00000001..-00059998 .Loss of $1 to -$59,998
                      000000001 .$1 or Break even
           000000002..999999999 .Total household income in dollars 
                                .(Components are rounded)

Note: Use ADJINC to adjust HINCP to constant dollars.

HUGCL      1      
    Household with grandparent living with grandchildren
           b .N/A (GQ/vacant)
           0 .Household without grandparent living with grandchildren
           1 .Household with grandparent living with grandchildren   
 
HUPAC      1      
    HH presence and age of children
           b .N/A (GQ/vacant)
           1 .With children under 6 years only
           2 .With children 6 to 17 years only
           3 .With children under 6 years and 6 to 17 years
           4 .No children 

HUPAOC     1      
    HH presence and age of own children
           b .N/A (GQ/vacant)
           1 .Presence of own children under 6 years only
           2 .Presence of own children 6 to 17 years only
           3 .Presence of own children under 6 years and 6 to 17 years
           4 .No own children present

HUPARC     1      
    HH presence and age of related children
           b .N/A (GQ/vacant)
           1 .Presence of related children under 6 years only
           2 .Presence of related children 6 to 17 years only
           3 .Presence of related children under 6 years and 6 to 17 years
           4 .No related children present

KIT        1      
    Complete kitchen facilities
           b .N/A (GQ)
           1 .Yes, has stove or range, refrigerator, and sink with a faucet
           2 .No

LNGI       1      
    Limited English speaking households
           b .N/A (GQ/vacant)
           1 .At least one person in the household 14 and over speaks English
             .only or speaks English 'very well'
           2 .No one in the household 14 and over speaks English only or 
             .speaks English 'very well'	

MULTG      1
    Multigenerational Household
           b .N/A (GQ/Vacant/NP=0)
           1 .No, not a multigenerational household
           2 .Yes, is a multigenerational household

MV         1       
    When moved into this house or apartment
           b .N/A (GQ/vacant)
           1 .12 months or less
           2 .13 to 23 months
           3 .2 to 4 years
           4 .5 to 9 years
           5 .10 to 19 years
           6 .20 to 29 years 
           7 .30 years or more

NOC        2      
    Number of own children in household (unweighted)
               bb .N/A(GQ/vacant)
               00 .No own children
           01..19 .Number of own children in household

NPF        2      
    Number of persons in family (unweighted)
               bb .N/A (GQ/vacant/non-family household)
           02..20 .Number of persons in family

NPP        1      
    Grandparent headed household with no parent present
           b .N/A (GQ/vacant)
           0 .Not a grandparent headed household with no parent present
           1 .Grandparent headed household with no parent present

NR         1      
    Presence of nonrelative in household
           b .N/A (GQ/vacant)
           0 .None                                                     
           1 .1 or more nonrelatives                             

NRC        2      
    Number of related children in household (unweighted)
               bb .N/A (GQ/vacant)
               00 .No related children
           01..19 .Number of related children in household

OCPIP      3      
    Selected monthly owner costs as a percentage of household 
    income during the past 12 months   
                bbb .N/A (GQ/vacant/not owned or being bought/    
                    .no household income)
           001..100 .1% to 100%
                101 .101% or more

PARTNER    1      
    Unmarried partner household          
           b .N/A (GQ/vacant)
           0 .No unmarried partner in household                        
           1 .Male householder, male partner                     
           2 .Male householder, female partner
           3 .Female householder, female partner
           4 .Female householder, male partner

PLM        1      
    Complete plumbing facilities
           b .N/A (GQ)
           1 .Yes, has hot and cold running water, a flush toilet, and a
             .bathtub or shower
           2 .No
	   9 .Case is from Puerto Rico, PLM recode not applicable 

PSF        1      
    Presence of subfamilies in Household
           b .N/A (GQ/vacant)
           0 .No subfamilies
           1 .1 or more subfamilies

R18        1      
    Presence of persons under 18 years in household (unweighted)
           b .N/A (GQ/vacant)
           0 .No person under 18 in household
           1 .1 or more persons under 18 in household

R60        1      
    Presence of persons 60 years and over in household (unweighted)
           b .N/A (GQ/vacant)
           0 .No person 60 and over
           1 .1 person 60 and over
           2 .2 or more persons 60 and over

R65        1      
    Presence of persons 65 years and over in household (unweighted)
           b .N/A (GQ/vacant)
           0 .No person 65 and over
           1 .1 person 65 and over
           2 .2 or more persons 65 and over

RESMODE    1
    Response mode                      
           b .N/A (GQ)
           1 .Mail                                                     
           2 .CATI/CAPI  
           3 .Internet                                        

SMOCP      5      
    Selected monthly owner costs
                  bbbbb .N/A (GQ/vacant/not owned or being bought)
	          00000 .None
           00001..99999 .$1 - $99999 (Components are rounded) 

Note: Use ADJHSG to adjust SMOCP to constant dollars.

SMX        1      
    Second or junior mortgage or home equity loan status
           b .N/A (GQ/vacant/not owned or being bought)
           1 .Yes, a second mortgage                        
           2 .Yes, a home equity loan
           3 .No
           4 .Both a second mortgage and a home equity loan

SRNT       1      
    Specified rent unit
           b .N/A
           0 .Not specified rent unit
           1 .Specified rent unit

SSMC       1
    Same-sex married couple households  
           0 .Households without a same-sex married couple
           1 .Same-sex married-couple household where not all relevant data 
             .shown as reported
           2 .All other same-sex married-couple households

SVAL       1      
    Specified value owner unit
           b .N/A
           0 .Not specified value owner unit
           1 .Specified value owner unit

TAXP       2      
    Property taxes (yearly amount)   
           bb .N/A (GQ/vacant/not owned or being bought)
           01 .None 
           02 .$   1 - $  49
           03 .$  50 - $  99
           04 .$ 100 - $ 149
           05 .$ 150 - $ 199
           06 .$ 200 - $ 249
           07 .$ 250 - $ 299
           08 .$ 300 - $ 349
           09 .$ 350 - $ 399
           10 .$ 400 - $ 449
           11 .$ 450 - $ 499
           12 .$ 500 - $ 549
           13 .$ 550 - $ 599
           14 .$ 600 - $ 649
           15 .$ 650 - $ 699
           16 .$ 700 - $ 749
           17 .$ 750 - $ 799
           18 .$ 800 - $ 849
           19 .$ 850 - $ 899
           20 .$ 900 - $ 949
           21 .$ 950 - $ 999
           22 .$1000 - $1099
           23 .$1100 - $1199
           24 .$1200 - $1299
           25 .$1300 - $1399
           26 .$1400 - $1499
           27 .$1500 - $1599
           28 .$1600 - $1699
           29 .$1700 - $1799
           30 .$1800 - $1899
           31 .$1900 - $1999
           32 .$2000 - $2099
           33 .$2100 - $2199
           34 .$2200 - $2299
           35 .$2300 - $2399
           36 .$2400 - $2499
           37 .$2500 - $2599
           38 .$2600 - $2699
           39 .$2700 - $2799
           40 .$2800 - $2899
           41 .$2900 - $2999
           42 .$3000 - $3099
           43 .$3100 - $3199
           44 .$3200 - $3299
           45 .$3300 - $3399
           46 .$3400 - $3499
           47 .$3500 - $3599
           48 .$3600 - $3699
           49 .$3700 - $3799
           50 .$3800 - $3899
           51 .$3900 - $3999
           52 .$4000 - $4099
           53 .$4100 - $4199
           54 .$4200 - $4299
           55 .$4300 - $4399
           56 .$4400 - $4499
           57 .$4500 - $4599 
           58 .$4600 - $4699
           59 .$4700 - $4799
           60 .$4800 - $4899
           61 .$4900 - $4999
           62 .$5000 - $5499
           63 .$5500 - $5999
           64 .$6000 - $6999
           65 .$7000 - $7999
           66 .$8000 - $8999
           67 .$9000 - $9999
           68 .$10000+ 	(Top-coded)

Note: No adjustment factor is applied to TAXP.

WIF        1      
    Workers in family during the past 12 months
           b .N/A (GQ/vacant/non-family household)
           0 .No workers
           1 .1 worker
           2 .2 workers
           3 .3 or more workers in family

WKEXREL    2      
    Work experience of householder and spouse
           bb .N/A (GQ/vacant/not a family)
           01 .Householder and spouse worked FT
           02 .Householder worked FT; spouse worked < FT
           03 .Householder worked FT; spouse did not work
           04 .Householder worked < FT; spouse worked FT
           05 .Householder worked < FT; spouse worked < FT
           06 .Householder worked < FT; spouse did not work
           07 .Householder did not work; spouse worked FT
           08 .Householder did not work; spouse worked < FT
           09 .Householder did not work; spouse did not work
           10 .Male householder worked FT; no spouse present
           11 .Male householder worked < FT; no spouse present
           12 .Male householder did not work; no spouse present
           13 .Female householder worked FT; no spouse present
           14 .Female householder worked < FT; no spouse present
           15 .Female householder did not work; no spouse present

WORKSTAT   2      
    Work status of householder or spouse in family households
           bb .N/A (GQ/not a family household)
           01 .Husband and wife both in labor force, both employed or in 
              .Armed Forces
           02 .Husband and wife both in labor force, husband employed or in 
              .Armed Forces, wife unemployed
           03 .Husband in labor force and wife not in labor force, husband     
              .employed or in Armed Forces 
           04 .Husband and wife both in labor force, husband unemployed, wife
              .employed or in Armed Forces 
           05 .Husband and wife both in labor force, husband unemployed, wife
              .unemployed
           06 .Husband in labor force, husband unemployed, wife not in labor
              .force
           07 .Husband not in labor force, wife in labor force, wife       
              .employed or in Armed Forces
           08 .Husband not in labor force, wife in labor force, wife 
              .unemployed
           09 .Neither husband nor wife in labor force
           10 .Male householder with no wife present, householder in 
              .labor force, employed or in Armed Forces
           11 .Male householder with no wife present, householder in
              .labor force and unemployed
           12 .Male householder with no wife present, householder not in 
              .labor force
           13 .Female householder with no husband present, householder in 
              .labor force, employed or in Armed Forces
           14 .Female householder with no husband present, householder in
              .labor force and unemployed
           15 .Female householder with no husband present, householder not in 
              .labor force

FACCESSP   1      
    Access to the Internet allocation flag
           0 .No
           1 .Yes

FACRP      1      
    Lot size allocation flag
           0 .No
           1 .Yes

FAGSP      1      
    Sales of Agricultural Products allocation flag
           0 .No
           1 .Yes

FBATHP     1
    Bathtub or shower allocation flag
           0 .No
           1 .Yes

FBDSP      1      
    Number of bedrooms allocation flag
           0 .No
           1 .Yes

FBLDP      1      
    Units in structure allocation flag
           0 .No
           1 .Yes

FBROADBNDP 1      
    Mobile broadband plan allocation flag
           0 .No
           1 .Yes

FBUSP      1      
    Business or medical office on property allocation flag
           0 .No
           1 .Yes

FCOMPOTHXP 1      
    Other computer equipment allocation flag
           0 .No
           1 .Yes

FCONP      1      
    Condominium fee allocation flag
           0 .No
           1 .Yes

FDIALUPP   1      
    Dial-up service allocation flag
           0 .No
           1 .Yes

FDSLP      1      
    DSL service allocation flag
           0 .No
           1 .Yes

FELEP      1      
    Electricity (monthly cost) allocation flag
           0 .No
           1 .Yes

FFIBEROPP  1      
    Fiber-optic Internet service allocation flag
           0 .No
           1 .Yes

FFINCP     1
       Family income (past 12 months) allocation flag
           0 .No
           1 .Yes

FFSP	   1
    Yearly food stamp/Supplemental Nutrition Assistance Program 
    recipiency allocation flag
           0 .No
           1 .Yes

FFULP      1      
    Fuel cost (yearly cost for fuels other than gas and electricity)
    allocation flag
           0 .No
           1 .Yes

FGASP      1      
    Gas (monthly cost) allocation flag
           0 .No
           1 .Yes

FGRNTP     1
    Gross rent (monthly amount) allocation flag
           0 .No
           1 .Yes

FHANDHELDP 1      
    Handheld computer allocation flag
           0 .No
           1 .Yes

FHFLP      1      					
    House heating fuel allocation flag
           0 .No
           1 .Yes

FHINCP     1
    Household income (past 12 months) allocation flag
           0 .No
           1 .Yes

FINSP      1      
    Fire, hazard, flood insurance (yearly amount) allocation flag
           0 .No
           1 .Yes

FKITP      1      
    Complete kitchen facilities allocation flag
           0 .No
           1 .Yes

FLAPTOPP   1      
    Laptop, desktop, or notebook computer allocation flag
           0 .No
           1 .Yes

FMHP       1      
    Mobile home costs (yearly amount) allocation flag
           0 .No
           1 .Yes

FMODEMP    1      
    Cable Internet service allocation flag
           0 .No
           1 .Yes

FMRGIP     1      
    First mortgage payment includes fire, hazard, flood insurance
    allocation flag
           0 .No
           1 .Yes

FMRGP      1      
    First mortgage payment (monthly amount) allocation flag
           0 .No
           1 .Yes

FMRGTP     1      
    First mortgage payment includes real estate taxes allocation flag
           0 .No
           1 .Yes

FMRGXP     1      
    First mortgage status allocation flag
           0 .No
           1 .Yes
          
FMVP       1      
    When moved into this house or apartment allocation flag
           0 .No
           1 .Yes

FOTHSVCEXP 1      
    Other Internet service allocation flag
           0 .No
           1 .Yes

FPLMP      1      
    Complete plumbing facilities allocation flag
           0 .No
           1 .Yes

FREFRP     1
    Refrigerator allocation flag
           0 .No
           1 .Yes

FRMSP      1      
    Number of rooms allocation flag
           0 .No
           1 .Yes

FRNTMP     1      
    Meals included in rent allocation flag
           0 .No
           1 .Yes

FRNTP      1      
    Monthly rent allocation flag
           0 .No
           1 .Yes

FRWATP     1
    Hot and cold running water allocation flag
           0 .No
           1 .Yes

FRWATPRP   1
    Running water allocation flag
           0 .No
           1 .Yes

FSATELLITEP 1      
    Satellite Internet service allocation flag
            0 .No
            1 .Yes

FSINKP     1
    Sink with a faucet allocation flag
           0 .No
           1 .Yes

FSMOCP     1
    Selected monthly owner cost allocation flag
           0 .No
           1 .Yes

FSMP       1      
    Total payment on second and junior mortgages and home equity loans 
    (monthly amount)allocation flag
           0 .No
           1 .Yes

FSMXHP     1      
    Home equity loan status allocation flag
           0 .No
           1 .Yes

FSMXSP     1      
    Second mortgage status allocation flag
           0 .No
           1 .Yes

FSTOVP     1
    Stove or range allocation flag
           0 .No
           1 .Yes

FTAXP      1      
    Property taxes (yearly amount) allocation flag
           0 .No
           1 .Yes

FTELP      1      
    Telephone allocation flag
           0 .No
           1 .Yes

FTENP      1      
    Tenure allocation flag
           0 .No
           1 .Yes

FTOILP     1
    Flush toilet allocation flag
           0 .No
           1 .Yes

FVACSP     1      
    Vacancy status allocation flag
           0 .No
           1 .Yes

FVALP      1      
    Property value allocation flag
           0 .No
           1 .Yes

FVEHP      1      
    Vehicles available allocation flag
           0 .No
           1 .Yes

FWATP      1      
    Water (yearly cost) allocation flag
           0 .No
           1 .Yes

FYBLP      1      
    When structure first built allocation flag
           0 .No
           1 .Yes

WGTP1      5
    Housing Weight replicate 1
           -9999..09999 .Integer weight of housing unit

WGTP2      5
    Housing Weight replicate 2
           -9999..09999 .Integer weight of housing unit

WGTP3      5
    Housing Weight replicate 3
           -9999..09999 .Integer weight of housing unit

WGTP4      5
    Housing Weight replicate 4
           -9999..09999 .Integer weight of housing unit

WGTP5      5
    Housing Weight replicate 5
           -9999..09999 .Integer weight of housing unit

WGTP6      5
    Housing Weight replicate 6
           -9999..09999 .Integer weight of housing unit

WGTP7      5
    Housing Weight replicate 7
           -9999..09999 .Integer weight of housing unit

WGTP8      5
    Housing Weight replicate 8
           -9999..09999 .Integer weight of housing unit

WGTP9      5
    Housing Weight replicate 9
           -9999..09999 .Integer weight of housing unit

WGTP10     5
    Housing Weight replicate 10
           -9999..09999 .Integer weight of housing unit

WGTP11     5
    Housing Weight replicate 11
           -9999..09999 .Integer weight of housing unit

WGTP12     5
    Housing Weight replicate 12
           -9999..09999 .Integer weight of housing unit

WGTP13     5
    Housing Weight replicate 13
           -9999..09999 .Integer weight of housing unit

WGTP14     5
    Housing Weight replicate 14
           -9999..09999 .Integer weight of housing unit

WGTP15     5
    Housing Weight replicate 15
           -9999..09999 .Integer weight of housing unit

WGTP16     5
    Housing Weight replicate 16
           -9999..09999 .Integer weight of housing unit

WGTP17     5
    Housing Weight replicate 17
           -9999..09999 .Integer weight of housing unit

WGTP18     5
    Housing Weight replicate 18
           -9999..09999 .Integer weight of housing unit

WGTP19     5
    Housing Weight replicate 19
           -9999..09999 .Integer weight of housing unit

WGTP20     5
    Housing Weight replicate 20
           -9999..09999 .Integer weight of housing unit

WGTP21     5
    Housing Weight replicate 21
           -9999..09999 .Integer weight of housing unit

WGTP22     5
    Housing Weight replicate 22
           -9999..09999 .Integer weight of housing unit

WGTP23     5
    Housing Weight replicate 23
           -9999..09999 .Integer weight of housing unit

WGTP24     5
    Housing Weight replicate 24
           -9999..09999 .Integer weight of housing unit

WGTP25     5
    Housing Weight replicate 25
           -9999..09999 .Integer weight of housing unit

WGTP26     5
    Housing Weight replicate 26
           -9999..09999 .Integer weight of housing unit

WGTP27     5
    Housing Weight replicate 27
           -9999..09999 .Integer weight of housing unit

WGTP28     5
    Housing Weight replicate 28
           -9999..09999 .Integer weight of housing unit

WGTP29     5
    Housing Weight replicate 29
           -9999..09999 .Integer weight of housing unit

WGTP30     5
    Housing Weight replicate 30
           -9999..09999 .Integer weight of housing unit

WGTP31     5
    Housing Weight replicate 31
           -9999..09999 .Integer weight of housing unit

WGTP32     5
    Housing Weight replicate 32
           -9999..09999 .Integer weight of housing unit

WGTP33     5
    Housing Weight replicate 33
           -9999..09999 .Integer weight of housing unit

WGTP34     5
    Housing Weight replicate 34
           -9999..09999 .Integer weight of housing unit

WGTP35     5
    Housing Weight replicate 35
           -9999..09999 .Integer weight of housing unit

WGTP36     5
    Housing Weight replicate 36
           -9999..09999 .Integer weight of housing unit

WGTP37     5
    Housing Weight replicate 37
           -9999..09999 .Integer weight of housing unit

WGTP38     5
    Housing Weight replicate 38
           -9999..09999 .Integer weight of housing unit

WGTP39     5
    Housing Weight replicate 39
           -9999..09999 .Integer weight of housing unit

WGTP40     5
    Housing Weight replicate 40
           -9999..09999 .Integer weight of housing unit

WGTP41     5
    Housing Weight replicate 41
           -9999..09999 .Integer weight of housing unit

WGTP42     5
    Housing Weight replicate 42
           -9999..09999 .Integer weight of housing unit

WGTP43     5
    Housing Weight replicate 43
           -9999..09999 .Integer weight of housing unit

WGTP44     5
    Housing Weight replicate 44
           -9999..09999 .Integer weight of housing unit

WGTP45     5
    Housing Weight replicate 45
           -9999..09999 .Integer weight of housing unit

WGTP46     5
    Housing Weight replicate 46
           -9999..09999 .Integer weight of housing unit

WGTP47     5
    Housing Weight replicate 47
           -9999..09999 .Integer weight of housing unit

WGTP48     5
    Housing Weight replicate 48
           -9999..09999 .Integer weight of housing unit

WGTP49     5
    Housing Weight replicate 49
           -9999..09999 .Integer weight of housing unit

WGTP50     5
    Housing Weight replicate 50
           -9999..09999 .Integer weight of housing unit

WGTP51     5
    Housing Weight replicate 51
           -9999..09999 .Integer weight of housing unit

WGTP52     5
    Housing Weight replicate 52
           -9999..09999 .Integer weight of housing unit

WGTP53     5
    Housing Weight replicate 53
           -9999..09999 .Integer weight of housing unit

WGTP54     5
    Housing Weight replicate 54

           -9999..09999 .Integer weight of housing unit

WGTP55     5
    Housing Weight replicate 55
           -9999..09999 .Integer weight of housing unit

WGTP56     5
    Housing Weight replicate 56
           -9999..09999 .Integer weight of housing unit

WGTP57     5
    Housing Weight replicate 57
           -9999..09999 .Integer weight of housing unit

WGTP58     5
    Housing Weight replicate 58
           -9999..09999 .Integer weight of housing unit

WGTP59     5
    Housing Weight replicate 59
           -9999..09999 .Integer weight of housing unit

WGTP60     5
    Housing Weight replicate 60
           -9999..09999 .Integer weight of housing unit

WGTP61     5
    Housing Weight replicate 61
           -9999..09999 .Integer weight of housing unit

WGTP62     5
    Housing Weight replicate 62
           -9999..09999 .Integer weight of housing unit

WGTP63     5
    Housing Weight replicate 63
           -9999..09999 .Integer weight of housing unit

WGTP64     5
    Housing Weight replicate 64
           -9999..09999 .Integer weight of housing unit

WGTP65     5
    Housing Weight replicate 65
           -9999..09999 .Integer weight of housing unit

WGTP66     5
    Housing Weight replicate 66
           -9999..09999 .Integer weight of housing unit

WGTP67     5
    Housing Weight replicate 67
           -9999..09999 .Integer weight of housing unit

WGTP68     5
    Housing Weight replicate 68
           -9999..09999 .Integer weight of housing unit

WGTP69     5
    Housing Weight replicate 69
           -9999..09999 .Integer weight of housing unit

WGTP70     5
    Housing Weight replicate 70
           -9999..09999 .Integer weight of housing unit

WGTP71     5
    Housing Weight replicate 71
           -9999..09999 .Integer weight of housing unit

WGTP72     5
    Housing Weight replicate 72
           -9999..09999 .Integer weight of housing unit

WGTP73     5
    Housing Weight replicate 73
           -9999..09999 .Integer weight of housing unit

WGTP74     5
    Housing Weight replicate 74
           -9999..09999 .Integer weight of housing unit

WGTP75     5
    Housing Weight replicate 75
           -9999..09999 .Integer weight of housing unit

WGTP76     5
    Housing Weight replicate 76
           -9999..09999 .Integer weight of housing unit

WGTP77     5
    Housing Weight replicate 77
           -9999..09999 .Integer weight of housing unit

WGTP78     5
    Housing Weight replicate 78
           -9999..09999 .Integer weight of housing unit

WGTP79     5
    Housing Weight replicate 79
           -9999..09999 .Integer weight of housing unit

WGTP80     5
    Housing Weight replicate 80
           -9999..09999 .Integer weight of housing unit


PERSON RECORD

RT         1      
    Record Type                         
           P .Person Record

SERIALNO   7      
    Housing unit/GQ person serial number    
           0000001..9999999 .Unique identifier

SPORDER    2      
    Person number
           01..20 .Person number

PUMA       5      
    Public use microdata area code (PUMA) based on 2010 Census definition         
           00100..70301 .Public use microdata area codes
           		 
Note: Public use microdata areas (PUMAs) designate areas of 100,000 or more population.  Use with ST for unique code.

ST         2      
    State Code
           01 .Alabama/AL                              
           02 .Alaska/AK                               
           04 .Arizona/AZ                              
           05 .Arkansas/AR                             
           06 .California/CA                           
           08 .Colorado/CO                             
           09 .Connecticut/CT                          
           10 .Delaware/DE                             
           11 .District of Columbia/DC                 
           12 .Florida/FL                              
           13 .Georgia/GA                              
           15 .Hawaii/HI                               
           16 .Idaho/ID                                
           17 .Illinois/IL                             
           18 .Indiana/IN                              
           19 .Iowa/IA                                 
           20 .Kansas/KS                               
           21 .Kentucky/KY                             
           22 .Louisiana/LA                            
           23 .Maine/ME                                
           24 .Maryland/MD                             
           25 .Massachusetts/MA                        
           26 .Michigan/MI                             
           27 .Minnesota/MN                            
           28 .Mississippi/MS                          
           29 .Missouri/MO                             
           30 .Montana/MT                              
           31 .Nebraska/NE                             
           32 .Nevada/NV                               
           33 .New Hampshire/NH                        
           34 .New Jersey/NJ                           
           35 .New Mexico/NM                           
           36 .New York/NY                             
           37 .North Carolina/NC                       
           38 .North Dakota/ND
           39 .Ohio/OH                                 
           40 .Oklahoma/OK                             
           41 .Oregon/OR                               
           42 .Pennsylvania/PA                         
           44 .Rhode Island/RI                         
           45 .South Carolina/SC                       
           46 .South Dakota/SD                         
           47 .Tennessee/TN                            
           48 .Texas/TX                                
           49 .Utah/UT                                 
           50 .Vermont/VT                              
           51 .Virginia/VA                             
           53 .Washington/WA                           
           54 .West Virginia/WV                        
           55 .Wisconsin/WI                            
           56 .Wyoming/WY                              
           72 .Puerto Rico/PR

ADJINC     7      
Adjustment factor for income and earnings dollar amounts (6 implied decimal places)
           1007549 .2013 factor (1.007549)

Note: The value of ADJINC inflation-adjusts reported income to 2013 dollars.  ADJINC applies to variables FINCP and HINCP in the housing record, and variables INTP, OIP, PAP, PERNP, PINCP, RETP, SEMP, SSIP, SSP, and WAGP in the person record. 

PWGTP      5      
    Person's weight   
           00001..09999 .Integer weight of person

AGEP       2      
    Age
               00 .Under 1 year    
           01..99 .1 to 99 years (Top-coded***)

CIT        1      
    Citizenship status
           1 .Born in the U.S.
           2 .Born in Puerto Rico, Guam, the U.S. Virgin Islands,
             .or the Northern Marianas
           3 .Born abroad of American parent(s)
           4 .U.S. citizen by naturalization
           5 .Not a citizen of the U.S.

CITWP      4      
    Year of naturalization write-in
           bbbb .Not eligible – not naturalized             
           1928 .1928 or earlier (Bottom-coded)
           1929 .1929 – 1933
	   1934 .1934 – 1939
	   1940 .1940 - 1942
           1943 .1943 - 1944
           1945 .1945
           1946 .1946 - 1947
           1948 .1948
           1949 .1949
           1950 .1950
           1951 .1951
           1952 .1952
           1953 .1953
           1954 .1954
           1955 .1955
           1956 .1956
           1957 .1957
           1958 .1958
           1959 .1959
           1960 .1960
           1961 .1961
           1962 .1962
           1963 .1963
           1964 .1964
           1965 .1965
           1966 .1966
           1967 .1967
           1968 .1968
           1969 .1969
           1970 .1970
           1971 .1971
           1972 .1972
           1973 .1973
           1974 .1974
           1975 .1975
           1976 .1976
           1977 .1977
           1978 .1978
           1979 .1979
           1980 .1980
           1981 .1981
           1982 .1982
           1983 .1983
           1984 .1984
           1985 .1985
           1986 .1986
           1987 .1987
           1988 .1988
           1989 .1989
           1990 .1990
           1991 .1991
           1992 .1992
           1993 .1993
           1994 .1994
           1995 .1995
           1996 .1996
           1997 .1997
           1998 .1998
           1999 .1999
           2000 .2000
           2001 .2001
           2002 .2002
           2003 .2003
           2004 .2004
           2005 .2005
           2006 .2006
           2007 .2007
           2008 .2008
           2009 .2009
           2010 .2010
	   2011 .2011
           2012 .2012
           2013 .2013

COW        1      
    Class of worker
           b .N/A (less than 16 years old/NILF who last
             .worked more than 5 years ago or never worked)
           1 .Employee of a private for-profit company or
             .business, or of an individual, for wages,
             .salary, or commissions
           2 .Employee of a private not-for-profit,
             .tax-exempt, or charitable organization
           3 .Local government employee (city, county, etc.)
           4 .State government employee
           5 .Federal government employee
           6 .Self-employed in own not incorporated
             .business, professional practice, or farm
           7 .Self-employed in own incorporated
             .business, professional practice or farm
           8 .Working without pay in family business or farm
           9 .Unemployed and last worked 5 years ago or earlier or never
             .worked
   
DDRS       1      
    Self-care difficulty
           b .N/A (Less than 5 years old)
           1 .Yes
           2 .No

DEAR	   1
    Hearing difficulty
           1. Yes
           2. No

DEYE       1      
    Vision difficulty
           1 .Yes
           2 .No

DOUT       1      
    Independent living difficulty
           b .N/A (Less than 15 years old)
           1 .Yes
           2 .No

DPHY       1      
    Ambulatory difficulty
           b .N/A (Less than 5 years old)
           1 .Yes
           2 .No

DRAT	   1
    Veteran service connected disability rating (percentage)
    	   b .N/A (No service-connected disability/never served in military) 
           1 .0 percent
           2 .10 or 20 percent
           3 .30 or 40 percent
           4 .50 or 60 percent
           5 .70, 80, 90, or 100 percent
           6 .Not reported

DRATX	   1
    Veteran service connected disability rating (checkbox)
    	   b .N/A (Less than 17 years old/never served in military) 
           1 .Yes
           2 .No

DREM       1      
    Cognitive difficulty 
           b .N/A (Less than 5 years old)
           1 .Yes
           2 .No

ENG        1      
    Ability to speak English
           b .N/A (less than 5 years old/speaks only English)
           1 .Very well
           2 .Well
           3 .Not well
           4 .Not at all

FER        1      
    Gave birth to child within the past 12 months
           b .N/A (less than 15 years/greater than 50 years/
             .male)
           1 .Yes      
           2 .No

GCL        1      
    Grandparents living with grandchildren 
           b .N/A (less than 30 years/institutional GQ)
           1 .Yes      
           2 .No           

GCM        1      
    Length of time responsible for grandchildren
           b .N/A (less than 30 years/grandparent not responsible for
             .grandchild/institutional GQ)
           1 .Less than 6 months
           2 .6 to 11 months
           3 .1 to 2 years
           4 .3 to 4 years
           5 .5 or more years

GCR        1      
    Grandparents responsible for grandchildren       
           b .N/A (less than 30 years/institutional GQ/grandparent not living
             .with grandchild)
           1 .Yes      
           2 .No   

HINS1      1
    Insurance through a current or former employer or union
           1 .Yes
           2 .No

HINS2      1      
    Insurance purchased directly from an insurance company
           1 .Yes
           2 .No

HINS3      1      
    Medicare, for people 65 and older, or people with certain disabilities
           1 .Yes
           2 .No

HINS4      1      
    Medicaid, Medical Assistance, or any kind of government-assistance plan 
    for those with low incomes or a disability
           1 .Yes
           2 .No

HINS5      1      
    TRICARE or other military health care
           1 .Yes
           2 .No

HINS6      1      
    VA (including those who have ever used or enrolled for VA health care)
           1 .Yes
           2 .No

HINS7      1      
    Indian Health Service
           1 .Yes
           2 .No 

INTP       6      
    Interest, dividends, and net rental income past 12 months (signed)
                   bbbbbb .N/A (less than 15 years old)
                   000000 .None
           -09999..-00001 .Loss of $1 to $9999 (Rounded and bottom-coded)
                   000001 .$1 or break even
           000002..999999 .$2 to $999999 (Rounded and top-coded)

Note: Use ADJINC to adjust INTP to constant dollars.

JWMNP      3      
    Travel time to work
                bbb .N/A (not a worker or worker who worked at 
                    .home)
           001..200 .1 to 200 minutes to get to work (Top-coded)

JWRIP      2      
    Vehicle occupancy

           bb .N/A (not a worker or worker whose means of
              .transportation to work was not car, truck,
              .or van)
           01 .Drove alone
           02 .In 2-person carpool
           03 .In 3-person carpool
           04 .In 4-person carpool
           05 .In 5-person carpool
           06 .In 6-person carpool
           07 .In 7-person carpool
           08 .In 8-person carpool
           09 .In 9-person carpool
           10 .In 10-person or more carpool (Top-coded)
          
JWTR       2      
    Means of transportation to work
           bb .N/A (not a worker--not in the labor force,
              .including persons under 16 years; unemployed;
              .employed, with a job but not at work; Armed
              .Forces, with a job but not at work)
           01 .Car, truck, or van
           02 .Bus or trolley bus
           03 .Streetcar or trolley car (carro publico in Puerto Rico)
           04 .Subway or elevated
           05 .Railroad
           06 .Ferryboat           
           07 .Taxicab
           08 .Motorcycle
           09 .Bicycle
           10 .Walked
           11 .Worked at home
           12 .Other method

LANX       1      
    Language other than English spoken at home
           b .N/A (less than 5 years old)
           1 .Yes, speaks another language
           2 .No, speaks only English

MAR        1      
    Marital status
           1 .Married
           2 .Widowed
           3 .Divorced
           4 .Separated
           5 .Never married or under 15 years old

MARHD      1
    Divorced in the past 12 months
           b .N/A (age less than 15 years; never married)
           1 .Yes
           2 .No

MARHM      1
    Married in the past 12 months
           b .N/A (age less than 15 years; never married)
           1 .Yes
           2 .No

MARHT      1
    Number of times married
           b .N/A (age less than 15 years; never married)
           1 .One time
           2 .Two times
           3 .Three or more times

MARHW      1
    Widowed in the past 12 months
           b .N/A (age less than 15 years; never married)
           1 .Yes
           2 .No

MARHYP     4
    Year last married
           bbbb. N/A (age less than 15 years; never married)
           1932 .1932 or earlier (Bottom-coded)
           1933 .1933
           1934 .1934
           1935 .1935
           1936 .1936
           1937 .1937
           1938 .1938
           1939 .1939
           1940 .1940
           1941 .1941
           1942 .1942
           1943 .1943
           1944 .1944
           1945 .1945
           1946 .1946
           1947 .1947
           1948 .1948
           1949 .1949
           1950 .1950
           1951 .1951
           1952 .1952
           1953 .1953
           1954 .1954
           1955 .1955
           1956 .1956
           1957 .1957
           1958 .1958
           1959 .1959
           1960 .1960
           1961 .1961
           1962 .1962
           1963 .1963
           1964 .1964
           1965 .1965
           1966 .1966
           1967 .1967
           1968 .1968
           1969 .1969
           1970 .1970
           1971 .1971
           1972 .1972
           1973 .1973
           1974 .1974
           1975 .1975
           1976 .1976
           1977 .1977
           1978 .1978
           1979 .1979
           1980 .1980
           1981 .1981
           1982 .1982
           1983 .1983
           1984 .1984
           1985 .1985
           1986 .1986
           1987 .1987
           1988 .1988
           1989 .1989
           1990 .1990
           1991 .1991
           1992 .1992
           1993 .1993
           1994 .1994
           1995 .1995
           1996 .1996
           1997 .1997
           1998 .1998
           1999 .1999
           2000 .2000
           2001 .2001
           2002 .2002
           2003 .2003
           2004 .2004
           2005 .2005
           2006 .2006
           2007 .2007
           2008 .2008
           2009 .2009
           2010 .2010
	   2011 .2011
           2012 .2012
           2013 .2013

MIG        1      
    Mobility status (lived here 1 year ago)
           b .N/A (less than 1 year old)
           1 .Yes, same house (nonmovers)
           2 .No, outside US and Puerto Rico
           3 .No, different house in US or Puerto Rico

MIL        1      
    Military service
           b .N/A (less than 17 years old)
           1 .Now on active duty
           2 .On active duty in the past, but not now
           3 .Only on active duty for training in Reserves/National Guard 
           4 .Never served in the military

MLPA       1      
    Served September 2001 or later
           b .N/A (less than 17 years old/no active duty)
           0 .Did not serve this period            
           1 .Served this period

MLPB       1      
    Served August 1990 - August 2001 (including Persian Gulf War)
           b .N/A (less than 17 years old/no active duty)
           0 .Did not serve this period            
           1 .Served this period   

MLPCD      1      
    Served May 1975 - July 1990
           b .N/A (less than 17 years old/no active duty)
           0 .Did not serve this period            
           1 .Served this period

MLPE       1      
    Served Vietnam era (August 1964 - April 1975)
           b .N/A (less than 17 years old/no active duty)
           0 .Did not serve this period            
           1 .Served this period

MLPFG      1      
    Served February 1955 - July 1964
           b .N/A (less than 17 years old/no active duty)
           0 .Did not serve this period            
           1 .Served this period

MLPH       1      
    Served Korean War (July 1950 - January 1955)
           b .N/A (less than 17 years old/no active duty)
           0 .Did not serve this period            
           1 .Served this period

MLPI       1      
    Served January 1947 - June 1950
           b .N/A (less than 17 years old/no active duty)
           0 .Did not serve this period            
           1 .Served this period

MLPJ       1      
    Served World War II (December 1941 - December 1946)
           b .N/A (less than 17 years old/no active duty)
           0 .Did not serve this period
           1 .Served this period

MLPK       1      
    Served November 1941 or earlier
           b .N/A (less than 17 years old/no active duty)
           0 .Did not serve this period            
           1 .Served this period

NWAB       1 (UNEDITED - See "Employment Status Recode" (ESR))
    Temporary absence from work 
           b .N/A (less than 16 years old/at work/on layoff)
           1 .Yes
           2 .No
           3 .Did not report

NWAV       1 (UNEDITED - See "Employment Status Recode" (ESR))       
    Available for work
           b .N/A (less than 16 years/at work/not looking)
           1 .Yes
           2 .No, temporarily ill
           3 .No, other reasons
           4 .No, unspecified
           5 .Did not report

NWLA       1 (UNEDITED - See "Employment Status Recode" (ESR))                     
    On layoff from work
           b .N/A (less than 16 years old/at work)       
           1 .Yes                   
           2 .No
           3 .Did not report

NWLK       1 (UNEDITED - See “Employment Status Recode” (ESR))   
    Looking for work
           b .N/A (less than 16 years old/at work/temporarily
             .absent/informed of recall)
           1 .Yes
           2 .No
           3 .Did not report

NWRE       1 (UNEDITED - See “Employment Status Recode” (ESR))  
    Informed of recall        
           b .N/A (less than 16 years old/at work/not on layoff)
           1 .Yes
           2 .No
           3 .Did not report

OIP        6      
    All other income past 12 months
                   bbbbbb .N/A (less than 15 years old)
                   000000 .None
           000001..999999 .$1 to $999999 (Rounded and top-coded)

Note: Use ADJINC to adjust OIP to constant dollars.

PAP        5         
    Public assistance income past 12 months
                  bbbbb .N/A (less than 15 years old)
                  00000 .None
           00001..99999 .$1 to $99999 (Rounded)
 
Note: Use ADJINC to adjust PAP to constant dollars.

RELP       2      
    Relationship
           00 .Reference person
           01 .Husband/wife
           02 .Biological son or daughter
           03 .Adopted son or daughter
           04 .Stepson or stepdaughter   
           05 .Brother or sister
           06 .Father or mother
           07 .Grandchild
           08 .Parent-in-law
           09 .Son-in-law or daughter-in-law
           10 .Other relative
           11 .Roomer or boarder
           12 .Housemate or roommate
           13 .Unmarried partner
           14 .Foster child
           15 .Other nonrelative
           16 .Institutionalized group quarters population
           17 .Noninstitutionalized group quarters population

RETP       6      
    Retirement income past 12 months
                   bbbbbb .N/A (less than 15 years old)
                   000000 .None
           000001..999999 .$1 to $999999 (Rounded and top-coded)

Note: Use ADJINC to adjust RETP to constant dollars.

SCH        1      
    School enrollment
           b .N/A (less than 3 years old)
           1 .No, has not attended in the last 3 months
           2 .Yes, public school or public college    
           3 .Yes, private school or college or home school

SCHG       2
    Grade level attending
           bb .N/A (not attending school)
           01 .Nursery school/preschool
           02 .Kindergarten
           03 .Grade 1
           04 .Grade 2
           05 .Grade 3
           06 .Grade 4
           07 .Grade 5
           08 .Grade 6
           09 .Grade 7
           10 .Grade 8
           11 .Grade 9
           12 .Grade 10
           13 .Grade 11
           14 .Grade 12
           15 .College undergraduate years (freshman to senior)
           16 .Graduate or professional school beyond a bachelor's degree

SCHL       2      
    Educational attainment
           bb .N/A (less than 3 years old)
           01 .No schooling completed
           02 .Nursery school, preschool   
           03 .Kindergarten
           04 .Grade 1
           05 .Grade 2
           06 .Grade 3                   
           07 .Grade 4
           08 .Grade 5
           09 .Grade 6
           10 .Grade 7                   
           11 .Grade 8  
           12 .Grade 9
           13 .Grade 10
           14 .Grade 11                   
           15 .12th grade - no diploma   
           16 .Regular high school diploma
           17 .GED or alternative credential
           18 .Some college, but less than 1 year
           19 .1 or more years of college credit, no degree
           20 .Associate's degree                           
           21 .Bachelor's degree
           22 .Master's degree
           23 .Professional degree beyond a bachelor's degree
           24 .Doctorate degree

SEMP       6      
    Self-employment income past 12 months (signed)
                   bbbbbb .N/A (less than 15 years old)
                   000000 .None                  
           -10000..-00001 .Loss of $1 to $10000 (Rounded and bottom-coded)                 
                   000001 .$1 or break even       
           000002..999999 .$2 to $999999 (Rounded and top-coded)
                          
Note: Use ADJINC to adjust SEMP to constant dollars.

SEX        1      
    Sex
           1 .Male
           2 .Female

SSIP       5      
    Supplementary Security Income past 12 months
                  bbbbb .N/A (less than 15 years old)
                  00000 .None
           00001..99999 .$1 to $99999 (Rounded)

Note: Use ADJINC to adjust SSIP to constant dollars.

SSP        5      

    Social Security income past 12 months
                  bbbbb .N/A (less than 15 years old)
                  00000 .None
           00001..99999 .$1 to $99999 (Rounded)

Note: Use ADJINC to adjust SSP to constant dollars.

WAGP       6      
    Wages or salary income past 12 months
                   bbbbbb .N/A (less than 15 years old)
                   000000 .None
           000001..999999 .$1 to 999999 (Rounded and top-coded)

Note: Use ADJINC to adjust WAGP to constant dollars.

WKHP       2      
    Usual hours worked per week past 12 months
               bb .N/A (less than 16 years old/did not work 
                  .during the past 12 months)
           01..98 .1 to 98 usual hours
               99 .99 or more usual hours

WKL        1      
    When last worked
           b .N/A (less than 16 years old)
           1 .Within the past 12 months
           2 .1-5 years ago
           3 .Over 5 years ago or never worked
          
WKW        1      
    Weeks worked during past 12 months
           b .N/A (less than 16 years old/did not work 
             .during the past 12 months)
           1 .50 to 52 weeks worked during past 12 months
           2 .48 to 49 weeks worked during past 12 months
           3 .40 to 47 weeks worked during past 12 months
           4 .27 to 39 weeks worked during past 12 months
           5 .14 to 26 weeks worked during past 12 months 
           6 .less than 14 weeks worked during past 12 months

WRK        1      
    Worked last week
           b .N/A (not reported)
           1 .Worked
           2 .Did not work

YOEP       4      
    Year of entry
           bbbb .Not eligible - Born in the US             
           1921 .1921 or earlier (Bottom-coded)
           1922 .1922 - 1923
           1924 .1924 - 1925
           1926 .1926 - 1927
           1928 .1928 - 1929
           1930 .1930 – 1931
	   1932 .1932 - 1934
           1935 .1935 - 1936
           1937 .1937 - 1938
           1939 .1939
           1940 .1940
           1941 .1941
           1942 .1942
           1943 .1943 - 1944
           1945 .1945
           1946 .1946
           1947 .1947
           1948 .1948
           1949 .1949
           1950 .1950
           1951 .1951
           1952 .1952
           1953 .1953
           1954 .1954
           1955 .1955
           1956 .1956
           1957 .1957
           1958 .1958
           1959 .1959
           1960 .1960
           1961 .1961
           1962 .1962
           1963 .1963
           1964 .1964
           1965 .1965
           1966 .1966
           1967 .1967
           1968 .1968
           1969 .1969
           1970 .1970
           1971 .1971
           1972 .1972
           1973 .1973
           1974 .1974
           1975 .1975
           1976 .1976
           1977 .1977
           1978 .1978
           1979 .1979
           1980 .1980
           1981 .1981
           1982 .1982
           1983 .1983
           1984 .1984
           1985 .1985
           1986 .1986
           1987 .1987
           1988 .1988
           1989 .1989
           1990 .1990
           1991 .1991
           1992 .1992
           1993 .1993
           1994 .1994
           1995 .1995
           1996 .1996
           1997 .1997
           1998 .1998
           1999 .1999
           2000 .2000
           2001 .2001
           2002 .2002
           2003 .2003
           2004 .2004
           2005 .2005
           2006 .2006
           2007 .2007
           2008 .2008
           2009 .2009
           2010 .2010
	   2011 .2011
           2012 .2012
           2013 .2013
       
ANC        1      
    Ancestry recode
           1 .Single
           2 .Multiple
           3 .Unclassified
           4 .Not reported

ANC1P      3      
    Recoded Detailed Ancestry - first entry     
           001 .Alsatian
           003 .Austrian
           005 .Basque
           008 .Belgian
           009 .Flemish
           011 .British
           012 .British Isles
           020 .Danish
           021 .Dutch
           022 .English
           024 .Finnish
           026 .French
           032 .German
           040 .Prussian
           046 .Greek
           049 .Icelander
           050 .Irish
           051 .Italian
           068 .Sicilian
           077 .Luxemburger
           078 .Maltese
           082 .Norwegian
           084 .Portuguese
           087 .Scotch Irish
           088 .Scottish
           089 .Swedish
           091 .Swiss
           094 .Irish Scotch
           097 .Welsh
           098 .Scandinavian
           099 .Celtic
           100 .Albanian
           102 .Belorussian
           103 .Bulgarian
           109 .Croatian
           111 .Czech
           112 .Bohemian
           114 .Czechoslovakian
           115 .Estonian
           122 .German Russian
           124 .Rom
           125 .Hungarian
           128 .Latvian
           129 .Lithuanian
           130 .Macedonian
	   131 .Montenegrin
           142 .Polish
           144 .Romanian
	   146 .Moldavian
           148 .Russian
           152 .Serbian
           153 .Slovak
           154 .Slovene
	   168 .Turkestani
	   169 .Uzbeg
           170 .Georgia CIS
           171 .Ukrainian
           176 .Yugoslavian
           177 .Herzegovinian
           178 .Slavic
           179 .Slavonian
	   181 .Central European
           183 .Northern European
	   185 .Southern European
           187 .Western European
           190 .Eastern European
           194 .Germanic
           195 .European
           200 .Spaniard
           210 .Mexican
           211 .Mexican American
           212 .Mexicano
           213 .Chicano
           215 .Mexican American Indian
           218 .Mexican State
           219 .Mexican Indian
           221 .Costa Rican
           222 .Guatemalan
           223 .Honduran
           224 .Nicaraguan
           225 .Panamanian
           226 .Salvadoran
           227 .Central American
           231 .Argentinean
           232 .Bolivian
           233 .Chilean
           234 .Colombian
           235 .Ecuadorian
           236 .Paraguayan
           237 .Peruvian
           238 .Uruguayan
           239 .Venezuelan
           249 .South American
           250 .Latin American
           251 .Latin
           252 .Latino
           261 .Puerto Rican
           271 .Cuban
           275 .Dominican
           290 .Hispanic
           291 .Spanish
           295 .Spanish American
           300 .Bahamian
           301 .Barbadian
           302 .Belizean
           308 .Jamaican
           310 .Dutch West Indian
           314 .Trinidadian Tobagonian
           322 .British West Indian
           325 .Antigua and Barbuda
           329 .Grenadian
           330 .Vincent-Grenadine Islander
           331 .St Lucia Islander
           335 .West Indian
           336 .Haitian
           359 .Other West Indian
           360 .Brazilian
           370 .Guyanese
           400 .Algerian
           402 .Egyptian
           406 .Moroccan
	   411 .North African
           416 .Iranian
           417 .Iraqi
           419 .Israeli
           421 .Jordanian
           425 .Lebanese
	   427 .Saudi Arabian
           429 .Syrian
           431 .Armenian
           434 .Turkish
           435 .Yemeni
           442 .Kurdish
           465 .Palestinian
           483 .Assyrian
           484 .Chaldean
           490 .Mideast
           495 .Arab
           496 .Arabic
           499 .Other Arab
           508 .Cameroonian
           510 .Cape Verdean
	   515 .Congolese
           522 .Ethiopian
           523 .Eritrean
           529 .Ghanaian
           534 .Kenyan
           541 .Liberian
           553 .Nigerian
           564 .Senegalese
           566 .Sierra Leonean
           568 .Somalian
           570 .South African
           576 .Sudanese
           587 .Other Subsaharan African
	   588 .Ugandan
           598 .Western African
           599 .African
           600 .Afghan
           603 .Bangladeshi
	   607 .Bhutanese
           609 .Nepali
           615 .Asian Indian
           618 .Bengali
           620 .East Indian
           650 .Punjab
           680 .Pakistani
           690 .Sri Lankan
           700 .Burmese
           703 .Cambodian
           706 .Chinese
           707 .Cantonese
           712 .Mongolian
	   714 .Tibetan
           720 .Filipino
           730 .Indonesian
           740 .Japanese
           748 .Okinawan
           750 .Korean
           765 .Laotian
           768 .Hmong
           770 .Malaysian
           776 .Thai
           782 .Taiwanese
           785 .Vietnamese
           793 .Eurasian
           795 .Asian
           799 .Other Asian
           800 .Australian
           803 .New Zealander
           808 .Polynesian
           811 .Hawaiian
           814 .Samoan
           815 .Tongan
           820 .Micronesian
           821 .Guamanian
           822 .Chamorro	     
           825 .Marshallese
           841 .Fijian
           850 .Pacific Islander
           899 .Other Pacific
           900 .Afro American
           901 .Afro
           902 .African American
           903 .Black
           904 .Negro
           907 .Creole
           913 .Central American Indian
           914 .South American Indian
           917 .Native American
           918 .Indian
           919 .Cherokee
           920 .American Indian
           921 .Aleut
           922 .Eskimo
           924 .White
           925 .Anglo
           927 .Appalachian
           929 .Pennsylvania German
           931 .Canadian
           935 .French Canadian
           937 .Cajun
           939 .American	     
           940 .United States
           983 .Texas
           994 .North American
           995 .Mixture
           996 .Uncodable entries
           997 .Other groups
           998 .Other responses
           999 .Not reported

ANC2P      3      
    Recoded Detailed Ancestry - second entry          
           001 .Alsatian
           003 .Austrian
           005 .Basque
           008 .Belgian
           009 .Flemish
           011 .British
           012 .British Isles
           020 .Danish
           021 .Dutch
           022 .English
           024 .Finnish
           026 .French
           032 .German
           040 .Prussian
           046 .Greek
           049 .Icelander
           050 .Irish
           051 .Italian
           068 .Sicilian
           077 .Luxemburger
           078 .Maltese
           082 .Norwegian
           084 .Portuguese
           087 .Scotch Irish
           088 .Scottish
           089 .Swedish
           091 .Swiss
           094 .Irish Scotch
           097 .Welsh
           098 .Scandinavian
           099 .Celtic
           100 .Albanian
           102 .Belorussian
           103 .Bulgarian
           109 .Croatian
           111 .Czech
           112 .Bohemian
           114 .Czechoslovakian
           115 .Estonian
           122 .German Russian
           124 .Rom
           125 .Hungarian
           128 .Latvian
           129 .Lithuanian
           130 .Macedonian
	   131 .Montenegrin
           142 .Polish
           144 .Romanian
	   146 .Moldavian
           148 .Russian
           152 .Serbian
           153 .Slovak
           154 .Slovene
	   168 .Turkestani
	   169 .Uzbeg
           170 .Georgia CIS
           171 .Ukrainian
           176 .Yugoslavian
           177 .Herzegovinian
           178 .Slavic
           179 .Slavonian
	   181 .Central European
           183 .Northern European
	   185 .Southern European
           187 .Western European
           190 .Eastern European
           194 .Germanic
           195 .European
           200 .Spaniard
           210 .Mexican
           211 .Mexican American
           212 .Mexicano
           213 .Chicano
           215 .Mexican American Indian
           218 .Mexican State
           219 .Mexican Indian
           221 .Costa Rican
           222 .Guatemalan
           223 .Honduran
           224 .Nicaraguan
           225 .Panamanian
           226 .Salvadoran
           227 .Central American
           231 .Argentinean
           232 .Bolivian
           233 .Chilean
           234 .Colombian
           235 .Ecuadorian
           236 .Paraguayan
           237 .Peruvian
           238 .Uruguayan
           239 .Venezuelan
           249 .South American
           250 .Latin American
           251 .Latin
           252 .Latino
           261 .Puerto Rican
           271 .Cuban
           275 .Dominican
           290 .Hispanic
           291 .Spanish
           295 .Spanish American
           300 .Bahamian
           301 .Barbadian
           302 .Belizean
           308 .Jamaican
           310 .Dutch West Indian
           314 .Trinidadian Tobagonian
           322 .British West Indian
           325 .Antigua and Barbuda
           329 .Grenadian
           330 .Vincent-Grenadine Islander
           331 .St Lucia Islander
           335 .West Indian
           336 .Haitian
           359 .Other West Indian
           360 .Brazilian
           370 .Guyanese
           400 .Algerian
           402 .Egyptian
           406 .Moroccan
	   411 .North African
           416 .Iranian
           417 .Iraqi
           419 .Israeli
           421 .Jordanian
           425 .Lebanese
	   427 .Saudi Arabian
           429 .Syrian
           431 .Armenian
           434 .Turkish
           435 .Yemeni
           442 .Kurdish
           465 .Palestinian
           483 .Assyrian
           484 .Chaldean
           490 .Mideast
           495 .Arab
           496 .Arabic
           499 .Other Arab
           508 .Cameroonian
           510 .Cape Verdean
	   515 .Congolese
           522 .Ethiopian
           523 .Eritrean
           529 .Ghanaian
           534 .Kenyan
           541 .Liberian
           553 .Nigerian
           564 .Senegalese
           566 .Sierra Leonean
           568 .Somalian
           570 .South African
           576 .Sudanese
           587 .Other Subsaharan African
	   588 .Ugandan
           598 .Western African
           599 .African
           600 .Afghan
           603 .Bangladeshi
	   607 .Bhutanese
           609 .Nepali
           615 .Asian Indian
           618 .Bengali
           620 .East Indian
           650 .Punjab
           680 .Pakistani
           690 .Sri Lankan
           700 .Burmese
           703 .Cambodian
           706 .Chinese
           707 .Cantonese
           712 .Mongolian
	   714 .Tibetan
           720 .Filipino
           730 .Indonesian
           740 .Japanese
           748 .Okinawan
           750 .Korean
           765 .Laotian
           768 .Hmong
           770 .Malaysian
           776 .Thai
           782 .Taiwanese
           785 .Vietnamese
           793 .Eurasian
           795 .Asian
           799 .Other Asian
           800 .Australian
           803 .New Zealander
           808 .Polynesian
           811 .Hawaiian
           814 .Samoan
           815 .Tongan
           820 .Micronesian
           821 .Guamanian
           822 .Chamorro	     
           825 .Marshallese
           841 .Fijian
           850 .Pacific Islander
           899 .Other Pacific
           900 .Afro American
           901 .Afro
           902 .African American
           903 .Black
           904 .Negro
           907 .Creole
           913 .Central American Indian
           914 .South American Indian
           917 .Native American
           918 .Indian
           919 .Cherokee
           920 .American Indian
           921 .Aleut
           922 .Eskimo
           924 .White
           925 .Anglo
           927 .Appalachian
           929 .Pennsylvania German
           931 .Canadian
           935 .French Canadian
           937 .Cajun
           939 .American 
	   940 .United States
           983 .Texas
           994 .North American
           995 .Mixture
           996 .Uncodable entries
           997 .Other groups
           998 .Other responses
           999 .Not reported

DECADE     1      
    Decade of entry
           b .N/A (Born in the US)
           1 .Before 1950
           2 .1950 - 1959
           3 .1960 - 1969
           4 .1970 - 1979
           5 .1980 - 1989
           6 .1990 - 1999
           7 .2000 or later 

DIS        1      
    Disability recode
           1 .With a disability
           2 .Without a disability

DRIVESP    1      
    Number of vehicles calculated from JWRI
           b .N/A (Nonworker or worker who does not drive to work)
           1 .1.000 vehicles (Drove alone)
           2 .0.500 vehicles (In a 2-person carpool)
           3 .0.333 vehicles (In a 3-person carpool)
           4 .0.250 vehicles (In a 4-person carpool)
           5 .0.200 vehicles (In a 5- or 6-person carpool)
           6 .0.143 vehicles (In a 7-or-more person carpool)

ESP        1      
    Employment status of parents
           b .N/A (not own child of householder, and not
             .child in subfamily)
             .Living with two parents:
           1 .Both parents in labor force 
           2 .Father only in labor force
           3 .Mother only in labor force
           4 .Neither parent in labor force
             .Living with one parent:
             .Living with father:
           5 .Father in the labor force       
           6 .Father not in labor force
             .Living with mother:
           7 .Mother in the labor force       
           8 .Mother not in labor force

ESR        1      
    Employment status recode
           b .N/A (less than 16 years old)
           1 .Civilian employed, at work
           2 .Civilian employed, with a job but not at work
           3 .Unemployed
           4 .Armed forces, at work
           5 .Armed forces, with a job but not at work
           6 .Not in labor force

FOD1P	   4
    Recoded field of degree - first entry
           bbbb .N/A (less than bachelor's degree)
           1100 .GENERAL AGRICULTURE
           1101 .AGRICULTURE PRODUCTION AND MANAGEMENT
           1102 .AGRICULTURAL ECONOMICS
           1103 .ANIMAL SCIENCES
           1104 .FOOD SCIENCE
           1105 .PLANT SCIENCE AND AGRONOMY
           1106 .SOIL SCIENCE
           1199 .MISCELLANEOUS AGRICULTURE
           1301 .ENVIRONMENTAL SCIENCE
           1302 .FORESTRY
           1303 .NATURAL RESOURCES MANAGEMENT
           1401 .ARCHITECTURE
           1501 .AREA ETHNIC AND CIVILIZATION STUDIES
           1901 .COMMUNICATIONS
           1902 .JOURNALISM
           1903 .MASS MEDIA
           1904 .ADVERTISING AND PUBLIC RELATIONS
           2001 .COMMUNICATION TECHNOLOGIES
           2100 .COMPUTER AND INFORMATION SYSTEMS
           2101 .COMPUTER PROGRAMMING AND DATA PROCESSING
           2102 .COMPUTER SCIENCE
           2105 .INFORMATION SCIENCES
           2106 .COMPUTER ADMINISTRATION MANAGEMENT AND SECURITY
           2107 .COMPUTER NETWORKING AND TELECOMMUNICATIONS
           2201 .COSMETOLOGY SERVICES AND CULINARY ARTS
           2300 .GENERAL EDUCATION
           2301 .EDUCATIONAL ADMINISTRATION AND SUPERVISION
           2303 .SCHOOL STUDENT COUNSELING
           2304 .ELEMENTARY EDUCATION
           2305 .MATHEMATICS TEACHER EDUCATION
           2306 .PHYSICAL AND HEALTH EDUCATION TEACHING
           2307 .EARLY CHILDHOOD EDUCATION
           2308 .SCIENCE AND COMPUTER TEACHER EDUCATION
           2309 .SECONDARY TEACHER EDUCATION
           2310 .SPECIAL NEEDS EDUCATION
           2311 .SOCIAL SCIENCE OR HISTORY TEACHER EDUCATION
           2312 .TEACHER EDUCATION: MULTIPLE LEVELS
           2313 .LANGUAGE AND DRAMA EDUCATION
           2314 .ART AND MUSIC EDUCATION
           2399 .MISCELLANEOUS EDUCATION
           2400 .GENERAL ENGINEERING
           2401 .AEROSPACE ENGINEERING
           2402 .BIOLOGICAL ENGINEERING
           2403 .ARCHITECTURAL ENGINEERING
           2404 .BIOMEDICAL ENGINEERING
           2405 .CHEMICAL ENGINEERING
           2406 .CIVIL ENGINEERING
           2407 .COMPUTER ENGINEERING
           2408 .ELECTRICAL ENGINEERING
           2409 .ENGINEERING MECHANICS PHYSICS AND SCIENCE
           2410 .ENVIRONMENTAL ENGINEERING
           2411 .GEOLOGICAL AND GEOPHYSICAL ENGINEERING
           2412 .INDUSTRIAL AND MANUFACTURING ENGINEERING
           2413 .MATERIALS ENGINEERING AND MATERIALS SCIENCE
           2414 .MECHANICAL ENGINEERING
           2415 .METALLURGICAL ENGINEERING
           2416 .MINING AND MINERAL ENGINEERING
           2417 .NAVAL ARCHITECTURE AND MARINE ENGINEERING
           2418 .NUCLEAR ENGINEERING
           2419 .PETROLEUM ENGINEERING
           2499 .MISCELLANEOUS ENGINEERING
           2500 .ENGINEERING TECHNOLOGIES
           2501 .ENGINEERING AND INDUSTRIAL MANAGEMENT
           2502 .ELECTRICAL ENGINEERING TECHNOLOGY
           2503 .INDUSTRIAL PRODUCTION TECHNOLOGIES
           2504 .MECHANICAL ENGINEERING RELATED TECHNOLOGIES
           2599 .MISCELLANEOUS ENGINEERING TECHNOLOGIES
           2601 .LINGUISTICS AND COMPARATIVE LANGUAGE AND LITERATURE
           2602 .FRENCH GERMAN LATIN AND OTHER COMMON FOREIGN LANGUAGE 
                .STUDIES
           2603 .OTHER FOREIGN LANGUAGES
           2901 .FAMILY AND CONSUMER SCIENCES
           3201 .COURT REPORTING
           3202 .PRE-LAW AND LEGAL STUDIES
           3301 .ENGLISH LANGUAGE AND LITERATURE
           3302 .COMPOSITION AND RHETORIC
           3401 .LIBERAL ARTS
           3402 .HUMANITIES
           3501 .LIBRARY SCIENCE
           3600 .BIOLOGY
           3601 .BIOCHEMICAL SCIENCES
           3602 .BOTANY
           3603 .MOLECULAR BIOLOGY
           3604 .ECOLOGY
           3605 .GENETICS
           3606 .MICROBIOLOGY
           3607 .PHARMACOLOGY
           3608 .PHYSIOLOGY
           3609 .ZOOLOGY
           3611 .NEUROSCIENCE
           3699 .MISCELLANEOUS BIOLOGY
           3700 .MATHEMATICS
           3701 .APPLIED MATHEMATICS
           3702 .STATISTICS AND DECISION SCIENCE
           3801 .MILITARY TECHNOLOGIES
           4000 .MULTI/INTERDISCIPLINARY STUDIES
           4001 .INTERCULTURAL AND INTERNATIONAL STUDIES
           4002 .NUTRITION SCIENCES
           4005 .MATHEMATICS AND COMPUTER SCIENCE
           4006 .COGNITIVE SCIENCE AND BIOPSYCHOLOGY
           4007 .INTERDISCIPLINARY SOCIAL SCIENCES
           4101 .PHYSICAL FITNESS PARKS RECREATION AND LEISURE
           4801 .PHILOSOPHY AND RELIGIOUS STUDIES
           4901 .THEOLOGY AND RELIGIOUS VOCATIONS
           5000 .PHYSICAL SCIENCES
           5001 .ASTRONOMY AND ASTROPHYSICS
           5002 .ATMOSPHERIC SCIENCES AND METEOROLOGY
           5003 .CHEMISTRY
           5004 .GEOLOGY AND EARTH SCIENCE
           5005 .GEOSCIENCES
           5006 .OCEANOGRAPHY
           5007 .PHYSICS
           5008 .MATERIALS SCIENCE
           5098 .MULTI-DISCIPLINARY OR GENERAL SCIENCE
           5102 .NUCLEAR, INDUSTRIAL RADIOLOGY, AND BIOLOGICAL TECHNOLOGIES
           5200 .PSYCHOLOGY
           5201 .EDUCATIONAL PSYCHOLOGY
           5202 .CLINICAL PSYCHOLOGY
           5203 .COUNSELING PSYCHOLOGY
           5205 .INDUSTRIAL AND ORGANIZATIONAL PSYCHOLOGY
           5206 .SOCIAL PSYCHOLOGY
           5299 .MISCELLANEOUS PSYCHOLOGY
           5301 .CRIMINAL JUSTICE AND FIRE PROTECTION
           5401 .PUBLIC ADMINISTRATION
           5402 .PUBLIC POLICY
           5403 .HUMAN SERVICES AND COMMUNITY ORGANIZATION
           5404 .SOCIAL WORK
           5500 .GENERAL SOCIAL SCIENCES
           5501 .ECONOMICS
           5502 .ANTHROPOLOGY AND ARCHEOLOGY
           5503 .CRIMINOLOGY
           5504 .GEOGRAPHY
           5505 .INTERNATIONAL RELATIONS
           5506 .POLITICAL SCIENCE AND GOVERNMENT
           5507 .SOCIOLOGY
           5599 .MISCELLANEOUS SOCIAL SCIENCES
           5601 .CONSTRUCTION SERVICES
           5701 .ELECTRICAL, MECHANICAL, AND PRECISION TECHNOLOGIES AND
                .PRODUCTION
           5901 .TRANSPORTATION SCIENCES AND TECHNOLOGIES
           6000 .FINE ARTS
           6001 .DRAMA AND THEATER ARTS
           6002 .MUSIC
           6003 .VISUAL AND PERFORMING ARTS
           6004 .COMMERCIAL ART AND GRAPHIC DESIGN
           6005 .FILM VIDEO AND PHOTOGRAPHIC ARTS
           6006 .ART HISTORY AND CRITICISM
           6007 .STUDIO ARTS
           6099 .MISCELLANEOUS FINE ARTS
           6100 .GENERAL MEDICAL AND HEALTH SERVICES
           6102 .COMMUNICATION DISORDERS SCIENCES AND SERVICES
           6103 .HEALTH AND MEDICAL ADMINISTRATIVE SERVICES
           6104 .MEDICAL ASSISTING SERVICES
           6105 .MEDICAL TECHNOLOGIES TECHNICIANS
           6106 .HEALTH AND MEDICAL PREPARATORY PROGRAMS
           6107 .NURSING
           6108 .PHARMACY PHARMACEUTICAL SCIENCES AND ADMINISTRATION
           6109 .TREATMENT THERAPY PROFESSIONS
           6110 .COMMUNITY AND PUBLIC HEALTH
           6199 .MISCELLANEOUS HEALTH MEDICAL PROFESSIONS
           6200 .GENERAL BUSINESS
           6201 .ACCOUNTING
           6202 .ACTUARIAL SCIENCE
           6203 .BUSINESS MANAGEMENT AND ADMINISTRATION
           6204 .OPERATIONS LOGISTICS AND E-COMMERCE
           6205 .BUSINESS ECONOMICS
           6206 .MARKETING AND MARKETING RESEARCH
           6207 .FINANCE
           6209 .HUMAN RESOURCES AND PERSONNEL MANAGEMENT
           6210 .INTERNATIONAL BUSINESS
           6211 .HOSPITALITY MANAGEMENT
           6212 .MANAGEMENT INFORMATION SYSTEMS AND STATISTICS
           6299 .MISCELLANEOUS BUSINESS & MEDICAL ADMINISTRATION
           6402 .HISTORY
           6403 .UNITED STATES HISTORY

FOD2P	   4
    Recoded field of degree - second entry
           bbbb .N/A (less than bachelor's degree)
           1100 .GENERAL AGRICULTURE
           1101 .AGRICULTURE PRODUCTION AND MANAGEMENT
           1102 .AGRICULTURAL ECONOMICS
           1103 .ANIMAL SCIENCES
           1104 .FOOD SCIENCE
           1105 .PLANT SCIENCE AND AGRONOMY
           1106 .SOIL SCIENCE
           1199 .MISCELLANEOUS AGRICULTURE
           1301 .ENVIRONMENTAL SCIENCE
           1302 .FORESTRY
           1303 .NATURAL RESOURCES MANAGEMENT
           1401 .ARCHITECTURE
           1501 .AREA ETHNIC AND CIVILIZATION STUDIES
           1901 .COMMUNICATIONS
           1902 .JOURNALISM
           1903 .MASS MEDIA
           1904 .ADVERTISING AND PUBLIC RELATIONS
           2001 .COMMUNICATION TECHNOLOGIES
           2100 .COMPUTER AND INFORMATION SYSTEMS
           2101 .COMPUTER PROGRAMMING AND DATA PROCESSING
           2102 .COMPUTER SCIENCE
           2105 .INFORMATION SCIENCES
           2106 .COMPUTER ADMINISTRATION MANAGEMENT AND SECURITY
           2107 .COMPUTER NETWORKING AND TELECOMMUNICATIONS
           2201 .COSMETOLOGY SERVICES AND CULINARY ARTS
           2300 .GENERAL EDUCATION
           2301 .EDUCATIONAL ADMINISTRATION AND SUPERVISION
           2303 .SCHOOL STUDENT COUNSELING
           2304 .ELEMENTARY EDUCATION
           2305 .MATHEMATICS TEACHER EDUCATION
           2306 .PHYSICAL AND HEALTH EDUCATION TEACHING
           2307 .EARLY CHILDHOOD EDUCATION
           2308 .SCIENCE AND COMPUTER TEACHER EDUCATION
           2309 .SECONDARY TEACHER EDUCATION
           2310 .SPECIAL NEEDS EDUCATION
           2311 .SOCIAL SCIENCE OR HISTORY TEACHER EDUCATION
           2312 .TEACHER EDUCATION: MULTIPLE LEVELS
           2313 .LANGUAGE AND DRAMA EDUCATION
           2314 .ART AND MUSIC EDUCATION
           2399 .MISCELLANEOUS EDUCATION
           2400 .GENERAL ENGINEERING
           2401 .AEROSPACE ENGINEERING
           2402 .BIOLOGICAL ENGINEERING
           2403 .ARCHITECTURAL ENGINEERING
           2404 .BIOMEDICAL ENGINEERING
           2405 .CHEMICAL ENGINEERING
           2406 .CIVIL ENGINEERING
           2407 .COMPUTER ENGINEERING
           2408 .ELECTRICAL ENGINEERING
           2409 .ENGINEERING MECHANICS PHYSICS AND SCIENCE
           2410 .ENVIRONMENTAL ENGINEERING
           2411 .GEOLOGICAL AND GEOPHYSICAL ENGINEERING
           2412 .INDUSTRIAL AND MANUFACTURING ENGINEERING
           2413 .MATERIALS ENGINEERING AND MATERIALS SCIENCE
           2414 .MECHANICAL ENGINEERING
           2415 .METALLURGICAL ENGINEERING
           2416 .MINING AND MINERAL ENGINEERING
           2417 .NAVAL ARCHITECTURE AND MARINE ENGINEERING
           2418 .NUCLEAR ENGINEERING
           2419 .PETROLEUM ENGINEERING
           2499 .MISCELLANEOUS ENGINEERING
           2500 .ENGINEERING TECHNOLOGIES
           2501 .ENGINEERING AND INDUSTRIAL MANAGEMENT
           2502 .ELECTRICAL ENGINEERING TECHNOLOGY
           2503 .INDUSTRIAL PRODUCTION TECHNOLOGIES
           2504 .MECHANICAL ENGINEERING RELATED TECHNOLOGIES
           2599 .MISCELLANEOUS ENGINEERING TECHNOLOGIES
           2601 .LINGUISTICS AND COMPARATIVE LANGUAGE AND LITERATURE
           2602 .FRENCH GERMAN LATIN AND OTHER COMMON FOREIGN LANGUAGE 
                .STUDIES
           2603 .OTHER FOREIGN LANGUAGES
           2901 .FAMILY AND CONSUMER SCIENCES
           3201 .COURT REPORTING
           3202 .PRE-LAW AND LEGAL STUDIES
           3301 .ENGLISH LANGUAGE AND LITERATURE
           3302 .COMPOSITION AND RHETORIC
           3401 .LIBERAL ARTS
           3402 .HUMANITIES
           3501 .LIBRARY SCIENCE
           3600 .BIOLOGY
           3601 .BIOCHEMICAL SCIENCES
           3602 .BOTANY
           3603 .MOLECULAR BIOLOGY
           3604 .ECOLOGY
           3605 .GENETICS
           3606 .MICROBIOLOGY
           3607 .PHARMACOLOGY
           3608 .PHYSIOLOGY
           3609 .ZOOLOGY
           3611 .NEUROSCIENCE
           3699 .MISCELLANEOUS BIOLOGY
           3700 .MATHEMATICS
           3701 .APPLIED MATHEMATICS
           3702 .STATISTICS AND DECISION SCIENCE
           3801 .MILITARY TECHNOLOGIES
           4000 .MULTI/INTERDISCIPLINARY STUDIES
           4001 .INTERCULTURAL AND INTERNATIONAL STUDIES
           4002 .NUTRITION SCIENCES
           4005 .MATHEMATICS AND COMPUTER SCIENCE
           4006 .COGNITIVE SCIENCE AND BIOPSYCHOLOGY
           4007 .INTERDISCIPLINARY SOCIAL SCIENCES
           4101 .PHYSICAL FITNESS PARKS RECREATION AND LEISURE
           4801 .PHILOSOPHY AND RELIGIOUS STUDIES
           4901 .THEOLOGY AND RELIGIOUS VOCATIONS
           5000 .PHYSICAL SCIENCES
           5001 .ASTRONOMY AND ASTROPHYSICS
           5002 .ATMOSPHERIC SCIENCES AND METEOROLOGY
           5003 .CHEMISTRY
           5004 .GEOLOGY AND EARTH SCIENCE
           5005 .GEOSCIENCES
           5006 .OCEANOGRAPHY
           5007 .PHYSICS
           5008 .MATERIALS SCIENCE
           5098 .MULTI-DISCIPLINARY OR GENERAL SCIENCE
           5102 .NUCLEAR, INDUSTRIAL RADIOLOGY, AND BIOLOGICAL TECHNOLOGIES
           5200 .PSYCHOLOGY
           5201 .EDUCATIONAL PSYCHOLOGY
           5202 .CLINICAL PSYCHOLOGY
           5203 .COUNSELING PSYCHOLOGY
           5205 .INDUSTRIAL AND ORGANIZATIONAL PSYCHOLOGY
           5206 .SOCIAL PSYCHOLOGY
           5299 .MISCELLANEOUS PSYCHOLOGY
           5301 .CRIMINAL JUSTICE AND FIRE PROTECTION
           5401 .PUBLIC ADMINISTRATION
           5402 .PUBLIC POLICY
           5403 .HUMAN SERVICES AND COMMUNITY ORGANIZATION
           5404 .SOCIAL WORK
           5500 .GENERAL SOCIAL SCIENCES
           5501 .ECONOMICS
           5502 .ANTHROPOLOGY AND ARCHEOLOGY
           5503 .CRIMINOLOGY
           5504 .GEOGRAPHY
           5505 .INTERNATIONAL RELATIONS
           5506 .POLITICAL SCIENCE AND GOVERNMENT
           5507 .SOCIOLOGY
           5599 .MISCELLANEOUS SOCIAL SCIENCES
           5601 .CONSTRUCTION SERVICES
           5701 .ELECTRICAL, MECHANICAL, AND PRECISION TECHNOLOGIES AND
                .PRODUCTION
           5901 .TRANSPORTATION SCIENCES AND TECHNOLOGIES
           6000 .FINE ARTS
           6001 .DRAMA AND THEATER ARTS
           6002 .MUSIC
           6003 .VISUAL AND PERFORMING ARTS
           6004 .COMMERCIAL ART AND GRAPHIC DESIGN
           6005 .FILM VIDEO AND PHOTOGRAPHIC ARTS
           6006 .ART HISTORY AND CRITICISM
           6007 .STUDIO ARTS
           6099 .MISCELLANEOUS FINE ARTS
           6100 .GENERAL MEDICAL AND HEALTH SERVICES
           6102 .COMMUNICATION DISORDERS SCIENCES AND SERVICES
           6103 .HEALTH AND MEDICAL ADMINISTRATIVE SERVICES
           6104 .MEDICAL ASSISTING SERVICES
           6105 .MEDICAL TECHNOLOGIES TECHNICIANS
           6106 .HEALTH AND MEDICAL PREPARATORY

