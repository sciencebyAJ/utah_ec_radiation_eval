This repository evaluates net radiation at the UGS eddy covariance sites.
Included is the agweatherqaqc package to compare SW in to theoretical maximum valus. More information on agweatherqaqc is in the paper here
[![DOI](https://joss.theoj.org/papers/10.21105/joss.06368/status.svg)](https://doi.org/10.21105/joss.06368)

The solar_check.ipynb notebook includes the analysis: 

My main take-aways by site are:

Dugout:
* Smaller difference in net radiation overall.
* Differences in net radiation values appear to be driven by longwave radiation measurements. 
* Incoming LW radiation appears to drive the difference between the two sensors. 
* SWin measurements from SW_1_1_2 appear to regularly exceed clear sky maximum, although this is not the primary driver of net radiation differences.
* A next step could be to calculate LW incoming values to check which sensor is more representative.


Escalante:
* Larger difference in net radiation.
* Net radiation difference is driven by LW incoming radiation, especially during winter.
* During summer the net radiation difference is due to differences are driven by both SW and LW components
* A next step could be to calculate LW incoming values to check which sensor is more representative.

Bluff:
* Net radiation difference is driven by SW radiation.
* Shortwave incoming radiation sensor SW_IN_1_1_1 measures higher values than SW_IN_1_1_2. 
* Comparing SW_IN_1_1_1 to theoretical clear sky SW incoming values indicates the sensor measures values slightly higher than theory
* Comparing SW_IN_1_1_2 to theoretical clear sky SW incoming values indicates the sensor measures values slightly lower than theory, especially during June -September 2024 and April to July 2025. 
* An action could be to check field notes to see if the pyranometer was dusty or cloudy. Additionally, you can check to see if this sensor is outside of its calibration lifetime and needs to be re-calibrated.
* The difference in net radiation is primarily driven by SW out.
* SW_OUT_1_1_2 measures greater outgoing shortwave radiation than SW_OUT_1_1_1
* An action could be to check field notes to check the field of view for each sensor. If the sensors are capturing the same general land cover & shadows then the sensors should be inspected further. You may want to look into adjusting the location of one of the sensors given the difference in out-going SW, likely due to difference in albedo.

