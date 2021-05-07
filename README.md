# mcSA
Short script to calculate the stand-adjusted (Wotton &amp; Beverly 2007) fine fuel moisture content estimate for wildfire behaviour prediction, based on the Canadian Forest Fire Danger Rating System. 

Stand-adjusted moisture content model for conifer forests; uses stand type, density, and season variables in addition to FFMC and DMC from the Canadian FWI System

Requires FFMC, DMC, 
stand (1:5; deciduous, Douglas-fir, mixedwood, pine, spruce), 
density (1:3; light, mod, dense), 
season (1, 1.5, 2, 3; spring, spr-sum transition, sum, fall); 
season==1.5 represents spring/summer transition (uses half of spring, half of summer estimate).

The present code produces a function that can be used in a variety of contexts. 
E.g. FFMC 90.5, DMC 70, pine, moderate density, summer:

```{r}
samc(90.5, 70, 4, 2, 2)

> 9.537645
```

Note that the mcSA behaves counter-intuitively at high FFMC levels; this is particularly a problem with 'high' density (density==3 in the function). 
See the 'ConPyro' branch for more details and a version that address this. 

#D.Perrakis, May 2021; daniel.perrakis@canada.ca


