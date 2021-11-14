# charges

data from:
https://gis-mdc.opendata.arcgis.com/datasets/jail-bookings-may-29-2015-to-current/explore

with a list of codes (Ex. 32733001) and knowledge of what stuff like (FRA SUB MIS WO CM AP) means,
I think this is pretty reasonable to clean

i think we MUST look at all 6 columns. the "Code2" column sometimes 
contains charge description instead of a code.
sometimes the "Charge1" column contains multiple charges.

i would rather have ONE charge column that contains all of the charge codes in a list. like this:
[84308102, 78703001, 89610105B]

and a lookup table or excel sheet that maps charge_codes to charges
84308102 -> Robbery

*** I am very interested in how law enforcement is ENTERING THE DATA ***
there may be a change to existing jail booking software that would allow ease of data collection AND
reduce the amount of data preprocessing needed

letting the person doing the jail booking type in a charge and having them select 
from a drop down list would help make future data more clean
