# Supporting data and code for "Root water uptake resolved by distributed storage changes through soil and weathered bedrock"

[![DOI](https://zenodo.org/badge/753748865.svg)](https://zenodo.org/doi/10.5281/zenodo.12537869)

This repository contains:

* Code:
  * massbal_etlayers_tdt.ipynb: a jupyter notebook to generate a background data figure for the study site, Elder Creek, CA
  * pyhydrus_manysites_explore.ipynb: a jupyter notebook that explores HYDRUS simulations run in pyhydrus_manysites_run.ipynb across 9 climate type locations
  * pyhydrus_manysites_run.ipynb: a jupyter notebook that runs HYDRUS simulations at 9 climate type locations across the Conterminous US and downloads the data for exploration in pyhydrus_manysites_explore.ipynb
  * pyhydrus_VMS_final.ipynb: a jupyter notebook that runs a HYDRUS simulation at Elder Creek and evaluates performance of 3 mass balance-based methods for calculating depth-distributed ET and drainage fluxes
  * separate_fluxes-final-github.ipynb: a jupyter notebook that runs the best mass balance method (Method 3, minimum drainage method) on data from the vadose zone monitoring system (VMS) at Elder Creek, CA and explores the results
* Data:
  * tdt: directory containing tdt data for each layer A1-A10. Raw data are stored in the column titled Vms_Rock_Moisture_A1
  * etdata_#CLIMATE TYPE#.csv: set of files with ET data from HYDRUS slimulations for each climate type. Time is time in days since 1-1-2016. vRoot is ET from HYDRUS over the full column in cm.
  * petdata_#CLIMATE TYPE#.csv: set of files with ET data from gridMET (Abatzoglou, 2013) for each climate type. Time is time in days since 1-1-2016, and PET is ET from gridMET in cm.
  * raindata_#CLIMATE TYPE#.csv: set of files with precipitation data from gridMET (Abatzoglou, 2013) for each climate type. Timestamp is the date. Time is the time in days since 1-1-2016. Prec is the precipitation from gridMET in cm.
  * data_for_datafig.csv: csv file containing data needed for data figure in massbal_etlayers_tdt.ipynb. Columns A1-A9 are tdt data from VMS, Rivendell_WY_Rain_mm is rainfall, well_10_adjust and well_07_adjust are well data, and PET_mmd is PET
  * ElderPML.csv: csv file containing ET data from the gridded dataset PML-V2 (Gan et al., 2018; Zhang et al., 2019; Zhang et al., 2016)
  * Elder_streamflow.txt: USGS streamflow data for Elder Creek gage number 11475560 queried
  * Sapflow.csv: Sapflow data from trees at Elder Creek, previously published by Bilir et al. (2021)
  * site_info.csv: Site information for 9 different climate types. Climte_type column is the label for each climate type. Longitude and Latitude provide the location of the representative point for each climate type. Aridity is PET/P using data from gridMET (Abatzoglou, 2013). P and PET and precipitation and PET from gridMET. Asynch is the asynchronicity index, calculated following Feng et al. (2019).
  * SNorth.csv: Soil moisture data for north slope of Elder Creek site, where VMS is located
  * SSouth.csv: Soil moisture data for south slope of Elder Creek site
  * angelo_weather_1H.csv: weather data for the Elder Creek area at Angelo Preserve
  * pet_data_hargreaves.csv: PET data for Elder Creek, mislabeled as Air Temp in file, calculated using the Hargreaves formula
 
References:

* Abatzoglou, J. T. (2013), Development of gridded surface meteorological data for ecological applications and modelling. Int. J. Climatol., 33: 121–131.
* Bilir, T. E., Fung, I., & Dawson, T. E. (2021). Slope‐aspect induced climate differences influence how water is exchanged between the land and atmosphere. Journal of Geophysical Research: Biogeosciences, 126(5), e2020JG006027.
* Feng, Xue, et al. "Quantifying asynchronicity of precipitation and potential evapotranspiration in Mediterranean climates." Geophysical Research Letters 46.24 (2019): 14692-14701.
* Gan, R., Zhang, Y., Shi, H., Yang, Y., Eamus, D., Cheng, L., ... & Yu, Q. (2018). Use of satellite leaf area index estimating evapotranspiration and gross assimilation for Australian ecosystems. Ecohydrology, 11(5), e1974.
* Zhang, Y., Kong, D., Gan, R., Chiew, F. H., McVicar, T. R., Zhang, Q., & Yang, Y. (2019). Coupled estimation of 500 m and 8-day resolution global evapotranspiration and gross primary production in 2002–2017. Remote sensing of environment, 222, 165-182.
* Zhang, Y., Peña-Arancibia, J. L., McVicar, T. R., Chiew, F. H., Vaze, J., Liu, C., ... & Pan, M. (2016). Multi-decadal trends in global terrestrial evapotranspiration and its components. Scientific reports, 6(1), 19124.
