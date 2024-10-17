# Heat Vulnerability Index for England, Wales and Scotland

A repo containing Heat Vulnerability Index datasets for England, Wales and Scotland.

## England and Wales

Data is from 2022 Climate Just Indices. Heat disadvantage  includes climate data (average temperature of top 5% hottest days) and social vulnerability to heat (sensitivity, ability to prepare, ability to respond, ability to recover, enhanced exposure). 

Heat disadvantage is a binary classification. The top 20% most disadvantaged for the combined climate and social vulnerability score (calculated by ClimateJust) is represented by a 1. Classification is calculated separately for England and Wales. There are two scenarios - baseline temperatures (uses temperatures of recent past (20 year mean, 1990-2019) and 1.5 degree scenario).

#### Columns
- "ls11_cd"  - LSOA (2011) code
- "ls11_nm"  - LSOA name
- "ht_bsln"  - heat disadvantage score; baseline
- "ht_1_5_"  - heat disadvantage score; 1.5 degree scenario
- "ht_bsl_"  - heat disadvantage binary classifcation (1 - heat disadvantaged, 0 - not heat disadavantaged); baseline scenario
- "h_1_5__"  - heat disadvantage binary classifcation (1 - heat disadvantaged, 0 - not heat disadavantaged); 1.5 degree scenario
- "geometry" - boundaries for LSOA

Source: Climate Just (2022), Climate data from Kennedy-Asser, AT et al 2022 Environ. Res. Lett. 17 034024, UKCP18 12km RCP 8.5 95th percentile data

## Scotland

Data is from 4EI heat hazard index and IMD. Heat hazard scoring analyses land surface temperature, averaged over a specific
time period. No climate Just data available for Scotland. 

Heat disadvantage is a binary classification. Classification is based on areas in hazard areas 4 and 5 (out of 5), and IMD 1, 2 and 3, represented by a 1. Classification is calculated separately for Scotland.
There is one scenario - temperatures of recent past.

#### Columns
- "dz11_cd"  - Data Zone (2011) code
- "hazard"   - Heat hazard score (5 - highest hazard, 1 - lowest hazard)    
- "imd"      - IMD score (10 - most deprived, 1 - least deprived)
- "ht_dsd_"  - heat disadvantage binary classifcation (1 - heat disadvantaged, 0 - not heat disadavantaged)
- "dz11_nm"  - DZ name
- "geometry" - boundaries for DZ

Source: 4 Earth Intelligence

## Northern Ireland

No climate just or heat hazard data is available.
