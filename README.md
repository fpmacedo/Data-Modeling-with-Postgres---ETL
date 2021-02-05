# Project: Data Modeling with Postgres

## Objective

This project has the purpose to show the concepts of Data Modeling in a relational database. The main objective is write an ETL pipeline
where we can extract data from JSON files and save this data in a Postgres database.

## Structure

|_ Data
|    |_ log_data (Log files showing what listeners are listening to)
|    |_ song_data (Files with musics data)
|
|
|_ create_tables.py (The script responsable for the criation of the tables in Postgres DB)
|
|
|_ sql_querys.py (Where are writed the querys used in create_tables.py to create tables, insert and read data)
|
|
|_ etl.ipynb (Jupyter notebook used to build the process of ETL)
|
|
|_ etl.py (The script to execute the ETL pipeline process)
|
|
|_ test.ipynb (Jupyter notebook used to test the ETL process)

## Running 

1 - First the command bellow should be executed to create the tables in the postgres database:
    
        ```run create_tables.py```
        
2 - Now we have to execute the ETL script contained in the file etl.py:

        ```run etl.py```
        
3 - After finished the process of ETL we can test if everything is ok just running the commands in the etl.ipynb.