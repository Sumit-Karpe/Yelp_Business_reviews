# Yelp_Business_reviews
Analyzing Yelp businesses and reviews using Snowflake, AWS S3, SQL, and Sentiment Analysis

[FINAL REPORT](https://github.com/Sumit-Karpe/Yelp_Business_reviews/blob/main/Yelp%20Reviews%20Report.pdf)
Project Overview
This project utilizes the Yelp Open Dataset—a rich resource containing real-world data on businesses, reviews, check-ins, and attributes. The primary objective was to gain insights into business performance, user interactions, review sentiments, and popular categories.

Technologies Used
AWS S3 for storing and managing dataset partitions.
Snowflake as the cloud data warehouse for efficient querying and analysis.
SQL for data manipulation and exploratory analysis.
Python with TextBlob for sentiment analysis.



Dataset Information
The Yelp Open Dataset includes JSON files covering:
Business information (categories, locations, ratings)
User reviews (ratings, texts, timestamps)
Attributes (hours, parking, ambience, etc.)


Dataset size: ~8.65 GB uncompressed (business and review JSON files).

Project Workflow
Data Acquisition & Preparation
Downloaded dataset from Yelp.
Partitioned large dataset into 10 equal segments.
Uploaded partitions to an AWS S3 bucket.
Data Storage and Integration
Created and configured Snowflake database.
Connected AWS S3 to Snowflake for seamless data ingestion.
Data Processing
Created Snowflake tables (yelp_businesses, yelp_reviews) using SQL.
Loaded data from JSON format into structured tables.
Sentiment Analysis


Built a Python-based sentiment analyzer using TextBlob.
Classified reviews into Positive, Neutral, and Negative categories.
Exploratory Analysis
Conducted SQL-based exploratory analysis to uncover meaningful insights.



Key Queries and Insights Explored
Number of businesses per category.
Most active reviewers on Yelp.
Popular categories based on user reviews.
Peak months for reviews.
Cities with the most business reviews.
Sentiment analysis on reviews (identifying top positively reviewed businesses).

Usage Instructions
Clone this repository.
Set up AWS S3 bucket with dataset partitions.
Configure Snowflake with appropriate credentials.
Run SQL scripts provided to replicate tables and insights.
Deploy sentiment analysis code using Python and Snowflake’s external function feature.
