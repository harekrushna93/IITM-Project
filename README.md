# IITM-Project
Due to data provider policy, we are not able to share flux tower data. The data folder contains only reanalysis data for the KNP site. The other site data can be download from IMDAA \n(https://rds.ncmrwf.gov.in/dashboard/download) and ERA5 (https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=overview). The MODIS satellite data can be downloaded from https://modis.gsfc.nasa.gov/data/.  


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
We have studied the effectiveness of machine learning-based algorithms for predicting latent
heat flux using reanalysis data at different sites in the tropical region. The purpose of using
reanalysis data for prediction was that it is easily available to all. Two methods are adopted
with five algorithms each for the prediction of LE. We have built five models in method-I,
and out of the five models, the SVM regression model has the best prediction values. The
R2 score of the model was 0.9 and the RMSE between predicted LE values and ground-
adjusted LE was 16.2 W m−2 during the period 2000 − 2021. The RMSE between predicted
LE values and Flux tower estimation LE was 16.8 W m−2 during the period 2016 − 2018.
The LE values more than 95 W m−2 can not be captured. The method-I is more focused on
a single site: KNP, whereas Method II is more general than method-I. The performance of
models in method-I can be improved by increasing the training dataset size and accuracy
of the input variables. This method can be applied to the KNP site only. The method-II
can be applied to more than one side. The site selection for method II plays an important
role in the performance of models. The similarity in climate conditions, elevations, and the
LE value ranges is needed in method II to enhance the estimation results. If the number of
sites is large, the similarity conditions can be omitted by adding vegetation type, soil type,
climate type, etc to input features for estimations. In conclusion, data-driven methods offer
a potential means to predict the Latent Heat Flux using reanalysis data.


