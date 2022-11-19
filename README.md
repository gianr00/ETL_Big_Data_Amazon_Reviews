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

#### Dataset used for this Extract, Transform and Load (ETL):
https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Major_Appliances_v1_00.tsv.gz

https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Personal_Care_Appliances_v1_00.tsv.gz

https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Luggage_v1_00.tsv.gz

#### DATA COLUMNS:
- marketplace       - 2 letter country code of the marketplace where the review was written.
- customer_id       - Random identifier that can be used to aggregate reviews written by a single author.
- review_id         - The unique ID of the review.
- product_id        - The unique Product ID the review pertains to. In the multilingual dataset the reviews
- for the same product in different countries can be grouped by the same product_id.
- product_parent    - Random identifier that can be used to aggregate reviews for the same product.
- product_title     - Title of the product.
- product_category  - Broad product category that can be used to group reviews 
- (also used to group the dataset into coherent parts).
- star_rating       - The 1-5 star rating of the review.
- helpful_votes     - Number of helpful votes.
- total_votes       - Number of total votes the review received.
- vine              - Review was written as part of the Vine program.
- verified_purchase - The review is on a verified purchase.
- review_headline   - The title of the review.
- review_body       - The review text.
- review_date       - The date the review was written.

#### DATA FORMAT
- Tab ('\t') separated text file, without quote or escape characters.
- First line in each file is header; 1 line corresponds to 1 record.

