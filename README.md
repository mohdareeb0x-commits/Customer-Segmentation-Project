# Customer Segmentation Project

A machine learning project that performs customer segmentation analysis using K-Means clustering on mall customer data.

## Overview

This project segments customers into distinct groups based on their demographic and spending characteristics. The analysis helps identify different customer profiles for targeted marketing strategies and business decision-making.

## Dataset

- **File**: `Mall_Customers.csv`
- **Features**:
  - **CustomerID**: Unique identifier for each customer
  - **Age**: Age of the customer
  - **Genre**: Gender of the customer (Male/Female)
  - **Annual Income (k$)**: Annual income in thousands of dollars
  - **Spending Score (1-100)**: Score assigned based on customer behavior and spending patterns

## Methodology

### Data Preprocessing
1. **Encoding**: Gender labels are encoded using LabelEncoder
2. **Scaling**: All features (Age, Annual Income, Spending Score, Genre) are standardized using StandardScaler for uniform feature importance

### Clustering
- **Algorithm**: K-Means Clustering
- **Number of Clusters**: 5
- **Evaluation Metric**: Silhouette Score

### Visualization
- **2D Scatter Plot**: Annual Income vs Spending Score to visualize customer segments
- **PCA Visualization**: Principal Component Analysis for dimensionality reduction and visual interpretation

## Customer Segments

The analysis identifies five customer segments:

| Cluster | Segment Name | Characteristics |
|---------|--------------|-----------------|
| 0 | Premium Customers | High Income, High Spending |
| 1 | Upsell Opportunity Customers | High Income, Low Spending |
| 2 | Promotion Sensitive Customers | Low Income, High Spending |
| 3 | Budget-Conscious Customers | Low Income, Low Spending |
| 4 | Average Customers | Moderate Income and Spending |

## Requirements

- Python 3.x
- pandas
- scikit-learn
- matplotlib

## Installation

Install required packages:
```bash
pip install pandas scikit-learn matplotlib
```

## Usage

Run the Jupyter notebook to execute the analysis:
```bash
jupyter notebook customer_segmentation.ipynb
```

The notebook will:
1. Load and preprocess the customer data
2. Apply K-Means clustering
3. Generate visualizations
4. Calculate the Silhouette Score
5. Display cluster profiles and interpretations

## Output

The analysis generates:
- Customer cluster assignments
- Silhouette Score (model quality metric)
- Mean profile statistics for each cluster
- 2D scatter plots showing cluster distribution
- PCA-based visualization for better interpretation

## Key Insights

- The segmentation reveals clear patterns in customer spending behavior relative to income levels
- Different segments can be targeted with different marketing strategies
- PCA visualization helps understand segment separation in reduced dimensions

## Author

[Your Name/Project Info]

## Date

December 28, 2025
