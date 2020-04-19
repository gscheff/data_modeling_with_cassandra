## Description: Data Modeling with Cassandra

A startup called Sparkify wants to analyze the data they've been collecting on
songs and user activity on their new music streaming app. The analysis team is
particularly interested in understanding what songs users are listening to.
Currently, there is no easy way to query the data to generate the results,
since the data reside in a directory of CSV files on user activity on the app.

They'd like a data engineer to create an Apache Cassandra database which can
create queries on song play data to answer the questions, and wish to bring you
on the project. Your role is to create a database for this analysis. You'll be
able to test your database by running queries given to you by the analytics
team from Sparkify to create the results.


## Project Overview

In this project, we use data modeling with Apache Cassandra and complete an ETL
pipeline using Python.  We will need to model the data by creating tables in
Apache Cassandra to run queries. We already have part of the ETL pipeline that
transfers data from a set of CSV files within a directory to create a
streamlined CSV file to model and insert data into Apache Cassandra tables.


## Dataset

For this project, we'll be working with one dataset: event_data. The directory
of CSV files partitioned by date. Here are examples of filepaths to two files
in the dataset:

```bash
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
```

## Project Steps

### Modeling the NoSQL database or Apache Cassandra database

  1. Design tables to answer the queries outlined in the project

  2. Write Apache Cassandra CREATE KEYSPACE and SET KEYSPACE statements

  3. Develop the CREATE statement for each of the tables to address each
     question

  4. Load the data with INSERT statement for each of the tables

  5. Include IF NOT EXISTS clauses in the CREATE statements to create tables
     only if the tables do not already exist. We recommend you also include
     DROP TABLE statement for each table, this way you can run drop and create
     tables whenever you want to reset your database and test your ETL pipeline

  6. Test by running the proper select statements with the correct WHERE clause


### Build ETL Pipeline

  1. Implement the logic in section Part I of the notebook template to iterate
     through each event file in event_data to process and create a new CSV file
     in Python

  2. Make necessary edits to Part II of the notebook template to include Apache
     Cassandra CREATE and INSERT statements to load processed records into
     relevant tables in the data model

  3. Test by running SELECT statements after running the queries on the
     database


