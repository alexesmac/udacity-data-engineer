## Sparkify ETL

##### Business purpose

The purpose of the sparkify database is to keep track of user data on the music application. This database
will allow data analysts to run analytical queries on song information, user information, and usage 
statistics. This database will faciliate the Sparkify company in making business decisions over rates, 
music retention, and user membership.

###### Technical Specification

The sparkifydb was created through an ETL pipeline written in python. The ETL is initiated by 
create_tables.py where the tables songplays, songs, users, artists, and time are created on the sparkifydb.
Once created etl.py can be ran to load the sparkify datasets from the data folder. These csv files are 
loaded into pandas dataframes which are then processed and filtered before the data is inserted into the
appropriate tables on the sparkifydb. 

The sparkifydb has data stored in the 3rd normal form in songs, users, artists, time, and songplays 
tables. Using the 3rd normal form as part of the schema design eliminates duplicates and allows analysts 
to run complex reports and queries for better user statistics. 
