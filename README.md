# Change Point detection in Time series Sensor data using R

This developer journey is intended for anyone who wants to experiment, learn, enhance and implement a new method for detecting Change point in Sensor data. Sensors mounted on devices like IoT devices, Automated manufacturing like Robot arms, Process monitoring and Control equipment etc., collect and transmit data on a continuous basis which is Time stamped. 
This journey takes you through end to end flow of steps in collating statistics on such Time series data and identify if a Change point has occurred. Core building blocks would include computing Statistical parameters from the Time series data, which compares a Previous dataset of a certain Time range in the past with the Current Series in a recent Time range. Statistical comparison between these two results in detection of any change points. R statistical software is used in this Journey with sample Sensor data loaded into the Data Science experience cloud.
All the intermediary steps are modularized and all code open sourced to enable developers to use / modify the modules / sub-modules as they see fit for their specific application

When you have completed this journey, you will understand how to
1.Read Sensor data for a single sensor
2.Extract 2 Time series datasets one in the past and another in the present
3.Compress these datasets by translating them into a bunch of statistics that accurately describe the characteristics 
   of these datasets
4.Compare these statistics and quantify them 
5.Analyze these comparisons to detect any occurrence of Change points in the data between Previous data set and 
  Current data set
 
![alt text](http://url/to/img.png)



1.	User logs into Data Science -> R Studio and selects the Sensor Time series data files in csv format from the local folder
2.	The documents stored in the local folder, will be uploaded to the cloud on which further processing will be applied
3.	User configures the parameters in R code flow to read the relevant subset from the Sensor data file
4.	Data from the cloud will be read by R Studio in Data Science Experience.
5.	The user will further extract the 2 series of datasets to be compared
6.	R Studio will use open R libraries and Custom built function components to get the statistics computed
7.	User will generate visual comparison charts to aid visualizing any hints for changes in behavior of the sensor
8.	These Statistical metrics will be compared and the changes analyzed using the Custom functions written in R
9.	Based on the threshold deviation specified by the user, Custom R functions will then output if there is a Change point occurrence detected
10.	Due to the reusable nature of the components, innumerable combination of data sets can be quickly compared for change point occurrence

All components that support the above steps are reusable like
1.	Reading specific Time series data points from a csv file like Time stamp, Sensor ID, Sensor values
2.	Time stamp conversion functions, filtering data for specific sensor
3.	User configurable Time ranges for Splitting Time series data into 2 sets for comparison
4.	Computations of key statistics that statistically compresses these series for useful comparison
5.	Build a dictionary of statistics to consistently compare these data sets
6.	Based on threshold specified by User, detect if a Change point has occurred in the data



