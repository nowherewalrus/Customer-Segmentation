# Customer Segmentation using K-Means Clustering

## 📊 Overview

This project implements a **customer segmentation analysis** using K-Means clustering algorithm to identify distinct customer groups based on demographic and behavioral data. The analysis helps businesses understand their customer base and develop targeted marketing strategies.

![Cluster Visualization](https://img.shields.io/badge/Clusters-5-blue) ![Python](https://img.shields.io/badge/Python-3.x-green) ![License](https://img.shields.io/badge/License-MIT-orange)

## 🎯 Features

- **Data Preprocessing**: Clean and prepare customer data for analysis
- **Optimal Cluster Detection**: Use Elbow Method to determine best number of clusters
- **K-Means Clustering**: Segment customers into distinct groups
- **Visualization**: 2D PCA plots for cluster visualization
- **Cluster Analysis**: Detailed statistics and interpretation for each segment
- **Model Evaluation**: Silhouette score calculation for quality assessment

## 📁 Dataset

The project uses a customer dataset with the following features:

| Feature | Description | Data Type |
|---------|-------------|-----------|
| CustomerID | Unique customer identifier | Integer |
| Gender | Customer gender (Male/Female) | Categorical |
| Age | Customer age | Integer |
| Annual Income (k$) | Annual income in thousands | Integer |
| Spending Score (1-100) | Spending behavior score | Integer |

## 🚀 Installation

### Prerequisites

- Python 3.6+
- pip (Python package installer)

### Required Libraries

Install the required packages using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## 📋 Project Structure

```
customer-segmentation/
│
├── Custim_Seg.ipynb     # Main Jupyter notebook
├── customer.csv                    # Dataset file
├── README.md                       # Project documentation
├── requirements.txt                # Python dependencies
│
├── images/                         # Generated visualizations
│   ├── elbow_method.png
│   ├── cluster_distribution.png
│   └── pca_visualization.png
│
└── outputs/                        # Analysis outputs
    └── segmented_customers.csv
```

## 💻 Usage

### 1. Clone the Repository

```bash
git clone https://github.com/nowherewalrus/Customer-Segmentation.git
cd Customer-Segmentation.git
```

### 2. Run the Analysis

Open the Jupyter notebook:

```bash
jupyter notebook customer_segmentation.ipynb
```

Or run as a Python script:

```bash
python customer_segmentation.py
```

### 3. Step-by-Step Process

The analysis follows these steps:

1. **Data Loading & Exploration**: Load customer data and examine structure
2. **Data Preprocessing**: Convert categorical variables and handle missing values
3. **Feature Selection**: Select relevant features for clustering
4. **Determine Optimal Clusters**: Use Elbow Method to find best K value
5. **Apply K-Means**: Segment customers into clusters
6. **Cluster Analysis**: Analyze characteristics of each segment
7. **Visualization**: Create PCA plots for cluster visualization
8. **Evaluation**: Calculate silhouette score for model validation
9. **Business Insights**: Generate actionable recommendations

## 📈 Results

### Cluster Summary

| Cluster | Size | Avg Age | Avg Income | Avg Spending Score | Profile Name |
|---------|------|---------|------------|-------------------|--------------|
| 0 | 46 customers | 45.2 | $26.3k | 20.9 | Conservative Shoppers |
| 1 | 39 customers | 32.7 | $86.5k | 82.1 | High-Value Customers |
| 2 | 37 customers | 40.3 | $87.4k | 18.2 | Wealthy Savers |
| 3 | 79 customers | 43.1 | $54.8k | 49.8 | Balanced Customers |
| 4 | 22 customers | 25.3 | $25.7k | 79.4 | Young Spenders |

### Model Performance

- **Silhouette Score**: 0.44 (Reasonable cluster structure)
- **Optimal Clusters**: 5 (determined by Elbow Method)
- **Total Customers**: 200

## 📊 Visualizations

### 1. Elbow Method Plot
![Elbow Method](images/elbow_method.png)

### 2. Cluster Visualization (PCA)
![PCA Visualization](images/pca_visualization.png)

### 3. Cluster Distribution
![Cluster Distribution](images/cluster_distribution.png)

## 🎯 Business Applications

### Marketing Strategies for Each Segment:

1. **Cluster 0 (Conservative Shoppers)**
   - Target with value-based messaging
   - Promote budget-friendly products
   - Focus on necessity-based marketing

2. **Cluster 1 (High-Value Customers)**
   - Premium product recommendations
   - VIP loyalty programs
   - Personalized shopping experiences

3. **Cluster 2 (Wealthy Savers)**
   - Investment-focused products
   - Long-term value propositions
   - Quality and durability messaging

4. **Cluster 3 (Balanced Customers)**
   - General promotions
   - Bundle offers
   - Seasonal campaigns

5. **Cluster 4 (Young Spenders)**
   - Trendy product recommendations
   - Social media campaigns
   - Flexible payment options

## 🔧 Technical Details

### Algorithm: K-Means Clustering
- **Initialization**: k-means++
- **Number of runs**: 12
- **Random State**: 42 (for reproducibility)
- **Distance Metric**: Euclidean distance

### Preprocessing
- Gender encoding: Male → 1, Female → 0
- No missing values handling needed
- No feature scaling applied (features already in similar ranges)

### Evaluation Metrics
- **Silhouette Score**: 0.44
- **Within-Cluster Sum of Squares (WCSS)**: Used for Elbow Method

## 🛠️ Dependencies

```txt
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
scikit-learn>=0.24.0
jupyter>=1.0.0
```

## 📝 Future Improvements

1. **Feature Engineering**: Add derived features like income-to-age ratio
2. **Alternative Algorithms**: Test DBSCAN, Hierarchical Clustering
3. **Dynamic Clustering**: Implement real-time customer segmentation
4. **A/B Testing**: Validate cluster-based marketing strategies
5. **Dashboard**: Create interactive dashboard for business users

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🙏 Acknowledgments

- Dataset inspired by retail customer analysis
- scikit-learn documentation for clustering implementation
- Matplotlib and Seaborn for visualization capabilities

## 📧 Contact

For questions or feedback, please open an issue in the GitHub repository.

Email: pkhaghani916@gmail.com
Project Link: https://github.com/nowherewalrus/Customer-Segmentation.git

---

**Note**: This project is for educational and demonstration purposes. Real-world customer segmentation may require additional data and domain-specific considerations.

---
⭐ **If you find this project useful, please give it a star!** ⭐
