#Flight USA EDA
## by Ouedraogo Ami Samyra


## Dataset

> Provide basic information about your dataset in this section. If you selected your own dataset, make sure you note the source of your data and summarize any data wrangling steps that you performed before you started your exploration.
The data consists of flight arrival and departure details for all commercial flights within the USA, from October 1987 to April 2008. This is a large dataset: there are nearly 120 million records in total, and takes up 1.6 gigabytes of space compressed and 12 gigabytes when uncompressed.
for this analysis i decided to work with the fligts information over 2007. Below you can find all the informations concerning each variable:
- Year 2007
- Month 1-12
- DayofMonth 1-31
- DayOfWeek 1 (Monday) - 7 (Sunday)
- DepTime actual departure time (local, hhmm)
- CRSDepTime scheduled departure time (local, hhmm)
- ArrTime actual arrival time (local, hhmm)
- CRSArrTime scheduled arrival time (local, hhmm)
- UniqueCarrier unique carrier code
- FlightNum flight number
- TailNum plane tail number: aircraft registration, unique aircraft identifier
- ActualElapsedTime in minutes
- CRSElapsedTime in minutes
- AirTime in minutes
- ArrDelay arrival delay, in minutes: A flight is counted as "on time" if it operated less than 15 minutes later the scheduled time shown in the -carriers' Computerized Reservations Systems (CRS).
- DepDelay departure delay, in minutes
- Origin origin IATA airport code
- Dest destination IATA airport code
- Distance in miles
- TaxiIn taxi in time, in minutes
- TaxiOut taxi out time in minutes
- Cancelled was the flight cancelled
- CancellationCode reason for cancellation (A = carrier, B = weather, C = NAS, D = security)
- Diverted 1 = yes, 0 = no
- CarrierDelay in minutes: Carrier delay is within the control of the air carrier. Examples of occurrences that may determine carrier delay are: -aircraft cleaning, aircraft damage, awaiting the arrival of connecting passengers or crew, baggage, bird strike, cargo loading, catering, -computer, outage-carrier equipment, crew legality (pilot or attendant rest), damage by hazardous goods, engineering inspection, fueling, handling disabled passengers, late crew, lavatory servicing, maintenance, oversales, potable water servicing, removal of unruly passenger, slow boarding or seating, stowing carry-on baggage, weight and balance delays.
- WeatherDelay in minutes: Weather delay is caused by extreme or hazardous weather conditions that are forecasted or manifest themselves on point of departure, enroute, or on point of arrival.
- NASDelay in minutes: Delay that is within the control of the National Airspace System (NAS) may include: non-extreme weather conditions, airport operations, heavy traffic volume, air traffic control, etc.
- SecurityDelay in minutes: Security delay is caused by evacuation of a terminal or concourse, re-boarding of aircraft because of security breach, inoperative screening equipment and/or long lines in excess of 29 minutes at screening areas.
- LateAircraftDelay in minutes: Arrival delay at an airport due to the late arrival of the same aircraft at a previous airport. The ripple effect of an earlier delay at downstream airports is referred to as delay propagation.

## Summary of Findings
 
> To conduct my analysis, I considered the causes of cancelled flights and delayed flights to try to understand how each variable behaves and also their correlation with the others. 
    Starting with delayed flights
    My exploration shows that most of the delayed flights were slightly delayed, taking into account that slightly delayed flights are flights that are delayed more than 15 minutes. I was curious about the main causes of flight delays, so I studied the delay variable to see their distribution. I noticed that their values were concentrated on the left side, which means that the majority of delays are short, and the longer delays, while unusual  are more time consuming.
    Regarding cancelled flights, the main reasons for flight cancellations are the carrier and weather, and there are almost no flights cancelled for safety reasons.
    In addition, I have observed that the cancelled flights may be related to the time of year. In fact, we have more cancelled flights in February, from May to June and finally in December. We also have more delays in departures in these periods which correspond mainly to spring, summer and winter.
    Finally, to see if the season  affects the delay of flights,particularly weather flight and diverted flights I decided to study the trend on the 10 most active airlines on the diverted flights and I noticed that the highest number of diverted is observed during summer when airlines are overwhelmed .

  
 

## Key Insights for Presentation
>My main goal is to share with the public some important information so that that they will be able to know some sligh condition for a flight to be cancelled or delays
>Based on the result of my exploration, I think it's worth looking into the problem of cancelled flights depending on the time of year.
>The main reason why these flights were cancelled
>Some specific information about the cancelled flights
>At what time of year our flight is most likely to be delayed.
