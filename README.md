# Mall Customer Segmentation using K-Means Clustering

A machine learning project that segments mall customers into distinct groups based on annual income and spending patterns using K-Means clustering algorithm.

## Overview

This project applies unsupervised learning to identify customer segments in a mall dataset. By clustering customers based on purchasing behavior and income levels, businesses can tailor marketing strategies to specific customer groups.

## Dataset

- Samples: 200 customers
- Features: CustomerID, Gender, Age, Annual Income (k$), Spending Score (1-100)
- Source: Mall Customer dataset

## Methodology

1. Load and explore customer data
2. Select features: Annual Income and Spending Score
3. Determine optimal clusters using Elbow Method
4. Apply K-Means clustering with 4 clusters
5. Analyze and visualize cluster characteristics

## Results

Four distinct customer segments identified:

- Cluster 1: Mid-income, moderate spenders (Income: $48.3K, Score: 56.5)
- Cluster 2: High-income, high spenders (Income: $86.5K, Score: 82.1)
- Cluster 3: High-income, low spenders (Income: $87.0K, Score: 18.6)
- Cluster 4: Low-income, low spenders (Income: $26.3K, Score: 20.9)

## Technologies

- Python 3.x
- pandas, scikit-learn, matplotlib, yellowbrick

## Usage

1. Clone the repository
2. Install dependencies: `pip install pandas matplotlib scikit-learn yellowbrick`
3. Run the Jupyter notebook: `jupyter notebook Clustering_Mall_Customer_Segmentation.ipynb`

## Files

- `Clustering_Mall_Customer_Segmentation.ipynb` - Analysis notebook
- `data/Mall_Customers.csv` - Customer dataset
- `README.md` - This file

## Business Applications

- Targeted marketing campaigns for each segment
- Product strategy development based on segment preferences
- Pricing models adjusted to spending capacity
- Customer service customization by segment value
- Revenue forecasting by customer group
