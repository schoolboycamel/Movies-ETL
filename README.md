# OVERVIEW 
 Amazing Prime is partaking in  a Hackathon that will essentially create an automated pipeline that takes in new data from Wikipedia, Kaggle metadata and the MovieLens rating data. Preceding in transforming the data, and finally  loading the  data into an existing PostgreSQL database.
For this analysis, we used the following breakdown:

- write an ETL function to read three data files,
- extract and transform the Wikipedia data,
- extract and transform the Kaggle and rating data,
- load the data to a PostgreSQL Movie Database.

#MOVIESETL

-Data  extracted from Wikipeadia, Kaggle, and movie lens in JSON formats. Data extracted in this format because it is not clean data. 
-Data transformed into Pandas data frames.
-JSON file requires extra step – loading file first and then transforming into data frame.

#First step was to write ETL functions to read three data files
-The function takes the Wikipedia JSON, the Kaggle metadata and MovieLens csv files and creates three separate DataFrames.

#Second step consists in extracting and transforming the Wikipedia data
Data filtered out the TV shows, consolidated the redundant data, removed the duplicates and formatted the Wikipedia data.

#Third step is to extract and Transform the Kaggle and rating data
Data was out togetherm then removed the duplicates, formatted and grouped the data.
Lartly, the Kaggle and rating data were then merged with the Wikipedia movies DataFrame.

