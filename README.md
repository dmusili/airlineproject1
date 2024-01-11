The primary goal of this project is to comprehensively analyze and understand the factors contributing to airline flight delays, with a focus on identifying patterns and root causes.

By leveraging extensive data and advanced analytics, our aim is to provide insights that can be utilized by airlines, regulatory bodies, and industry stakeholders to improve overall operational efficiency and passenger satisfaction.

Source Files
1. Airlines.csv: IATA airline codes and names
2. Airports.csv: IATA airport codes and names
3. Flights.csv: Contains a list of flights by each airline, departure and destination airports, and information on whether the flight was on time or delayed. If the flight was delayed, it also lists the reason for the delay

The data used in this project was obtained from the U.S. Department of Transportation’s Bureau of Transportation Statistics. The U.S. Department of Transportation's (DOT) Bureau of Transportation Statistics tracks the on-time performance of domestic flights operated by large air carriers. This summary information on the number of on-time, delayed, canceled, and diverted flights is published in DOT's monthly Air Travel Consumer Report and in this dataset of 2015 flight delays and cancellations.

Data Exploration Process;

In order to better explore the data, the flight data was divided into 3 distinct quarters
1) Quarter 1: January to April 2015
2) Quarter 2: May to August 2015
3) Quarter 3: September to December 2015
We narrowed down the data to only include the top 9 airlines with the most delays instead of all the 15 airlines in the dataset. The reason being that the other airlines (not included in our reporting) had minimal delays.

Also, in order for us to properly do our analysis, we had to define what a ‘flight delay’ meant.

Based on our research, we found that the United States Federal Aviation Administration (FAA) considers a flight to be delayed when it arrives (or departs) 15 minutes later than its scheduled time. 
As a result of our findings, we ended up adopting FAA’s definition of a flight delay for our analysis.

Data Clean up
This project’s primary dataset is the flights.csv file (which consists of the flight data). In order for our team to do the data analysis, the data had to be cleaned in the following ways
Rows containing null values for the arrival and departure times were removed
Some of the columns not needed for analyzing flight delays were removed.
The flight data was merged with data from the airlines.csv file. This enabled our reports to use the airline name and not the IATA airline code e.g. American Airlines instead of ‘AA’.
The flights were grouped by individual airlines and then summed up all the flight delays for both arrival and departure delays (for each airline) as well as cancelled and diverted flights.
The flights were also grouped by day of departure/arrival for all delayed flights.

