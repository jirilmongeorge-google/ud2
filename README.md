# Project 2 - Purpose
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. 
The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

# Database schema design
The DB design is done based on the SQL query requirements.
Three tables were created and data was ingested to meet the requirements of below 3 queries:
1. Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4
2. Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

# ETL pipeline
The ETL piepline file does model the data by creating tables in Apache Cassandra to run queries. 
ETL pipeline also transfers data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables.

# Project Files
- *Project_1B_ Project_Template.ipynb* A notebook that contains the entire ETL pieline. 
