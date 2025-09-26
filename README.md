# Customer Segmentation Analysis Using Machine Learning

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AhmedEhab2022/Customer-Segmentation/blob/main/Customer_Segmentation.ipynb)

A comprehensive data science project that performs customer segmentation analysis on mall customer data using multiple clustering algorithms. This project helps businesses understand their customer base and develop targeted marketing strategies by identifying distinct customer groups based on purchasing behavior and demographics.

## Project Overview

This repository contains a complete customer segmentation workflow that analyzes mall customer data to identify meaningful customer segments. The analysis uses annual income and spending score as primary features to group customers into distinct segments for business intelligence purposes.

## Dataset

The project uses mall customer data (`Mall_Customers.csv`) containing:

- **Customer Demographics**: Age, Gender
- **Financial Information**: Annual Income (in thousands)
- **Behavioral Data**: Spending Score (1-100 scale)

The dataset contains 200 customer records with no missing values.

## Methodology

### Data Preprocessing

- Exploratory data analysis with comprehensive visualizations
- Data cleaning and validation (duplicate/missing value checks)
- Feature scaling using StandardScaler for distance-based algorithms
- Outlier detection and impact analysis

### Clustering Algorithms

1. **K-Means Clustering**

   - Optimal cluster number determination using silhouette analysis
   - Centroid visualization and interpretation
   - Comparison with/without outliers

2. **Hierarchical Clustering**

   - Ward linkage method implementation
   - Dendrogram visualization for cluster structure analysis

3. **DBSCAN (Density-Based Clustering)**
   - Noise point detection capabilities
   - Parameter tuning for optimal density-based grouping

## Key Findings

The analysis identifies **5 distinct customer segments**:

| Segment                 | Description                       | Age Group   | Income Level | Spending Level | Business Strategy                |
| ----------------------- | --------------------------------- | ----------- | ------------ | -------------- | -------------------------------- |
| **Premium Customers**   | Young, high-income, high-spending | Young       | High         | Very High      | Luxury & premium offerings       |
| **Trend Followers**     | Young, low-income, high-spending  | Very Young  | Low          | High           | Affordable luxury & fast fashion |
| **Balanced Customers**  | Moderate income/spending          | Middle-aged | Moderate     | Average        | Mainstream products              |
| **Conservative Savers** | High-income, low-spending         | Middle-aged | High         | Very Low       | Investment products              |
| **Budget-Conscious**    | Low-income, conservative spending | Older       | Low          | Low            | Value & essential products       |

## Requirements

```txt
pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
scipy
jupyter
```

## How to Run

### Option 1: Google Colab (Recommended)

1. Click the "Open in Colab" badge above
2. Upload the dataset to your Google Drive in the appropriate folder
3. Run all cells in sequence

### Option 2: Local Setup

1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open `Customer_Segmentation.ipynb` in Jupyter
4. Update the data path to point to your local dataset
5. Run all cells

## Technologies Used

- **Python Libraries**: pandas, numpy, matplotlib, seaborn, plotly
- **Machine Learning**: scikit-learn (KMeans, DBSCAN, StandardScaler)
- **Statistical Analysis**: scipy (hierarchical clustering)
- **Evaluation Metrics**: Silhouette analysis for cluster validation
- **Environment**: Jupyter Notebook

## Project Structure

```
customer-segmentation/
├── Customer_Segmentation.ipynb   # Main analysis notebook
├── Mall_Customers.csv            # Customer dataset
├── README.md                     # Project documentation
├── LICENSE                       # License information
├── requirements.txt              # Python dependencies
```

## Key Visualizations

The project includes comprehensive visualizations:

- **Scatter Plots**: Customer distribution by income vs spending score
- **Cluster Visualization**: K-means clusters with centroids
- **Dendrograms**: Hierarchical clustering structure
- **Distribution Plots**: Feature distributions and outlier analysis
- **Box Plots**: Outlier detection across different features

## Business Applications

- **Targeted Marketing**: Develop personalized campaigns for each segment
- **Product Strategy**: Tailor offerings to specific customer groups
- **Pricing Strategy**: Optimize pricing based on spending behaviors
- **Customer Retention**: Identify high-value customers for loyalty programs
- **Market Expansion**: Understand customer preferences for new market entry

## 🔍 Analysis Highlights

- **Optimal Clusters**: Determined using silhouette analysis (k=5)
- **Algorithm Comparison**: K-Means vs DBSCAN vs Hierarchical clustering
- **Outlier Impact**: Analysis shows minimal effect on clustering results
- **Statistical Validation**: Comprehensive cluster characterization with demographics

## Key Insights

1. **Premium segment** represents the highest value customers (young, high-income, high-spending)
2. **Conservative savers** have purchasing power but prefer investments over consumption
3. **Trend followers** show high spending despite lower income - opportunity for affordable luxury
4. **Balanced customers** form the stable mainstream market segment
5. **Budget-conscious** customers prioritize value and essential purchases

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Data Source

Dataset: [Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python) from Kaggle
