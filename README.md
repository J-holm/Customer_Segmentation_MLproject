# Customer Segmentation with RFM Analysis and K-means Clustering

This project demonstrates customer segmentation using Recency, Frequency, Monetary (RFM) analysis and K-means clustering. It is crucial for businesses to understand their customer base to enhance marketing efficiency, customer engagement, and ultimately, drive more sales.

## Objective

- Analyze customer data to understand customer behavior.
- Segment customers based on recency, frequency, and monetary value of purchases.
- Develop targeted marketing strategies for each segment.

## Data Preparation

Data is loaded from the `online_retail_II.xlsx` file. It is cleaned by removing cancellations and null customer IDs. A new column `TotalPrice` is added, which is the product of `Quantity` and `Price`.

## RFM Analysis

RFM Analysis is used to calculate:
- Recency: Number of days since the last purchase.
- Frequency: Number of transactions.
- Monetary: Total amount of transactions.

This step involves grouping the data by Customer ID and calculating the Recency, Frequency, and Monetary value for each customer.

## K-means Clustering

K-means clustering is used to segment customers into groups based on their RFM values.
- Feature scaling is performed to normalize the RFM values.
- The Elbow Method is used to determine the optimal number of clusters.
- The K-means model is fit with the optimal number of clusters, and the clusters are assigned back to each customer.

## Interpretation and Strategy Development

The final step involves interpreting the clusters by analyzing the average RFM values of each cluster. Based on the characteristics, different marketing strategies are suggested for each segment. For example:
- High-value active customers might be targeted with exclusive deals and loyalty programs.
- Churning high-value customers might be re-engaged with personalized offers.

## Visualizations

Visualizations are employed to better understand and present the clusters:
- A line chart to find the optimal number of clusters using the Elbow Method.
- A scatter plot to visualize the clusters based on Recency and Monetary value.

## Requirements

- Python 3.x
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn


## Dataset Source

The dataset used in this project is the [Online Retail II Data Set](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II) from the UCI Machine Learning Repository.
