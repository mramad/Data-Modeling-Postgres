# Data-Modeling-Postgres
Relational modeling with Postgres

This Project Analyzes the data for a startup company called "Sparkify". Specifically it processes data that the company have collected for songs and User Activity.

For this purpose, this project does the following:

- Model the data for songs and user activity using relational modeling.
- Uses Postgres database to host the data models.
- Dimensions are created to represent the metadata (songs,artists,Users and Time)
- Single Fact table (songplays) is created to insert the user activity data
- Referental integrity constraints are added where applicable
- Uses python to build ETL pipelines that reads JSON files that represents the songs metadata   (Song data) and User activity data (Log data) recorded     and inserts the data into the relational models.

The Project has three files detailed as the following:

create_tables.py: This file creates a database named "Sparkify" , drop the relational tables if they exist , and then create fresh ones.

etl.py: reads and processes files from song_data and log_data and loads them into the created tables. 

sql_queries.py: has the sql queries to drop,create and query database tables.

Project Run:

In order to run the project, please follow the below sequence.

1- Run create_tables.py, this should drop any existent "Sparkifydb" and create new one and then create necessary tables along with their referential integrity.

2- Run etl.py, this should scan the song and log data directories, extract the json files stored, transform data into required structures/formats and then load it into thier respective tables.


