# SantanderRecommendation
Predicting Security account holders for Santander customers

Consumer level data contains a plethora of information that provides insight into customer behavior. Whether these are more general macro-level demographic characteristics or micro-level transaction data, the wide spectrum of existing features can easily be used to engineer new features either through brute force EDA, or more creative unsupervised learning algorithms such as clustering into interpretable personas that may themselves be used as categorical features in a supervised model. This is critical insight for marketing data scientists and product managers to recommend the appropriate strategy to target potential customers.

Throughout the series of 4 notebooks, this project seeks to predict whether a customer will open/have a new Securities account by the end of May 2016 (the last month in time series axis if of the dataset). The original data source and base version of this problem was posed by Santander Bank here, where you may also find the data dictionary.

You may find the raw data downloaded as train_ver2.csv.

## Notebook 1 of 4 - Data Cleaning & Wrangling

This notebook achieves the goal of wrangling the initial raw dataset to produce a cleaned dataset for use in subsequent EDA and modeling pipelines. S3 is used as the source/destination for the raw dataset and the processed dataset and spark is utilized to carry out the data wrangling process.

## Notebook 2 of 4 - Exploratory Data Analysis

This notebook seeks to explore the data first at a high level, followed by deep dives accordingly based on standout patterns or peculiarities revealed by the data. The intention is to provide a firm basis for the intuition behind Feature Engineering, which comes immediately afterwards.


