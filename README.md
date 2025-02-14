# AB_NYC_2019 Dataset Cleaning and Preprocessing
## Project Oerview
This project aims to clean and preprocess the AB_NYC_2019 dataset to ensure data consistency, accuracy, and readiness for further analysis. The goal is to enable reliable insights into Airbnb listings in New York City.
## Project Scope
This project is dedicated to the thorough cleaning and preprocessing of the AB_NYC_2019 dataset, which contains valuable information about New York City’s rental market. Key tasks include:
-	Identifying and addressing missing values to ensure data completeness.
-	Detecting and resolving duplicate entries to maintain data integrity.
-	Detecting and handling outliers to prevent skewed analysis.
-	Converting data types to ensure compatibility for analysis.
-	Rectifying inconsistencies within the data to enhance reliability.
## Out of Scope
-	Exploratory Data Analysis (EDA) beyond cleaning.
-	Feature engineering and model building.
## Dataset Description

-	File Name: AB_NYC_2019.ipynb
-	Dataset Source: https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data
-	Size: 48,895 rows × 16 columns
-	Key Attributes

| Column Name | Description |
|-------------|-------------|
| Id |Unique identifier for each listing |
| name	| Title or name of the Airbnb listing |
| host_id	| Unique identifier for the host |
| host_name |	Name of the host |
| neighbourhood_group |	The borough where the listing is located (e.g., Manhattan, Brooklyn) |
| neighbourhood	| Specific neighborhood within the borough |
| Latitude |	Latitude coordinate of the listing location |
| longitude |	Longitude coordinate of the listing location |
| room_type	| Type of rental (Entire home/apartment, Private room, Shared room) |
| Price |	Price per night in USD |
| minimum_nights |	Minimum number of nights required to book |
| number_of_reviews |	Total number of reviews for the listing |
| last_review |	Date of the most recent review |
| reviews_per_month |	Average number of reviews per month |
| calculated_host_listings_count |	Number of listings owned by the host |
| availability_365 |	Number of days the listing is available per year (0-365) |
## Methodology
1. Data Loading and Initial Inspection
- Step 1: Import pandas library
- Step 2. View the top Five rows of the dataset
- Step 3: Descriptive analysis
2. Handling Missing Values
- Step 1: Identifying Columns with Missing Values
- Step 2: Handling Missing Values
- Step 3: Verifying Missing Value Handling
3. Handling Duplicates:
  No duplicate values were found.
  
4. Handling Outliers (Winsorization Method)
- 4.1 Price Column
- 4.2 Minimum Nights Column
- 4.3 Number of Reviews Column
- 4.4 Reviews Per Month Column
- 4.5 Comparison of Statistics before and after cleaning
  
Summary of Data Cleaning Process
|Step	| Action	| Outcome|
|-----|---------|--------|
|Missing Values |	name, host_name, last_review, reviews_per_month fixed	| No missing values left |
| Duplicates	| Checked for duplicates |	None found |
| Outliers (Winsorization)	| Capped extreme values in price, minimum_nights, number_of_reviews, reviews_per_month |	Balanced dataset |


