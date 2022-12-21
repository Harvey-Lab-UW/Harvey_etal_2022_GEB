---
editor_options: 
  markdown: 
    wrap: sentence
---

# Harvey_etal_2023_GEB

Data accompanying the manuscript 'Spatial interactions among short-interval fires reshape forest landscapes' by Harvey, Buonanduci, and Turner published in Global Ecology and Biogeography.
See the main text of the manuscript for complete description of data processing.

[![CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by/4.0/)

This information is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).
Any user of these data ("User" hereafter) is required to cite it appropriately in any publication that results from its use.
These data may be actively used by others for ongoing research, so coordination may be necessary to prevent duplicate publication.
The User is urged to contact the authors of these data for questions about methodology or results.
The User is encouraged to consider collaboration or co-authorship with authors where appropriate.
Misinterpretation of data may occur if used out of context of the original study.
Substantial efforts are made to ensure accuracy of the data and documentation, however complete accuracy of data sets cannot be guaranteed.
All data are made available as is.
Data may be updated periodically and it is the responsibility of the User to check for new versions of the data.
The authors and the repository where these data were obtained shall not be liable for damages resulting from any use or misinterpretation of the data.

[![CC BY 4.0](https://i.creativecommons.org/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)

There are 14 main data files made available for reproducibility purposes:

-   NW_reburns_gridMET_drought.csv
-   NW_reburns_gridMET_weather.csv
-   NW_reburns_SR_landscape_metrics_RT_75.csv
-   NW_reburns_SR_landscape_metrics_75.csv
-   NW_reburns_SR_landscape_metrics_RT_90.csv
-   NW_reburns_SR_landscape_metrics_90.csv
-   NW_triple_SR_landscape_metrics_75.csv
-   NW_triple_SR_landscape_metrics_90.csv
-   NW_reburns_DTS_departure_75.csv
-   NW_reburns_DTS_departure_90.csv
-   NW_reburns_DTS_departure_RT_75.csv
-   NW_reburns_DTS_departure_RT_90.csv
-   NW_reburns_DTS_SDC_RT_75.csv
-   NW_reburns_DTS_SDC_RT_90.csv


### NW_reburns_gridMET_drought.csv

This file contains drought data associated with each fire. The following columns are included:

-   **Fire_ID**: unique fire identifier.
-   **Ig_Day**: date of year that fire was ignited (Julian Day).
-   **Order**: Code signifying 1st "First" or 2nd "Second" fire in reburned landscape.
-   **Reburn_Polygon_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Year**: Year of fire in YYYY.
-   **gm_Date**: The 15th day following the ignition date of the fire for which the EDDI and SPEI values were assigned (i.e., generating the 30-day window of 15 days prior to and 15 days after ignition date. 
-   **eddi30d**: Evaporative Demand Drought Index (EDDI, ranging from -2.5-wet to +2.5-dry) aggregated over the 30-day period centered on the ignition date (15 days prior to and 15 days after ignition) averaged over the spatial footprint of each reburned landscape.
-   **spei30d**: Standardized Precipitation-Evapotranspiration Index (SPEI) aggregated over the 30-day period centered on the ignition date (15 days prior to and 15 days after ignition) averaged over the spatial footprint of each reburned landscape.
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.


### NW_reburns_gridMET_weather.csv

This file contains fire weather data associated with each fire. The following columns are included: 

-   **Fire_ID**: unique fire identifier.
-   **Ig_Day**: date of year that fire was ignited (Julian Day).
-   **Order**: Code signifying 1st "First" or 2nd "Second" fire in reburned landscape.
-   **Reburn_Polygon_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Year**: Year of fire in YYYY.
-   **erc_max_max**: the maximum Energy Release Component (ERC) value for each pixel within the 30-day window centered on the Ig_Day (15 days prior and 15 days after) and then the maximum value selected within the spatial footprint of the reburn.
-   **erc_max_mean**: the maximum Energy Release Component (ERC) value for each pixel within the 30-day window centered on the Ig_Day (15 days prior and 15 days after) and then averaged among all pixels within the spatial footprint of the reburn.
-   **erc_mean_max**: the mean Energy Release Component (ERC) value for each pixel within the 30-day window centered on the Ig_Day (15 days prior and 15 days after) and then the maximum value selected within the spatial footprint of the reburn.
-   **erc_mean_mean**: the mean Energy Release Component (ERC) value for each pixel within the 30-day window centered on the Ig_Day (15 days prior and 15 days after) and then averaged among all pixels within the spatial footprint of the reburn.
-   **vpd_max_max**: the maximum Vapor Pressure Deficit (VPD) value for each pixel within the 30-day window centered on the Ig_Day (15 days prior and 15 days after) and then the maximum value selected within the spatial footprint of the reburn.
-   **vpd_max_mean**: the maximum Vapor Pressure Deficit (VPD) value for each pixel within the 30-day window centered on the Ig_Day (15 days prior and 15 days after) and then averaged among all pixels within the spatial footprint of the reburn.
-   **vpd_mean_max**: the mean Vapor Pressure Deficit (VPD) value for each pixel within the 30-day window centered on the Ig_Day (15 days prior and 15 days after) and then the maximum value selected within the spatial footprint of the reburn.
-   **vpd_mean_mean**: the mean Vapor Pressure Deficit (VPD) value for each pixel within the 30-day window centered on the Ig_Day (15 days prior and 15 days after) and then averaged among all pixels within the spatial footprint of the reburn.
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.


### NW_reburns_SR_landscape_metrics_RT_75.csv

This file contains landscape metrics of stand-replacing fire associated with each fire in a reburned landscape, using a threshold of stand-replacing fire of 75% basal area mortality from fire (of basal area live at time of fire) and calibrating RdNBR to different thresholds for stand-replacing fire in the second fire depending on whether a pixel burned as stand-replacing fire in the first fire. The following columns are included: 

-   **Reburn_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Reburn_Order**: Code for landscape metrics calculated for the first fire (Fire_1), second fire (Fire_2), union of the two fires (Either), and intersection of the two fires (Both) 
-   **Reburn_Interval**: Interval between 1st and 2nd fire (years) 
-   **Fire_ID**: unique fire identifier.
-   **Year**: Year of fire in YYYY.
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **class**: field indicating stand-replacing (2) or less than stand-replacing (1) 
-   **patch_area_mean**: mean patch size of stand-replacing patches (ha) 
-   **patch_area_AW_mean**: area-weighted mean patch size of stand-replacing patches (ha) 
-   **patch_PARA_mean**: mean edge-to-area ratio of stand-replacing patches.
-   **patch_PARA_AW_mean**: area-weighted mean edge-to-area ratio of stand-replacing patches.
-   **class_total_core_ha**: total core area within stand-replacing patches (ha); i.e. amount of area that is interior to stand-replacing patches and further than 150 m from patch edge.
-   **largest_patch_ind**: largest patch index (proportion of landscape composed of the largest patch of stand-replacing fire) 
-   **class_area_ha**: total area of stand-replacing fire (ha) 
-   **reburn_area_ha**: total area of reburned landscape (ha).
-   **class_prop**: proportion of fire burned as stand-replacing.


### NW_reburns_SR_landscape_metrics_75.csv

This file contains landscape metrics of stand-replacing fire associated with each fire in a reburned landscape, using a threshold of stand-replacing fire of 75% basal area mortality from fire (of basal area live at time of fire) and using the same RdNBR thresholds for stand-replacing fire in the second fire as in the first fire, regardless of severity in the first fire. The following columns are included: 

-   **Reburn_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Reburn_Order**: Code for landscape metrics calculated for the first fire (Fire_1), second fire (Fire_2), union of the two fires (Either), and intersection of the two fires (Both) 
-   **Reburn_Interval**: Interval between 1st and 2nd fire (years) 
-   **Fire_ID**: unique fire identifier.
-   **Year**: Year of fire in YYYY.
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **class**: field indicating stand-replacing (2) or less than stand-replacing (1) 
-   **patch_area_mean**: mean patch size of stand-replacing patches (ha) 
-   **patch_area_AW_mean**: area-weighted mean patch size of stand-replacing patches (ha) 
-   **patch_PARA_mean**: mean edge-to-area ratio of stand-replacing patches.
-   **patch_PARA_AW_mean**: area-weighted mean edge-to-area ratio of stand-replacing patches.
-   **class_total_core_ha**: total core area within stand-replacing patches (ha); i.e. amount of area that is interior to stand-replacing patches and further than 150 m from patch edge.
-   **largest_patch_ind**: largest patch index (proportion of landscape composed of the largest patch of stand-replacing fire) 
-   **class_area_ha**: total area of stand-replacing fire (ha) 
-   **reburn_area_ha**: total area of reburned landscape (ha).
-   **class_prop**: proportion of fire burned as stand-replacing.


### NW_reburns_SR_landscape_metrics_RT_90.csv

This file contains landscape metrics of stand-replacing fire associated with each fire in a reburned landscape, using a threshold of stand-replacing fire of 90% basal area mortality from fire (of basal area live at time of fire) and calibrating RdNBR to different thresholds for stand-replacing fire in the second fire depending on whether a pixel burned as stand-replacing fire in the first fire. The following columns are included: 

-   **Reburn_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Reburn_Order**: Code for landscape metrics calculated for the first fire (Fire_1), second fire (Fire_2), union of the two fires (Either), and intersection of the two fires (Both) 
-   **Reburn_Interval**: Interval between 1st and 2nd fire (years) 
-   **Fire_ID**: unique fire identifier.
-   **Year**: Year of fire in YYYY.
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **class**: field indicating stand-replacing (2) or less than stand-replacing (1) 
-   **patch_area_mean**: mean patch size of stand-replacing patches (ha) 
-   **patch_area_AW_mean**: area-weighted mean patch size of stand-replacing patches (ha) 
-   **patch_PARA_mean**: mean edge-to-area ratio of stand-replacing patches.
-   **patch_PARA_AW_mean**: area-weighted mean edge-to-area ratio of stand-replacing patches.
-   **class_total_core_ha**: total core area within stand-replacing patches (ha); i.e. amount of area that is interior to stand-replacing patches and further than 150 m from patch edge.
-   **largest_patch_ind**: largest patch index (proportion of landscape composed of the largest patch of stand-replacing fire) 
-   **class_area_ha**: total area of stand-replacing fire (ha) 
-   **reburn_area_ha**: total area of reburned landscape (ha).
-   **class_prop**: proportion of fire burned as stand-replacing.


### NW_reburns_SR_landscape_metrics_90.csv

This file contains landscape metrics of stand-replacing fire associated with each fire in a reburned landscape, using a threshold of stand-replacing fire of 90% basal area mortality from fire (of basal area live at time of fire) and using the same RdNBR thresholds for stand-replacing fire in the second fire as in the first fire, regardless of severity in the first fire. The following columns are included: 

-   **Reburn_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Reburn_Order**: Code for landscape metrics calculated for the first fire (Fire_1), second fire (Fire_2), union of the two fires (Either), and intersection of the two fires (Both) 
-   **Reburn_Interval**: Interval between 1st and 2nd fire (years) 
-   **Fire_ID**: unique fire identifier.
-   **Year**: Year of fire in YYYY.
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **class**: field indicating stand-replacing (2) or less than stand-replacing (1) 
-   **patch_area_mean**: mean patch size of stand-replacing patches (ha) 
-   **patch_area_AW_mean**: area-weighted mean patch size of stand-replacing patches (ha) 
-   *patch_PARA_mean*: mean edge-to-area ratio of stand-replacing patches.
-   **patch_PARA_AW_mean**: area-weighted mean edge-to-area ratio of stand-replacing patches.
-   **class_total_core_ha**: total core area within stand-replacing patches (ha); i.e. amount of area that is interior to stand-replacing patches and further than 150 m from patch edge.
-   **largest_patch_ind**: largest patch index (proportion of landscape composed of the largest patch of stand-replacing fire) 
-   **class_area_ha**: total area of stand-replacing fire (ha) 
-   **reburn_area_ha**: total area of reburned landscape (ha).
-   **class_prop**: proportion of fire burned as stand-replacing.


### NW_reburns_DTS_departure_RT_75.csv

This file contains values for the Menning Departure Index as one measure of changes in distributions of distances to seed source associated with each fire in a reburned landscape, using a threshold of stand-replacing fire of 75% basal area mortality from fire (of basal area live at time of fire) and calibrating RdNBR to different thresholds for stand-replacing fire in the second fire depending on whether a pixel burned as stand-replacing fire in the first fire. The following columns are included: 

-   **Fire_ID_1**: unique fire identifier for 1st fire in each reburned landscape.
-   **Fire_ID_2**: unique fire identifier for 2nd fire in each reburned landscape.
-   **Reburn_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Reburn_Interval**: Interval between 1st and 2nd fire (years) 
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **departure**: Menning Departure Index comparing differences in distributions of distance to seed source associated with each fire in a reburned landscape.


### NW_reburns_DTS_departure_75.csv

This file contains values for the Menning Departure Index as one measure of changes in distributions of distances to seed source associated with each fire in a reburned landscape, using a threshold of stand-replacing fire of 75% basal area mortality from fire (of basal area live at time of fire) and using the same RdNBR thresholds for stand-replacing fire in the second fire as in the first fire, regardless of severity in the first fire. The following columns are included: 

-   **Fire_ID_1**: unique fire identifier for 1st fire in each reburned landscape.
-   **Fire_ID_2**: unique fire identifier for 2nd fire in each reburned landscape.
-   **Reburn_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Reburn_Interval**: Interval between 1st and 2nd fire (years) 
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **departure**: Menning Departure Index comparing differences in distributions of distance to seed source associated with each fire in a reburned landscape.


### NW_reburns_DTS_departure_RT_90.csv

This file contains values for the Menning Departure Index as one measure of changes in distributions of distances to seed source associated with each fire in a reburned landscape, using a threshold of stand-replacing fire of 90% basal area mortality from fire (of basal area live at time of fire) and calibrating RdNBR to different thresholds for stand-replacing fire in the second fire depending on whether a pixel burned as stand-replacing fire in the first fire. The following columns are included: 

-   **Fire_ID_1**: unique fire identifier for 1st fire in each reburned landscape.
-   **Fire_ID_2**: unique fire identifier for 2nd fire in each reburned landscape.
-   **Reburn_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Reburn_Interval**: Interval between 1st and 2nd fire (years) 
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **departure**: Menning Departure Index comparing differences in distributions of distance to seed source associated with each fire in a reburned landscape.


### NW_reburns_DTS_departure_90.csv

This file contains values for the Menning Departure Index as one measure of changes in distributions of distances to seed source associated with each fire in a reburned landscape, using a threshold of stand-replacing fire of 90% basal area mortality from fire (of basal area live at time of fire) and using the same RdNBR thresholds for stand-replacing fire in the second fire as in the first fire, regardless of severity in the first fire. The following columns are included: 

-   **Fire_ID_1**: unique fire identifier for 1st fire in each reburned landscape.
-   **Fire_ID_2**: unique fire identifier for 2nd fire in each reburned landscape.
-   **Reburn_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Reburn_Interval**: Interval between 1st and 2nd fire (years) 
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **departure**: Menning Departure Index comparing differences in distributions of distance to seed source associated with each fire in a reburned landscape.


### NW_reburns_DTS_SDC_RT_75.csv

This file contains values for the Menning Departure Index as one measure of changes in distributions of distances to seed source associated with each fire in a reburned landscape, using a threshold of stand-replacing fire of 75% basal area mortality from fire (of basal area live at time of fire) and calibrating RdNBR to different thresholds for stand-replacing fire in the second fire depending on whether a pixel burned as stand-replacing fire in the first fire. The following columns are included: 

-   **Year_1**: Year of 1st fire in YYYY.
-   **Year_2**: Year of 2nd fire in YYYY.
-   **Interval**: Interval between 1st and 2nd fire (years) 
-   **Fire_ID_1**: unique fire identifier for 1st fire in each reburned landscape.
-   **Fire_ID_2**: unique fire identifier for 2nd fire in each reburned landscape.
-   **Fire_Name_1**: Fire name for 1st fire in each reburned landscape.
-   **Fire_Name_2**: Fire name for 2nd fire in each reburned landscape.
-   **Ig_Day_1**: date of year that 1st fire was ignited (Julian Day).
-   **Ig_Day_2**: date of year that 2nd fire was ignited (Julian Day).
-   **area_ha**: total area of reburned landscape (ha).
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Prp_forest**: proportion of reburned landscape area that is forested cover prior to 1st fire.
-   **FRG_1**: proportion of reburned landscape that is in Landfire Fire Regime Group 1.
-   **FRG_2**: proportion of reburned landscape that is in Landfire Fire Regime Group 2.
-   **FRG_3**: proportion of reburned landscape that is in Landfire Fire Regime Group 3.
-   **FRG_4**: proportion of reburned landscape that is in Landfire Fire Regime Group 4.
-   **FRG_5**: proportion of reburned landscape that is in Landfire Fire Regime Group 5.
-   **FRG_max5**: FRG with plurality of pixels in reburned landscape.
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   *Reburn_Polygon_ID*: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Reburn_Order**: Code for landscape metrics calculated for the first fire (Fire_1), second fire (Fire_2), union of the two fires (Either), and intersection of the two fires (Both) 
-   **SDC**: Stand-replacing Decay Coefficient (SDC) for each fire in a reburned landscape.


### NW_reburns_DTS_SDC_RT_90.csv

This file contains values for the Menning Departure Index as one measure of changes in distributions of distances to seed source associated with each fire in a reburned landscape, using a threshold of stand-replacing fire of 90% basal area mortality from fire (of basal area live at time of fire) and calibrating RdNBR to different thresholds for stand-replacing fire in the second fire depending on whether a pixel burned as stand-replacing fire in the first fire. The following columns are included: 

-   **Year_1**: Year of 1st fire in YYYY.
-   **Year_2**: Year of 2nd fire in YYYY.
-   **Interval**: Interval between 1st and 2nd fire (years) 
-   **Fire_ID_1**: unique fire identifier for 1st fire in each reburned landscape.
-   **Fire_ID_2**: unique fire identifier for 2nd fire in each reburned landscape.
-   **Fire_Name_1**: Fire name for 1st fire in each reburned landscape.
-   **Fire_Name_2**: Fire name for 2nd fire in each reburned landscape.
-   **Ig_Day_1**: date of year that 1st fire was ignited (Julian Day).
-   **Ig_Day_2**: date of year that 2nd fire was ignited (Julian Day).
-   **area_ha**: total area of reburned landscape (ha).
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Prp_forest**: proportion of reburned landscape area that is forested cover prior to 1st fire.
-   **FRG_1**: proportion of reburned landscape that is in Landfire Fire Regime Group 1.
-   **FRG_2**: proportion of reburned landscape that is in Landfire Fire Regime Group 2.
-   **FRG_3**: proportion of reburned landscape that is in Landfire Fire Regime Group 3.
-   **FRG_4**: proportion of reburned landscape that is in Landfire Fire Regime Group 4.
-   **FRG_5**: proportion of reburned landscape that is in Landfire Fire Regime Group 5.
-   **FRG_max5**: FRG with plurality of pixels in reburned landscape.
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **Reburn_Polygon_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Reburn_Order**: Code for landscape metrics calculated for the first fire (Fire_1), second fire (Fire_2), union of the two fires (Either), and intersection of the two fires (Both) 
-   **SDC**: Stand-replacing Decay Coefficient (SDC) for each fire in a reburned landscape.


### NW_triple_SR_landscape_metrics_75.csv

This file contains landscape metrics of stand-replacing fire associated with each fire in a thrice burned landscape, using a threshold of stand-replacing fire of 75% basal area mortality from fire (of basal area live at time of fire) and using the same RdNBR thresholds for stand-replacing fire in the second fire and third fire as in the first fire, regardless of severity in the first fire or the second fire. The following columns are included: 

-   **Reburn_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Reburn_Order**: Code for landscape metrics calculated for the first fire (Fire_a), second fire (Fire_b), third fire (Fire_c), union of the three fires (any), and intersection of the three fires (all) 
-   **Reburn_Interval_1**: Interval between 1st and 2nd fire (years) 
-   **Reburn_Interval_2**: Interval between 2nd and 3rd fire (years) 
-   **Fire_ID**: unique fire identifier.
-   **Year**: Year of fire in YYYY.
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **class**: field indicating stand-replacing (2) or less than stand-replacing (1) 
-   **patch_area_mean**: mean patch size of stand-replacing patches (ha) 
-   **patch_area_AW_mean**: area-weighted mean patch size of stand-replacing patches (ha) 
-   **patch_PARA_mean**: mean edge-to-area ratio of stand-replacing patches.
-   **patch_PARA_AW_mean**: area-weighted mean edge-to-area ratio of stand-replacing patches.
-   **class_total_core_ha**: total core area within stand-replacing patches (ha); i.e. amount of area that is interior to stand-replacing patches and further than 150 m from patch edge.
-   **largest_patch_ind**: largest patch index (proportion of landscape composed of the largest patch of stand-replacing fire) 
-   **class_area_ha**: total area of stand-replacing fire (ha) 
-   **reburn_area_ha**: total area of reburned landscape (ha).
-   **class_prop**: proportion of fire burned as stand-replacing.


### NW_triple_SR_landscape_metrics_90.csv

This file contains landscape metrics of stand-replacing fire associated with each fire in a thrice burned landscape, using a threshold of stand-replacing fire of 90% basal area mortality from fire (of basal area live at time of fire) and using the same RdNBR thresholds for stand-replacing fire in the second fire and third fire as in the first fire, regardless of severity in the first fire or the second fire. The following columns are included: 

-   **Reburn_ID**: unique identifier of reburned landscape that combines the values in the field "Fire_ID" for the 1st and 2nd fire in each reburned landscape.
-   **Polygon_ID**: Polygon ID for reburned landscape (=1 unless reburned landscape is more than one polygon) 
-   **Reburn_Order**: Code for landscape metrics calculated for the first fire (Fire_a), second fire (Fire_b), third fire (Fire_c), union of the three fires (any), and intersection of the three fires (all) 
-   **Reburn_Interval_1**: Interval between 1st and 2nd fire (years) 
-   **Reburn_Interval_2**: Interval between 2nd and 3rd fire (years) 
-   **Fire_ID**: unique fire identifier.
-   **Year**: Year of fire in YYYY.
-   **Ecoregion**: EPA Level III Ecoregion for plurality of area within fire footprint.
-   **N_Rockies**: Region lumped by EPA Level III Ecoregion into either "Northern Rockies" or "Pacific Northwest" 
-   **FRG_max4**: the dominant fire regime for each reburned landscape designated by the fire regime (LSF, MSF, HSF) with a plurality of pixels within the spatial footprint.
-   **class**: field indicating stand-replacing (2) or less than stand-replacing (1) 
-   **patch_area_mean**: mean patch size of stand-replacing patches (ha) 
-   **patch_area_AW_mean**: area-weighted mean patch size of stand-replacing patches (ha) 
-   **patch_PARA_mean**: mean edge-to-area ratio of stand-replacing patches.
-   **patch_PARA_AW_mean**: area-weighted mean edge-to-area ratio of stand-replacing patches.
-   **class_total_core_ha**: total core area within stand-replacing patches (ha); i.e. amount of area that is interior to stand-replacing patches and further than 150 m from patch edge.
-   **largest_patch_ind**: largest patch index (proportion of landscape composed of the largest patch of stand-replacing fire) 
-   **class_area_ha**: total area of stand-replacing fire (ha) 
-   **reburn_area_ha**: total area of reburned landscape (ha).
-   **class_prop**: proportion of fire burned as stand-replacing.
