# Mall Customer Segmentation using K-Means Clustering

A machine learning project that segments mall customers into distinct groups based on their annual income and spending patterns using K-Means clustering algorithm.

## 📌 Overview

This project applies unsupervised learning to identify customer segments in a mall dataset. By clustering customers based on their purchasing behavior and income levels, businesses can tailor marketing strategies and product offerings to specific customer groups.

## 🎯 Key Insights

The analysis identifies **4 distinct customer segments**:

| Segment | Avg. Income | Avg. Spending | Profile |
|---------|------------|---------------|---------|
| **Cluster 1** | $48.3K | 56.5/100 | Mid-income, moderate spenders |
| **Cluster 2** | $86.5K | 82.1/100 | High-income, high spenders |
| **Cluster 3** | $87.0K | 18.6/100 | High-income, low spenders |
| **Cluster 4** | $26.3K | 20.9/100 | Low-income, low spenders |

## 📊 Dataset

- **Source**: Mall Customer dataset
- **Samples**: 200 customers
- **Features**:
  - `CustomerID`: Unique customer identifier
  - `Gender`: Customer gender (Male/Female)
  - `Age`: Customer age (18-70 years)
  - `Annual Income (k$)`: Annual income in thousands of dollars
  - `Spending Score (1-100)`: Spending behavior score

## 🛠️ Technologies & Libraries

- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **scikit-learn**: Machine learning algorithms (K-Means, DBSCAN)
- **matplotlib**: Data visualization
- **yellowbrick**: ML visualization toolkit (Elbow method)

## 🔍 Methodology

### 1. **Data Exploration**
   - Load and analyze customer demographics
   - Examine distribution of age, income, and spending scores
   - Visualize gender and age group distributions

### 2. **Feature Selection**
   - Select Annual Income and Spending Score as primary clustering features
   - These features best represent customer value and behavior

### 3. **Optimal Cluster Selection**
   - Applied **Elbow Method** using KElbowVisualizer
   - Determined optimal number of clusters = **4**

### 4. **K-Means Clustering**
   - Trained K-Means model with 4 clusters
   - Computed cluster centroids
   - Analyzed cluster characteristics

### 5. **Cluster Analysis**
   - Calculated mean income and spending score per cluster
   - Identified distinct customer personas
   - Visualized clusters with centroids

## 📈 Results & Visualizations

The notebook includes:
- **Gender distribution** pie chart
- **Age group distribution** bar chart
- **Income distribution** bar chart
- **Cluster scatter plot** with centroids showing spatial separation

## 🚀 Usage

### Running the Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/Devaaldo/mall-customer-segmentation-kmeans.git
   cd mall-customer-segmentation-kmeans
   ```

2. Install dependencies:
   ```bash
   pip install pandas matplotlib scikit-learn yellowbrick
   ```

3. Open and run the Jupyter notebook:
   ```bash
   jupyter notebook Clustering_Mall_Customer_Segmentation.ipynb
   ```

### Expected Output

- Data exploration with statistics and visualizations
- Elbow curve showing optimal cluster count
- 2D scatter plot of customer clusters
- Cluster characteristics summary

## 💡 Business Applications

This segmentation can be used for:
- **Targeted Marketing**: Customize campaigns for each segment
- **Product Strategy**: Develop products suited to segment preferences
- **Pricing Models**: Adjust pricing based on spending capacity
- **Customer Service**: Tailor service levels to segment value
- **Sales Forecasting**: Predict revenue by segment

## 📝 Files

- `Clustering_Mall_Customer_Segmentation.ipynb` - Main analysis notebook
- `data/Mall_Customers.csv` - Customer dataset
- `README.md` - This file

## 🎓 Learning Outcomes

This project demonstrates:
- Data preprocessing and exploratory data analysis (EDA)
- Unsupervised learning with K-Means clustering
- Elbow method for optimal parameter selection
- Cluster validation and interpretation
- Data visualization and insights communication

## 📌 Future Enhancements

- Implement DBSCAN for density-based clustering comparison
- Add silhouette score analysis for cluster quality evaluation
- Include 3D visualization with age as additional feature
- Develop interactive dashboard with Streamlit/Plotly
- Test alternative features (e.g., age + income, age + spending)

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

**Devaaldo**

---

**Note**: This is a demonstration of customer segmentation techniques suitable for portfolio and learning purposes.
