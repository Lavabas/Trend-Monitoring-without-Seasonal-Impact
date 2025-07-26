# Climatic Water Deficit Trend Analysis without Seasonal Impact in Polonnaruwa, Sri Lanka using Python API(Xee)
## Overview
This project analyzes long-term trends in climatic water deficit (DEF), a key drought and water stress indicator, for agricultural land in Eastern Polonnaruwa, Sri Lanka. Using monthly TerraClimate data (1980–2025), the analysis removes seasonal effects to highlight true underlying trends, detect change points, and quantify significant shifts in water availability over the last 40+ years.

## Objective
1. Analyze climatic water deficit trends in a paddy-dominated region of Sri Lanka.
2. Remove seasonal variation to detect long-term changes in moisture stress.

### Raw DEF Time Series (Monthly Average)
<img width="559" height="432" alt="image" src="https://github.com/user-attachments/assets/fc390c36-1d10-41cc-a2fb-c5d36c889cce" />

### Seasonal Decomposition Plot
<img width="630" height="470" alt="image" src="https://github.com/user-attachments/assets/b249b03f-a7e8-43ff-ad82-85f884ff4f94" />

### DEF Time Series - No Seasonal Influence (Monthly Average)
<img width="550" height="432" alt="image" src="https://github.com/user-attachments/assets/62042a09-bfc5-469a-b4aa-41b6ae5b410c" />

### Statistical tests show 
1. Seasonal noise has been effectively removed, allowing robust detection of trends.
2. The region has experienced a significant reduction in drought stress over the last four decades.
3. An important climatic or management change happened around 2006 that further contributed to the decrease in water deficit.

## Dataset
Dataset	- IDAHO_EPSCOR/TERRACLIMATE	
Temporal Coverage: 1980–2025
Unit Adjustment: DEF values were multiplied by 0.1 to scale them from tenths of mm to mm

## Tools and Libraries
Google Earth Engine Python API
1. geemap – ROI drawing and visualization
2. xee – Read GEE ImageCollections into xarray
3. xarray – For handling spatiotemporal data
4. pandas – DataFrame conversion
5. matplotlib – Plotting
6. statsmodels – Time series decomposition
7. pymannkendall – Mann-Kendall trend test
8. pyhomogeneity – Pettitt’s test for change-point detection



## Notes
1. Climatic Water Deficit (DEF) reflects the unmet atmospheric demand for water, i.e., the difference between PET and AET. Higher DEF indicates more stress.
2. Trend detection without seasonal cycles avoids false positives caused by the bimodal monsoon system in Sri Lanka.




