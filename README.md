# IITM-Project
Due to data provider policy, we are not able to share flux tower data. The data flolder contains only reanalysis data for KNP site. The other site data can be download from IMDAA \n(https://rds.ncmrwf.gov.in/dashboard/download) and ERA5 (https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=overview). The MODIS satellite data can be download from https://modis.gsfc.nasa.gov/data/.  
Latent heat flux (LE) is a fundamental component in the study of Earth’s energy balance
and the exchange of energy and water between the Earth’s surface and the atmosphere. It
refers to the amount of energy that is transferred from the surface to the atmosphere through
the process of evaporation, which involves the conversion of liquid water into water vapor.
This energy transfer is a critical component of the hydrologic cycle and plays an important
role in regulating the Earth’s climate. In this process, water vapor is transported from the
surface into the atmosphere, where it can condense and form clouds, releasing energy back
into the atmosphere. Understanding the mechanisms of latent heat flux is essential for pre-
dicting weather patterns, climate change, and the behavior of ecosystems. In this work,
reanalysis data is used to estimate LE. The variables to predict LE are air temperature, rel-
ative humidity, downward shortwave radiation, soil moisture, downward longwave radiation,
precipitation, air pressure, and vapor pressure deficit. The data is acquired from the Indian
Monsoon Data Assimilation and Analysis (IMDAA), European Centre for Medium-Range
Weather Forecasts (ERA5) reanalysis data, and Moderate Resolution Imaging Spectrora-
diometer (MODIS) sensors onboard the Terra satellite. The target variable is LE s estimated
by flux tower. To evaluate LE, the machine learning techniques linear regression, support
vector machine regressor, random forest regressor, Adaboost regressor, and gradient boost
regressor were utilized. In general, there was an error in the reanalysis data, which was
validated against the flux tower data. We have tried two procedures in this work. First,
we adjusted the reanalysis data and MODIS data with flux tower data to reduce errors for
input variables on one site. Different models are trained on ground-adjusted data and results
are compared with flux tower data. In this procedure, the results were good for the site on
which models are trained but required much improvement for other sites. Next, we train
models on five sites. The input data were reanalysis data and the target variable was LE
estimated by flux tower. This procedure has shown promise in estimating latent heat flux
from reanalysis data.  
The outputs of the mmodel are shown in the figures.
![Alt Text]()
