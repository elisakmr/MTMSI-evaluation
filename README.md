# MTMSI-evaluation
We describe the R package that enables to evaluate MTMSI reanalysis of annual maxima of snow depth.
Codes are describes in the order that the user should follow too.
Each file has first a "packages" section that should be run, and sometimes also a "parameters" section that can be modified by the user.

## Extraction codes
  # 1.  MTMSI_extract
  The code enables the extraction of daily snow depth values from a netcdf file, along with the metadata of each series of values. 
  Daily maxima are also used to compute the annual maxima.
  
  # 2.  nuts_extract
  The code enables to build 3 shapefiles with increasing details about the NUTS-3, that are required for the majority of the remaining codes.

  # 3.  map_elevation
  The code enables to build the NUTS-3 mean elevation and the NUTS type maps side by side.

  # 3.  obs_extract_alp, obs_extract_ger, obs_extract_fin, obs_extract_ecad
  The codes enable the extraction of
  - daily values of snow depth per station
  - derived annual maxima of snow depth
  - shapefile of the stations that provided the measures
 
  # 3.  obs_extract_merged
  The code enables in-situ data merging
  - merging of the annual maxima
  - merging of the shapefiles
  
  # 4.  obs_nbyear & obs_prop_dispo
  The codes enable to depict data availability of the in-situ datasets with two plots

  # 4.  shp_nbSTAT & map_NBstations
  The codes enable to first build the shapefile of the amount of stations per NUTS-3, and then map it.

  # 5.  mtmsi_timeseries
  The user can choose a NUTS-3 id and elevation, and the timeseries is plot against the in-situ timeseries.
  
  # 5.  score
  The code compute multiple scores for each NUTS/elevation pair, that are stored in lists.

  # 5.  score_histogram
  The user can plot a histogram giving the proportion of the MTMSI data set that has been evaluated, by 500m elevation range.

  # 6.  score_boxplot
  The code enables to build boxplots of the correlation and bias scores, as well as the median intercorrelation, 
  per 500m elevation range.

  # 6.  shp_SCORE_meanalt & map_scores
  The code enables to build the shapefiles of the selected score on each of the NUTS-3 mean elevation, and map it 
  (side by side or single map).



