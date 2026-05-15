# Zomato Data Analysis Using Python

# Project Overview

This project focuses on analyzing Zomato restaurant data using Python to discover meaningful business insights related to customer preferences, restaurant trends, online ordering behavior, ratings, and pricing patterns.

The analysis helps understand how restaurants perform based on customer engagement, ratings, restaurant types, and online delivery availability.


# Business Problems Solved

The project answers the following business questions:

- Do more restaurants provide online delivery compared to offline services?
- Which types of restaurants are most preferred by customers?
- What price range do couples generally prefer?
- Which restaurants receive the highest votes?
- How do ratings differ between online and offline ordering?
- What is the relationship between restaurant type and online ordering?


# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook


# Dataset Information

The dataset contains restaurant-related information such as:

- Restaurant Name
- Ratings
- Votes
- Online Order Availability
- Restaurant Category
- Approximate Cost for Two People

Dataset Format: CSV


# Project Workflow

1. Importing Required Libraries
2. Loading Dataset
3. Data Cleaning
4. Exploratory Data Analysis (EDA)
5. Data Visualization
6. Business Insight Generation


# Data Cleaning Steps

The following preprocessing steps were performed:

- Converted restaurant ratings into float values
- Removed unnecessary characters from rating column
- Checked missing/null values
- Verified dataset information and data types

Example:

python
def handleRate(value):
    value = str(value).split('/')
    value = value[0]
    return float(value)

dataframe['rate'] = dataframe['rate'].apply(handleRate)


# Exploratory Data Analysis

## 1. Restaurant Type Analysis

Analyzed the `listed_in(type)` column to identify the most common restaurant categories.

### Insight
Dining restaurants are the most common restaurant category.

## 2. Votes Analysis by Restaurant Type

Calculated total votes received by each restaurant category.

### Insight
Dining restaurants are preferred by a larger number of customers.

## 3. Online Order Availability

Analyzed restaurants accepting online orders versus offline services.

### Insight
Most restaurants do not provide online ordering services.

## 4. Ratings Distribution

Visualized restaurant rating distribution using histograms.

### Insight
Most restaurants received ratings between 3.5 and 4.


## 5. Approximate Cost for Couples

Analyzed the preferred spending range for couples.

### Insight
Most couples prefer restaurants with an approximate cost of ₹300.


## 6. Ratings Comparison: Online vs Offline Orders

Compared restaurant ratings based on online order availability.

### Insight
Restaurants offering online ordering generally receive better ratings.


## 7. Heatmap Analysis

Created a heatmap to analyze the relationship between restaurant type and online ordering.

### Insight
- Dining restaurants mostly prefer offline ordering
- Cafes mainly receive online orders


# Visualizations Included

The project includes the following visualizations:

- Count Plot
- Histogram
- Line Plot
- Box Plot
- Heatmap


# Key Business Insights

- Dining restaurants dominate the market.
- Online ordering is not adopted by most restaurants.
- Online-order restaurants tend to receive higher ratings.
- Mid-range pricing is preferred by most couples.
- Customer behavior differs across restaurant categories.


# Learning Outcomes

Through this project, I learned:

- Data Cleaning using Pandas
- Exploratory Data Analysis (EDA)
- Data Visualization using Matplotlib and Seaborn
- Business Insight Generation
- Customer Behavior Analysis
- Data Aggregation and Pivot Tables

# Future Improvements

Future enhancements for this project may include:

- Sentiment Analysis on Customer Reviews
- Restaurant Recommendation System
- Sales and Demand Forecasting
- Interactive Dashboard using Power BI or Tableau
- Location-Based Restaurant Analysis

# Project Structure

├── Zomato_Data_Analysis.ipynb
├── Zomato-data.csv
├── README.md
└── images

# Conclusion

This project demonstrates how Python-based data analysis can help businesses understand customer preferences, restaurant trends, pricing behavior, and online ordering patterns using real-world datasets.
The project also highlights the importance of exploratory data analysis and visualization in making data-driven business decisions.


