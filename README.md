0WI_DATA readme

Demographic data for 2010 and general elections for all years came with the ward geometries shapefile from The Wisconsin Legislature arcgis portal.
Metadata and notes on their process can be found here, including election data disaggregation: https://data-ltsb.opendata.arcgis.com/datasets/LTSB::2012-2020-election-data-with-2020-wards/about
and here for more detail on demographic data: https://www.arcgis.com/sharing/rest/content/items/f67c2e7f43bb432687b4a42bee50a16c/info/metadata/metadata.xml?format=default&output=html
Demographic data comes from 2011 and 2010 census blocks.

2020 demographic data came from a seperate wards shapefile from the Wisconsin State Legislature arcgis portal. 
Documentation on the data provided in this shapefile, which follows the conventions for redistricting population data definitions set by the state Department of Justice, can found here:
https://legis.wisconsin.gov/ltsb/gisdocs/Data2020/2020_PL_94-171_Data_Calculations.pdf
The Department of Justice redistricting guidelines: https://legis.wisconsin.gov/ltsb/gisdocs/Data2020/DOJ_Redistricting_Guidelines.pdf were published in 2001, so although the 2010 census demographic data does not have its own variable definitions, we presume here the same DOJ designated definitions seen in the 2020 data.

Despite both being ward shapefiles from the same source, the election data file and the 2020 population data file were not a perfect one-to-one match for joining wards.

The following adjustments were made to the election wards file:
- `merge` Chippewa Falls - C 0007 & Chippewa Falls - C 0007S
- `merge` Milwaukee County Bayside - V 0001 & Bayside - V 001S
-	`merge` Milwaukee County Bayside - V 0003 & Bayside - V 003S
-	`merge` Milwaukee County Glendale - C 0008 & Bayside - C 008S
-	`merge` Milwaukee County Glendale - C 0011 & Bayside - C 011S
-	`merge` Oshkosh - C 022A & Oshkosh - C 022B
-	`merge` Milwaukee County Franklin - C 015A & Franklin - C 015B
-	`merge` Monroe County La Grange - T 002A & La Grange - T 002B
-	`merge` Menasha C 005A & Menasha C 005A
-	`merge` Oshkosh - C 029A & Oshkosh - C 029B
-	`merge` Oshkosh - C 025A & Oshkosh - C 025B
-	`merge` Oshkosh - C 028A & Oshkosh - C 028B
-	`merge` Oshkosh - C 023A & Oshkosh - C 023B
-	`merge` Oshkosh - T 001A & Oshkosh - T 001B
-	`merge` Monroe County La Grange - T 001A & La Grange - T 001B
-	`merge` Milwaukee County Franklin - C 022A & Franklin - C 022B
-	`merge` Mequon - C 007A & Mequon - C 007B

Democratic primary election data for the year 2018 was added to the shapefile from the following tabular source: https://elections.wi.gov/elections-voting/results/2014/partisan-primary
These elections were disaggregated to the ward level to be joined on to the state-provided shapefile.

Column definitions:

-	`COUNTYFP` County FIPS code
-	`COUNTY` County name (str)
-	`NAME` Ward group name (str) 
-	`POP10` Total population 2010
-	`VAP10` Voting age population 2010
-	`WHITE10` Non-Hispanic White population 2010
-	`BLACK10` Non-Hispanic Black + Non-Hispanic Black and White population 2010
-	`HISPANIC10` Hispanic Alone population 2010
-	`ASIAN10` Non-Hispanic Asian + Non-Hispanic Asian and White population 2010
-	`AMIN10` Non-Hispanic American Indian and Alaska Native + Non-Hispanic American Indian and Alaska Native and White population 2010
-	`NHPI10` Non-Hispanic Native Hawaiian and Other Pacific Islander + Non-Hispanic Native Hawaiian and Other Pacific Islander and White population 2010
-	`OTHER10` Population of Non-Hispanic Other Races 2010
-	`MLT10` Population of Non-Hispanic Other Races Multiracial 2010
-	`WVAP10` Non-Hispanic White population over 18 2010
-	`BVAP10` Black population over 18 2010
-	`HVAP10` Hispanic Alone population over 18 2010
-	'ASIANVAP10' Non-Hispanic Asian + Non-Hispanic Asian and White population population over 18 2010
-	`AMINVAP10` Non-Hispanic American Indian and Alaska Native + Non-Hispanic American Indian and Alaska Native and White population population over 18 2010
	`NHPIVAP10` on-Hispanic Native Hawaiian and Other Pacific Islander + Non-Hispanic Native Hawaiian and Other Pacific Islander and White population over 18 2010
-	`OTHERVAP10` Population of Non-Hispanic Other Races over 18 2010
-	`MLTVAP10` Population of Non-Hispanic Other Races Multiracial over 18 2010
-	`POP20` Total population 2020
-	`VAP20` Voting age population 2020
-	`WHITE20` Non-Hispanic White population 2020
-	`BLACK20` Non-Hispanic Black + Non-Hispanic Black and White population 2020
-	`HISPANIC20` Hispanic Alone population 2020
- `ASIAN20` Non-Hispanic Asian + Non-Hispanic Asian and White population 2020
-	`AMIN20` Non-Hispanic American Indian and Alaska Native + Non-Hispanic American Indian and Alaska Native and White population 2020
-	`NHPI20` Non-Hispanic Native Hawaiian and Other Pacific Islander + Non-Hispanic Native Hawaiian and Other Pacific Islander and White population 2020
-	`OTHER20` Population of Non-Hispanic Other Races 2020
-	`MLT20` Population of Non-Hispanic Other Races Multiracial 2020
-	`WVAP20` Non-Hispanic White population over 18 2020
-	`BVAP20` Black population over 18 2020
-	`HVAP20` Hispanic Alone population over 18 2020
-	'ASIANVAP20' Non-Hispanic Asian + Non-Hispanic Asian and White population population over 18 2020
-	`AMINVAP20` Non-Hispanic American Indian and Alaska Native + Non-Hispanic American Indian and Alaska Native and White population population over 18 2020
-	`NHPIVAP20` on-Hispanic Native Hawaiian and Other Pacific Islander + Non-Hispanic Native Hawaiian and Other Pacific Islander and White population over 18 2020
-	`OTHERVAP20` Population of Non-Hispanic Other Races over 18 2020
-	`MLTVAP20` Population of Non-Hispanic Other Races Multiracial over 18 2020
-	`GOVTOT18` Total votes for Governors race 2018
-	`GOVR18` Votes for Republican Gubernatorial candidate 2018 (Scott Walker)
-	`GOVD18` Votes for Democratic Gubernatorial candidate 2018 (Tony Evers)
-	`SOSTOT18` Total votes for Secretary of State race 2018
-	`SOSR18` Votes for Republican Seceratary of State candidate 2018 (Jay Shcroeder)
-	`SOSD18` Votes for Democratic Secretary of State candidate 2018 (Doug La Follette)
-	`TRESTOT18` Total votes for Treasurer race 2018
-	`TRESR18` Votes for Republican Treasurer candidate 2018 (Travis Hartwig)
-	`TRESD18 - Votes for Democratic Treasurer candidate 2018 (Sarah Godlewski)
-	`LG18P_KOBE` Votes for Democratic Lieutenant Governor primary candidate Kurt Kober 2018
-	`LG18P_BARN` Votes for Democratic Lieutenant Governor primary candidate Mandela Barnes 2018
-	`GOV18P_FLY` Votes for Democratic Governor primary candidate Matthew Flynn 2018
-	`GOV18P_EVE` Votes for Democratic Governor primary candidate Tony Evers 2018
-	`GOV18P_MCC` Votes for Democratic Governor primary candidate Michael McCabe 2018
-	`GOV18P_MIT` Votes for Democratic Governor primary candidate Mahlon Mitchell 2018
-	`GOV18P_ROY` Votes for Democratic Governor primary candidate Kelda Roys 2018
-	`GOV18P_SOG` Votes for Democratic Governor primary candidate Paul Sogin 2018
-	`GOV18P_VIN` Votes for Democratic Governor primary candidate Kathleen Vinehout 2018
-	`SOS18P_LAF` Votes for Democratic Secretary of State primary candidate Doug La Follette 2018
-	`SOS18P_MAR` Votes for Democratic Secretary of State primary candidate Arvina Martin 2018
-	`TRES18P_SA` Votes for Democratic Treasurer primary candidate Dawn Marie Sass 2018
-	`TRES18P_KA` Votes for Democratic Treasurer primary candidate Cynthia Kaump 2018
-	`TRES18P_GOD` Votes for Democratic Governor primary candidate Sarah Godlewski 2018
