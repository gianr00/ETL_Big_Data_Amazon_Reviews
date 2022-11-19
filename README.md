# ETL (Extract, Transform and Load) of Big Data using Amazon Reviews dataset

Author: Rosie Gianan, gianr00@gmail.com

Build With: Python, Pandas,  AWS S3 and RDS, PySpark, Postgres, jupyter notebook 

## Objective:

Extract, Transform and Load the Amazon reviews data from AWS S3. 

Note: Many of Amazon's shoppers depend on product reviews to make a purchase. Amazon makes these [Reviews Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
publicly available. They are quite large and can exceed the capacity of local machines. One dataset alone contains over 1.5 million rows; with over 40 datasets, data analysis can be very demanding on the average local computer. 

## Solution:

Create the ETL (Extract, Transform and Load) process using PySpark, Postgres, AWS S3 and AWS RDS.
-    Extract – Extract the datasets for analysis from AWS S3. Save the data into the dataframe.
-    Transform – Clean the data then format it to fit the Postgres table schema
-    Load – Load the clean and formatted data into AWS RDS Postgres database.


