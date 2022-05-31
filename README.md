# Airline-Delay-and-Timeseries-Analysis
#### Extensive Exploratory Data Analysis

--- 
## 1. Data: https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp?20=E
#### Duration: 2013 to 2020

The dataset has 73282 data points. 

----
# Notebook 1: 01_Exploration.ipynb
## 1. Data Cleaning
* Check for consistency in column names
* Missing Data Treatment
* Drop duplicates
* Check for data consistency (Carrier code and Carrier Names), and clean them

## 2. Exploratory Data Analysis
* Plots and Inferences


# Notebook 2: 02_Forecasting.ipynb
* Import clean data (Generated in EDA)
* Create Train, Validation and Test set
* Check for Stationarity and Make series stationary
* Check for ACF and PACF
* Apply ARIMA and SARIMA
* Forecast 'What if there was no covid-19…?'

---

### The features of the dataset are:
1. **year**: year of the data point
2. **month**: month of the data point
3. **carrier**: The airline carrier code
4. **carrier_name**: Name of the Airline Carrier
5. **airport**: code of the airport
6. **airport_name**: Name of the airport 
7. **arr_flights**: Number of flights arrived in that airport
8. **arr_del15**: Number of delayed flights arrived. The flights that are delayed by 15 or more minutes are considered as delayed
9. **carrier_ct**: Number of flights delayed due to the circumstances within the airline's control (e.g. maintenance or crew problems, aircraft cleaning, baggage loading, fueling, etc.).
10. **weather_ct**: Number of flights delayed due to extreme weather conditions, such as hurricane, snowstorm etc.
11. **nas_ct**: Number of flights delayed due to National Aviation System (NAS). NAS has broad set of conditions such as non-extreme weather, airport operations, heavy traffic volume, and air traffic control.
12. **security_ct**: Number of flights delayed due to airport/flight security reasons such as re-boardig of aircraft due to security breach, inoperative screening equipment or long queues.
13. **late_aircraft_ct**: Number of flights delayed due to a previous flight with same aircraft arrived late, causing the present flight to depart late.
14. **arr_cancelled**: Number of flights cancelled.
15. **arr_diverted**: Number of flights diverted to other airports. Some of the reasons for diversons are Bad Weather, Mechanical issue/ less fuel in the aircraft, Unruly Passenger, and Medical Emergency ... etc
16. **arr_delay**: Delay time in minutes of the flights that arrived late.
17. **carrier_delay**: Delay time in minutes of the flights that are delayed due to the circumstances within the airline's control. Time of delay for the flights in carrier_ct.
18. **weather_delay**: Delay time in minutes of the flights that are delayed due to extreme weather conditions. Time of delay for the flights in weather_ct.
19. **nas_delay**: Delay time in minutes of the flights that are delayed due to the circumstances within the NAS's control. Time of delay for the flights in nas_ct.
20. **security_delay**: Delay time in minutes of the flights that are delayed due to the process of security check in the airport. Time of delay for the flights in security_ct.
21. **late_aircraft_delay**: Delay time in minutes of the flights that are delayed due to the delay in arrival of the same aircraft.





References used for analysis:
* https://simpleflying.com/american-airlines-us-airways-merger/#:~:text=American%20Airlines%20and%20US%20Airways,largest%20airline%20at%20the%20time
* https://www.transtats.bts.gov/Tables.asp?QO_VQ=EFD&QO_anzr=Nv4yv0r%FDb0-gvzr%FDcr4s14zn0pr%FDQn6n&QO_fu146_anzr=b0-gvzr
* https://en.wikipedia.org/wiki/ExpressJet
* https://en.wikipedia.org/wiki/Pinnacle_Airlines_Corp.
* https://en.usvisaservice.de/us-visa-news/article/us-travel-ban-coronavirus/
* https://www.transtats.bts.gov/Fields.asp?gnoyr_VQ=FGK
* Master Thesis: Jetzki, Martina. "The propagation of air transport delays in Europe." Master's thesis, RWTH Aachen University, Airport and Air Transportation Research (2009).


