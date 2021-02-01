# Script for skill analysis of drought indicators SPI/ SPEI 

## `spi_spei_analysis.R`

The script to calculate skill scores (POD and FAR) of SPI, SPEI vs impact proxy crop yield.

The outputs are figures of SPI/SPEI against crop yield, maps of skill scores per livelihood zones, csv and shapefiles with the scores.

### Usage:

Load input data as instructed in the script, then call the function `skill_analysis` with the correct order of syntax: 

`skill_analysis(si_type, si, si_thr, crop_type, yield.df, yield_anomaly_thr, countryshape, livelyzoneshape)`

Where:

   `si_type`: standardised index type (string)  
   `si`: loaded nc file of the standardised index  
   `si_thr`: the standardised index threshold (single value)  
   `crop_type`: crop yield type (string)  
   `yield.df`: data.frame of the crop yield  
   `yield_anomaly_thr`: crop yield anomaly (single value)  
   `countryshape`: shapefile of country (for cropping global dataset with country extent)  
   `livelyzoneshape`: shapefile of livelihood zones (for calculation)  
