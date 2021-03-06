# Appliances-Energy-Prediction
This project deals with predicting appliances energy consumption of a particular household in Belgium based on the temperature and humidity levels of different rooms in the building and the weather reports in the area over a period of 4.5 months.
# Dataset link:-
https://drive.google.com/drive/u/0/folders/1ZZXTFzQ6bJs3CVzLHGsgSy_1sCIErqOz
# Dataset Information:-
The data set is at 10 min for about 4.5 months. The house temperature and humidity conditions were monitored with a ZigBee wireless sensor network. Each wireless node transmitted the temperature and humidity conditions around 3.3 min. Then, the wireless data was averaged for 10 minutes periods. The energy data was logged every 10 minutes with m-bus energy meters. Weather from the nearest airport weather station (Chievres Airport, Belgium) was downloaded from a public data set from Reliable Prognosis (rp5.ru) and merged together with the experimental data sets using the date and time column. Two random variables have been included in the data set for testing the regression models and to filter out non-predictive attributes (parameters).
# Aim of Project:-
Experimental data used to create regression models of appliances energy use in a low energy building.
# Attribute information:-
* date time year-month-day hour:minute:second
* Appliances, energy use in Wh
* lights, energy use of light fixtures in the house in Wh
* T1, Temperature in kitchen area, in Celsius
* RH_1, Humidity in kitchen area, in %
* T2, Temperature in living room area, in Celsius
* RH_2, Humidity in living room area, in %
* T3, Temperature in laundry room area
* RH_3, Humidity in laundry room area, in %
* T4, Temperature in office room, in Celsius
* RH_4, Humidity in office room, in %
* T5, Temperature in bathroom, in Celsius
* RH_5, Humidity in bathroom, in %
* T6, Temperature outside the building (north side), in Celsius
* RH_6, Humidity outside the building (north side), in %
* T7, Temperature in ironing room , in Celsius
* RH_7, Humidity in ironing room, in %
* T8, Temperature in teenager room 2, in Celsius
* RH_8, Humidity in teenager room 2, in %
* T9, Temperature in parents room, in Celsius
* RH_9, Humidity in parents room, in %
* To, Temperature outside (from Chievres weather station), in Celsius
* Pressure (from Chievres weather station), in mm Hg
* RH_out, Humidity outside (from Chievres weather station), in %
* Wind speed (from Chievres weather station), in m/s
* Visibility (from Chievres weather station), in km
* Tdewpoint (from Chievres weather station), ????C
* rv1, Random variable 1, nondimensional
* rv2, Random variable 2, nondimensional


Where indicated, hourly data (then interpolated) from the nearest airport weather station (Chievres Airport, Belgium) was downloaded from a public data set from Reliable Prognosis, rp5.ru. Permission was obtained from Reliable Prognosis for the distribution of the 4.5 months of weather data.
# Conclusion
* The temperature/ humidity features showed little to no correlation w.r.t to target variable (<1%), although being highly correlation among each other.

* The time zone of the day plays an important role in deciding power consumption of appliances.

* The best Algorithm to use for this dataset is Extra Trees Regressor

* PCA helped us to reduce our feature set dimension considerably without affcting performance of our models significantly.

* The untuned model was able to explain 63% of variance on test set, while the tuned model was able to explain 64% of variance on test set which is improvement of 1.5 %

* The least RMSE score on test data set is found to be around 0.6.
