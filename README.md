WI_VRA18 readme

Demographic data and general elections came with the ward geometries shapefile from The Wisconsin Legislature arcgis portal.
Metadata and notes on their process can be found here, including election data disaggregation:https://data-ltsb.opendata.arcgis.com/datasets/LTSB::2012-2020-election-data-with-2020-wards/about
and here for more detail on demographic data: https://www.arcgis.com/sharing/rest/content/items/f67c2e7f43bb432687b4a42bee50a16c/info/metadata/metadata.xml?format=default&output=html
Demographic data comes from 2011 and 2010 census blocks.

Primary election data was added to the shapefile from the following tabular source: https://elections.wi.gov/elections-voting/results/2014/partisan-primary
These elections were disaggregated to the ward level to be joined on to the state-provided shapefile.

Column definitions:

COUNTYFP- County FIPS code
COUNTY - County name (str)
NAME - Ward group name (str)
DISTRICT - 
POP - Total population
VAP - Voting age population
WHITE - White population
BLACK - Black Population
HISPANIC - Hispanic population
ASIAN - Asian population
AMIN - American Indian Alaskan Native population
NHPI - Native Hawaiian Pacific Islander Population
OTHER - Population of Other races
OTHERMLT - Population of Other races multiracial
WHITE18 - White population over 18 (WVAP)
BLACK18 - Black population over 18 (BVAP)
HISPANIC18 - Hispanic population over 18 (HVAP)
ASIAN18 - Asian population over 18 (HVAP)
AMIN18 - American Indian Alaskan Native population over 18 (AMINVAP)
NHPI18 - Native Hawaiian Pacific Island population over 18 (NHPIVAP) 
OTHER18 - Population of Other races over 18 (OTHERVAP)
OTHERMLT18 - Population of Other races over 18 multiracial
GOVTOT18 - Total votes for Governors race 2018
GOVR18 - Votes for Republican Gubernatorial candidate 2018 (Scott Walker)
GOVD18 - Votes for Democratic Gubernatorial candidate 2018 (Tony Evers)
SOSTOT18 - Total votes for Secretary of State race 2018
SOSR18 - Votes for Republican Seceratary of State candidate 2018 (Jay Shcroeder)
SOSD18 - Votes for Democratic Secretary of State candidate 2018 (Doug La Follette)
TRESTOT18 - Total votes for Treasurer race 2018
TRESR18 - Votes for Republican Treasurer candidate 2018 (Travis Hartwig)
TRESD18 - Votes for Democratic Treasurer candidate 2018 (Sarah Godlewski)
LG18P_KOBE - Votes for Democratic Lieutenant Governor primary candidate Kurt Kober 2018
LG18P_BARN - Votes for Democratic Lieutenant Governor primary candidate Mandela Barnes 2018
GOV18P_FLY - Votes for Democratic Governor primary candidate Matthew Flynn 2018
GOV18P_EVE - Votes for Democratic Governor primary candidate Tony Evers 2018
GOV18P_MCC - Votes for Democratic Governor primary candidate Michael McCabe 2018
GOV18P_MIT - Votes for Democratic Governor primary candidate Mahlon Mitchell 2018
GOV18P_ROY - Votes for Democratic Governor primary candidate Kelda Roys 2018
GOV18P_SOG - Votes for Democratic Governor primary candidate Paul Sogin 2018
GOV18P_VIN - Votes for Democratic Governor primary candidate Kathleen Vinehout 2018
SOS18P_LAF - Votes for Democratic Secretary of State primary candidate Doug La Follette 2018
SOS18P_MAR - Votes for Democratic Secretary of State primary candidate Arvina Martin 2018
TRES18P_SA - Votes for Democratic Treasurer primary candidate Dawn Marie Sass 2018
TRES18P_KA - Votes for Democratic Treasurer primary candidate Cynthia Kaump 2018
TRES18P_GOD - Votes for Democratic Governor primary candidate Sarah Godlewski 2018