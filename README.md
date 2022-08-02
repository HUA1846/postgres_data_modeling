# Sparkify Data ETL Pipelines

## Objective:
- Create a postgres database with tables that are easy to query for song play analysis. Build ETL pipelines on songs and user activity JSON data collected on the music streaming app for the analysis team. 

## Analytics Goals:
    1. Understand what songs are our users listening to
    2. Understand what artists' song our users like
    3. Understand user behaviors in free and paid plans

## How to run the Python script?
   - Run create_tables.py to initialze the database and data schema
   - Run the etl.py file to insert all data from the ./data directory to the tables

## File explanations
1. sql_queries.py contains sql queries to create database, drop tables, create tables, insert records, and select songs
2. etl.ipynb demonstrated the process of data ETL with a small set of data

## Database Design
- The database follows star scehma design to make queries easier with simple JOINS.
- The database has one Fact table which has records of songs played by users.
- The database has four Dimension tables for users, songs, artists, and time to allow simple JOINs to the fact table for analysis.




