# Crime-Data-Analysis
# Database-Analytics-Programming-Final-Project
 A Final DAP Project for Gokhan,Joseph,Alper for Data Analytics Master Programme at NCI in 2023
 
# Our Scope/Problem Statement:
Our objective is to gain a comprehensive understanding of the types of crimes that occur in three distinct cities in the United States: New York, Chicago, and San Francisco. We aim to conduct a detailed analysis of the prevalence of various crimes and determine the most common days of the week and hours of the day during which these crimes are committed. 
 
# Data Source
We got our data source by calling the below APIs:

# NewYork Crime Data
https://data.cityofnewyork.us/api/views/qb7u-rbmr/rows.csv
# Chicago Crime Data
https://data.cityofchicago.org/api/views/ijzp-q8t2/rows.csv
# San Franscisco Crime Data
https://data.sfgov.org/api/views/wg3w-h783/rows.csv



# Steps We followed/ Our Work Flow:

# 1) Conversion of the CSV Data Source to JSON format: Since the requirement stated that we need to query a semi structured datasource (e.g JSON, XML), we had to open the CSV file for reading and converting the list of dictionaries to a JSON string. We then wrote the json string to a file.
# 2) Connecting to MongoDB database "MachineLearning" and inserting the imported Json files' contents into NewYorkCrime, ChicagoCrime, and SanFranciscoCrime collections for NewYork, Chicago, and San Franscisco Collections. 
# 3) Extraction of Files from MongoDB into a new CSV file Using the Luigi Library - Helps to show the status of scheduled tasks (whether successful or not).
# 4) Preprocess, and Transforms the imported data using python pandas library. 
# 5) Load the transformed dataframe into posstgreSQL server.
# 6) Save data into postgreSQL as we carryout out analysis
# 7) Draw Conclusions

Check the code section on stepwise on how we were able to achieve the above.

