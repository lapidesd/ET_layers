# Supporting data and code for "Root water uptake resolved by distributed storage changes through soil and weathered bedrock"

This repository contains:

* Code:
  * massbal_etlayers_tdt.ipynb: a jupyter notebook to generate a background data figure for the study site, Elder Creek, CA
  * pyhydrus_VMS_final.ipynb: a jupyter notebook that runs a HYDRUS simulation at Elder Creek and evaluates performance of 3 mass balance-based methods for calculating depth-distributed ET and drainage fluxes
  * separate_fluxes-final.ipynb: a jupyter notebook that runs the best mass balance method (Method 3, minimum drainage method) on data from the vadose zone monitoring system (VMS) at Elder Creek, CA and explores the results
* Data:
  * tdt:
  * ElderPML.csv: csv file containing ET data from the gridded dataset PML-V2 (Gan et al., 2018; Zhang et al., 2019; Zhang et al., 2016)
  * Elder_streamflow.txt: USGS streamflow data for Elder Creek gage number 11475560 queried
  * Sapflow.csv: Sapflow data from trees at Elder Creek, previously published by Bilir et al. (2021)
  * angelo_weather_1H.csv: weather data for the Elder Creek area at Angelo Preserve
  * pet_data_frompete.csv: PET data for Elder Creek, mislabeled as Air Temp in file
 
References:

* Bilir, T. E., Fung, I., & Dawson, T. E. (2021). Slope‐aspect induced climate differences influence how water is exchanged between the land and atmosphere. Journal of Geophysical Research: Biogeosciences, 126(5), e2020JG006027.
* Gan, R., Zhang, Y., Shi, H., Yang, Y., Eamus, D., Cheng, L., ... & Yu, Q. (2018). Use of satellite leaf area index estimating evapotranspiration and gross assimilation for Australian ecosystems. Ecohydrology, 11(5), e1974.
* Zhang, Y., Kong, D., Gan, R., Chiew, F. H., McVicar, T. R., Zhang, Q., & Yang, Y. (2019). Coupled estimation of 500 m and 8-day resolution global evapotranspiration and gross primary production in 2002–2017. Remote sensing of environment, 222, 165-182.
* Zhang, Y., Peña-Arancibia, J. L., McVicar, T. R., Chiew, F. H., Vaze, J., Liu, C., ... & Pan, M. (2016). Multi-decadal trends in global terrestrial evapotranspiration and its components. Scientific reports, 6(1), 19124.
