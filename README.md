# mcSA
Short script to calculate the stand-adjusted (Wotton &amp; Beverly 2007) fine fuel moisture content estimate for wildfire behaviour prediction, based on the Canadian Forest Fire Danger Rating System. 

Stand-adjusted moisture content model for conifer forests; uses stand type, density, and season variables in addition to FFMC and DMC from the Canadian FWI System

Requires FFMC, DMC, 
stand (1:5; deciduous, Douglas-fir, mixedwood, pine, spruce), 
density (1:3; light, mod, dense), 
season (1, 1.5, 2, 3; spring, spr-sum transition, sum, fall)
season==1.5 represents spring/summer transition (uses half of spring, half of summer estimate);

#D.Perrakis, October 2020; daniel.perrakis@canada.ca
