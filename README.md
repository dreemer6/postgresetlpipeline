# Data Modeling with Postgres (Project 1)

A startup called Sparkify has been collecting data on songs and user activity on their new music streaming app. The analytics team needs to analyze the data, but the data is not optimized for running queries since it exists in JSON files in two directories. One directory contains logs on user activity on the app and the other contains metadata on the songs in their app.

The required task is to create a Postgres database with tables designed to optimize queries on song play analysis. A database schema and ETL pipeline needs to be created for this analysis. 

Five tables will be created for a star schema namely:
* songplays (fact table)
* user, song, artist, time (dimension tables)

## Running the Python Scripts
At the terminal: 
1. `python create_tables.py`
2. `python etl.py`

## Description of Files in the Project
In addition to the files in the data folder, there are six files in this project:
1. `test.ipynb` displays the first few rows of each table to inspect the database.
2. `create_tables.py` drops and creates the tables. This file must be run to reset the tables before each time running the ETL scripts.
3. `etl.ipynb` reads and processes a single file from song_data and log_data and loads the data into your tables. This notebook contains detailed instructions on the ETL process for each of the tables.
4. `etl.py` reads and processes files from song_data and log_data and loads them into the tables.
5. `sql_queries.py` contains all the sql queries, and is imported into the last three files above.
6. `README.md` provides discussion on the project.