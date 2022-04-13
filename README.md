# US-Accidents-2016-2021---EDA
In this Notebook we are going to perform various Exploratory Data Analysis as well as Data Visualization techniques to extract meaningful Insights from different features of the US Accidents Dataset.
US Accidents (2016-2021) - EDA

# Objective:
The main moto of this Project is accident prediction and prevention, car accidents hotspot locations, and various other insights based on the given features.
In this Notebook we are going to perform various Exploratory Data Analysis as well as Data Visualization techniques to extract meaningful Insights from different features of the US Accidents Dataset.
Questions: 1) Which city in US has reported the most number of accident cases?
2) Which 5 states reported the highest number of accident cases?
3) Which timezone reported the most number of accident cases?
4) Which street is most accident prone in US?
5) What time of the day are accidents most frequent in?
6) Which days of the week have the most accidents?
7) Which months have the most accidents?
8) What is the trend of accidents year over year (decreasing/increasing?)
9) Effects of road condition on the accident cases.
10) How did the weather conditions affected the cases?

# What is EDA?
Exploratory Data Analysis refers to the critical process of performing initial investigations on data so as to discover patterns,to spot anomalies,to test hypothesis and to check assumptions with the help of summary statistics and graphical representations. It is a good practice to understand the data first and try to gather as many insights from it. EDA is all about making sense of data in hand,before getting them dirty with it.

# Dataset Details:
This is a countrywide car accident dataset, which covers 49 states of the USA. The accident data are collected from February 2016 to Dec 2021, using multiple APIs that provide streaming traffic incident (or event) data. These APIs broadcast traffic data captured by a variety of entities, such as the US and state departments of transportation, law enforcement agencies, traffic cameras, and traffic sensors within the road-networks. Currently, there are about 2.8 million accident records in this dataset.

# Acknowledgement for Dataset:
Please cite the following papers if you use this dataset:
1) Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, and Rajiv Ramnath. “A Countrywide Traffic Accident Dataset.”, 2019.
2) Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, Radu Teodorescu, and Rajiv Ramnath. "Accident Risk Prediction based on Heterogeneous Sparse Data: New Dataset and Insights." In proceedings of the 27th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems, ACM, 2019.

# Dataset abbrevations:
ID - This is a unique identifier of the accident record.<br>
Severity - Shows the severity of the accident, a number between 1 and 4, where 1 indicates the least impact on traffic (i.e., short delay as a result of the accident) and 4 indicates a significant impact on traffic (i.e., long delay).<br>
Start_Time - Shows start time of the accident in local time zone.<br>
End_Time - Shows end time of the accident in local time zone. End time here refers to when the impact of accident on traffic flow.<br>
Start_Lat - Shows latitude in GPS coordinate of the start point.<br>
Start_Lng - Shows longitude in GPS coordinate of the start point.<br>
End_Lat - Shows latitude in GPS coordinate of the end point.<br>
End_Lng - Shows longitude in GPS coordinate of the end point.<br>
Distance(mi) - The length of the road extent affected by the accident.<br>
Description - Shows natural language description of the accident.<br>
Number - Shows the street number in address record.<br>
Street - Shows the street name in address record.<br>
Side - Shows the relative side of the street (Right/Left) in address record.<br>
City - Shows the city in address record.<br>
County - Shows the county in address record.<br>
State - Shows the state in address record.<br>
Zipcode - Shows the zipcode in address record.<br>
Country - Shows the country in address record.<br>
Timezone - Shows timezone based on the location of the accident (eastern, central, etc.).<br>
Airport_Code - Denotes an airport-based weather station which is the closest one to location of the accident.<br>
Weather_Timestamp - Shows the time-stamp of weather observation record (in local time).<br>
Temperature(F) - Shows the temperature (in Fahrenheit).<br>
Wind_Chill(F) - Shows the wind chill (in Fahrenheit).<br>
Humidity(%) - Shows the humidity (in percentage).<br>
Pressure(in) - Shows the air pressure (in inches).<br>
Visibility(mi) - Shows visibility (in miles).<br>
Wind_Direction - Shows wind direction.<br>
Wind_Speed(mph) - Shows wind speed (in miles per hour).<br>
Precipitation(in) - Shows precipitation amount in inches, if there is any.<br>
Weather_Condition - Shows the weather condition (rain, snow, thunderstorm, fog, etc.). <br>
Amenity - A POI annotation which indicates presence of amenity in a nearby location.<br>
Bump - A POI annotation which indicates presence of speed bump or hump in a nearby location.<br>
Crossing - A POI annotation which indicates presence of crossing in a nearby location.<br>
Give_Way - A POI annotation which indicates presence of give_way in a nearby location.<br>
Junction - A POI annotation which indicates presence of junction in a nearby location.<br>
No_Exit - A POI annotation which indicates presence of junction in a nearby location.<br>
Railway - A POI annotation which indicates presence of railway in a nearby location.<br>
Roundabout - A POI annotation which indicates presence of roundabout in a nearby location.<br>
Station - A POI annotation which indicates presence of station in a nearby location.<br>
Stop - A POI annotation which indicates presence of stop in a nearby location.<br>
Traffic_Calming - A POI annotation which indicates presence of traffic_calming in a nearby location.<br>
Traffic_Signal - A POI annotation which indicates presence of traffic_signal in a nearby location.<br>
Turning_Loop - A POI annotation which indicates presence of turning_loop in a nearby location.<br>
Sunrise_Sunset - Shows the period of day (i.e. day or night) based on sunrise/sunset.<br>
Civil_Twilight - Shows the period of day (i.e. day or night) based on civil twilight.<br>
Nautical_Twilight - Shows the period of day (i.e. day or night) based on nautical twilight.<br>
Astronomical_Twilight - Shows the period of day (i.e. day or night) based on astronomical twilight.<br>
