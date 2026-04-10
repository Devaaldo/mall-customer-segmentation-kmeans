# Customer Segmentation with K-Means Clustering

Unsupervised machine learning project to segment mall customers based on annual income and spending behavior, with both 2D and 3D clustering approaches.

## Dataset

200 mall customers with features: Age, Gender, Annual Income (k$), Spending Score (1-100).

Source: [Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

## Methodology

1. Exploratory Data Analysis — distribution, correlation, demographic breakdown
2. Feature scaling with StandardScaler
3. Optimal cluster selection via Elbow Method and Silhouette Score
4. 2D clustering: Annual Income + Spending Score (k=5, Silhouette: 0.5547)
5. 3D clustering: Age + Annual Income + Spending Score
6. Segment profiling with business recommendations

## Results

Five customer segments identified:

| Segment | Count | Avg Income | Avg Spending |
|---|---|---|---|
| Target Customers | 39 | $86.5k | 82.1 |
| Conservative Rich | 35 | $88.2k | 17.1 |
| Standard Customers | 81 | $55.3k | 49.5 |
| Careless Spenders | 22 | $25.7k | 79.4 |
| Careful Spenders | 23 | $26.3k | 20.9 |

## Project Structure

```
customer-segmentation-kmeans/
├── data/
│   └── Mall_Customers.csv
├── notebook/
│   └── customer_segmentation.ipynb
├── .gitignore
├── README.md
└── requirements.txt
```

## Setup

```bash
git clone https://github.com/Devaaldo/customer-segmentation-kmeans.git
cd customer-segmentation-kmeans
pip install -r requirements.txt
jupyter notebook notebook/customer_segmentation.ipynb
```

## Tech Stack

- Python 3.x
- pandas, numpy, matplotlib, seaborn
- scikit-learn, yellowbrick
