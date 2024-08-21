# The "Jared Is Miserable" (JIM) Index
## Written by Jared Rennie (@jjrennie)
> "Misery, she needs me, but I need her more"
> --- Metallica

If you're looking for a metric to objectively decide good weather days from bad, then you're at the wrong place. I'd suggest checking out someone else's site like [this one](https://www.cbsnews.com/boston/news/how-many-top-10-weather-days-do-we-get-in-boston/)

This notebook creates times in the Contiguous US where Jared would be miserable. After extensive analysis and peer-review research, the "JIM" is defined as the following:

$Td>=55°F$

Because it's literally not the heat, it's the humidity! This notebook utilizes the [High-Resolution Rapid Refresh (HRRR)](https://rapidrefresh.noaa.gov/hrrr/) model stored in AWS in ZARR format. This is maintained by MesoWest, and their description of HRRR in ZARR format is [here](https://mesowest.utah.edu/html/hrrr/)

### What You Need

First off, the entire codebase works in Python... sort of. 

You will need the following programs installed: 
- Python
- s3fs | numpy | xarray | matplotlib | cartopy | h5netcdf | h5py | zarr | metpy
    
The "easiest" way is to install these is by installing <a href='https://www.anaconda.com/' target="_blank">Anaconda</a>, and then applying <a href='https://conda-forge.org/' target="_blank">conda-forge</a>. Afterward, then you can install the above packages. 

### Launch now with Binder:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jjrennie/Jared-Is-Miserable/HEAD?labpath=JIM.ipynb)
