# SantanderRecommendation
Predicting Security account holders for Santander customers

Consumer level data contains a plethora of information that provides insight into customer behavior. Whether these are more general macro-level demographic characteristics or micro-level transaction data, the wide spectrum of existing features can easily be used to engineer new features either through brute force EDA, or more creative unsupervised learning algorithms such as clustering into interpretable personas that may themselves be used as categorical features in a supervised model. This is critical insight for marketing data scientists and product managers to recommend the appropriate strategy to target potential customers.

Throughout the series of 4 notebooks, this project seeks to predict whether a customer will open/have a new Securities account by the end of May 2016 (the last month in time series axis if of the dataset). The original data source and base version of this problem was posed by Santander Bank here, where you may also find the data dictionary.

You may find the raw data downloaded as train_ver2.csv.

## Notebook 1 of 4 - Data Cleaning & Wrangling
This notebook achieves the goal of wrangling the initial raw dataset to produce a cleaned dataset for use in subsequent EDA and modeling pipelines. S3 is used as the source/destination for the raw dataset and the processed dataset and spark is utilized to carry out the data wrangling process.

## Notebook 2 of 4 - Exploratory Data Analysis
This notebook seeks to explore the data first at a high level, followed by deep dives accordingly based on standout patterns or peculiarities revealed by the data. The intention is to provide a firm basis for the intuition behind Feature Engineering, which comes immediately afterwards.

## Notebook 3 of 4 - Feature Engineering and Modeling Part 1 (Unsupervised Learning)
In this notebook, the wrangled and imputed data is taken and used to create additional features required for modeling. Additionally, some of the existent features are also tweaked according to the modeling needs.
In the second part of this notebook, unsupervised modeling approaches are tried on the data to see if any useful patterns/findings can be extracted to use as further features in supervised learning.

## Notebook 4 of 4 - Modeling (Part II): Supervised Learning
This is the final notebook that takes all our engineered features (including those from unsupervised approaches) and lessons learned from EDA to construct supervised learning models to predict our final outcome of whether a customer will open or still choose to keep a securities account by month end of May 2016 based on all features under consideration. We explore both parametric and non-parametric models here, but start simple and add complexity as needed.
