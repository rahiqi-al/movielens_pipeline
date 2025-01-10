# MovieLens Data Pipeline

This is a group project created by **Anass**, **Ali**,  **Sliman** and **rabii**. It focuses on processing and analyzing data from the MovieLens dataset and loading it into a SQL Server database using an ETL process. The project also includes creating visualizations with Power BI.

## Table of Contents
1. [Overview](#overview)
2. [Data Sources](#data-sources)
3. [Data Pipeline Workflow](#data-pipeline-workflow)
5. [Usage](#usage)
6. [Optimization](#optimization)



## Overview
This project processes the MovieLens dataset by cleaning and transforming the data, loading it into a SQL Server database, and generating reports and visualizations. 

## Data Sources
The dataset contains the following files:
- **movies.csv**: Information about movies.
- **ratings.csv**: User ratings for movies.
- **users.csv**: Information about users.
- **tags.csv**: User-generated tags for movies.

## Data Pipeline Workflow
The pipeline is divided into four main sub-jobs:

1. **DimDate:** Generates a date dimension table.
2. **DimUser:** Cleans and loads user data.
3. **DimMovie:** Cleans and loads movie data.
4. **FactRatings:** Cleans and loads ratings data with lookups to the dimension tables.


## Usage
1. Run the ETL job to clean, transform, and load the data into SQL Server.
2. Use Power BI to visualize the data and create reports like top-rated movies, rating distributions, and genre popularity.

## Optimization
The following index optimizations are suggested for SQL Server:

1. **Clustered Index** on primary keys in the dimension tables.
2. **Non-clustered Index** on business keys such as UserID, MovieID, and Rating.
3. **Columnstore Index** for large fact tables to speed up analytical queries.
4. **Maintenance Tasks** such as rebuilding/reorganizing indexes and updating statistics.

## Acknowledgements
This project was completed as a group effort by Annas, Ali, rabii, and Sliman. Special thanks to everyone who contributed their time and expertise to make this project a success!

Feel free to reach out if you have any questions or feedback.

Thank you for visiting!

