# Hieratical-forecasting
This project aim to illustrate the algo of Hirratical-forecasting
1) Botton-up approach 
An advantage of this approach is that we are forecasting at the bottom-level of a structure, and therefore no information is lost due to aggregation. On the other hand, bottom-level data can be quite noisy and more challenging to model and forecast.
As for X, Forecast is made at BU-Province level and aggregated into country level, and LDP enriched in Country level only currently. 


![image](https://user-images.githubusercontent.com/65513033/154527049-96b60299-bccb-4f4e-9645-885c165684df.png)

![image](https://user-images.githubusercontent.com/65513033/154528226-fd63c019-5bbc-49ee-a819-5aa1a7ce94d4.png)
* MAPE Calculated using the formular above and it s 6 months´ MAPE(2020.3-2020.8)
** MAPE Calculated using the formular above and it s 6 months´ MAPE(2020.3-2020.8), suppose without regressors, as no regressor added on GMID level.

Top-down approaches (Previously in Manugistics, different hierarchical fcst methods between first three forecasting months and the months left)

Forecast proportions-Because historical proportions used for disaggregation do not take account of how those proportions may change over time, top-down approaches based on historical proportions tend to produce less accurate forecasts at lower levels of the hierarchy than bottom-up approaches. To address this issue, proportions based on forecasts rather than historical data can be used (Athanasopoulos, Ahmed, & Hyndman, 2009).

Consider a one level hierarchy. We first generate h -step-ahead forecasts for all of the series. We don’t use these forecasts directly, and they are not coherent (they don’t add up correctly). Let’s call these “initial” forecasts. We calculate the proportion of each  h-step-ahead initial forecast at the bottom level, to the aggregate of all the h -step-ahead initial forecasts at this level. We refer to these as the forecast proportions, and we use them to disaggregate the top-level  h -step-ahead initial forecast in order to generate coherent forecasts for the whole of the hierarchy.                                                                
                                                                                                                                                                                                                                                          * reference:https://otexts.com/fpp2/top-down.html

Data Visulization about the sales distribution on BU and province to better communicate with our stakeholders




