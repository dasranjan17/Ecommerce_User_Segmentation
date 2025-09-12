# E-commerce User Segmentation Project

## Overview
This project delivers a complete pipeline for e-commerce customer segmentation using user event data. The workflow covers data exploration, cleaning, feature engineering, clustering, and deriving actionable business insights to inform marketing strategies.

## Project Structure

| Notebook | Description |
|----------|-------------|
| `01_data_exploration_eda.ipynb` | Loads and explores raw dataset, visualizes missing values, and documents initial observations. |
| `02_data_cleaning.ipynb` | Handles missing values, removes duplicates, detects and removes outliers (IQR method), and validates data types. |
| `03_preprocessing_feature_engineering.ipynb` | Encodes categorical variables, scales numerical features, and engineers 32+ customer-level features (purchase frequency, browsing ratios, session metrics). |
| `04_clustering_ml.ipynb` | Applies K-Means clustering, determines optimal clusters using Elbow Method and Silhouette Score, and assigns cluster labels. |
| `05_cluster_analysis_insights.ipynb` | Profiles each cluster, visualizes key metrics, creates customer personas, and derives marketing strategies and business recommendations. |

## Key Features & Methods

- **Data Cleaning:** Imputation, outlier removal, duplicate handling, and type validation.  
- **Feature Engineering:** Combines purchase history, browsing behavior, session activity, and spending into detailed customer profiles.  
- **Clustering:** K-Means with statistical validation (Elbow Method and Silhouette Analysis). Final segmentation into **4 actionable groups**:  
  - Premium Customers  
  - Efficient Buyers  
  - Budget Browsers  
  - Category Explorers  
- **Business Insights:** Each segment is profiled for size, spending, engagement, and behavior patterns. Actionable strategies are suggested for targeted marketing.  
- **Exportable Outputs:** Cleaned datasets and cluster labels ready for CRM integration and marketing dashboards.  

## Tech Stack

- Python: `pandas`, `numpy`, `scikit-learn`  
- Jupyter Notebooks  
- Data Visualization: `Matplotlib`, `Seaborn`  
- Data Pipeline & Storage: Pickle  

## Results

- **4 distinct customer segments** identified and statistically validated (Silhouette Score ≈ 0.19)  
- **2,400+ unique customers** analyzed  
- **32 engineered behavioral features** for clustering  
- Actionable marketing and business strategies provided for each segment  

## Key Insights & Customer Segments

| Segment | % of Customers | Behavioral Summary | Suggested Actions |
|---------|----------------|------------------|-----------------|
| Premium Customers | 18.8% | High spend, frequent engagement | Focus on loyalty programs, premium offerings, and personalized campaigns |
| Efficient Buyers | 20.7% | Fast decision-making, high conversion | Optimize checkout flow, cross-sell complementary products |
| Budget Browsers | 29.1% | Price-sensitive, browse many categories | Highlight discounts, value deals, and promotions |
| Category Explorers | 31.3% | Engage with diverse products, exploratory browsing | Recommend curated bundles, cross-selling, and targeted suggestions |

## How to Run

1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd <repository-folder>

2. Set up Python Environment
    ```bash
    pip install -r requirements.txt

3. Run Notebooks in Order
- Open and execute notebooks sequentially:
    - 01_data_exploration_eda.ipynb
    - 02_data_cleaning.ipynb
    - 03_preprocessing_feature_engineering.ipynb
    - 04_clustering_ml.ipynb
    - 05_cluster_analysis_insights.ipynb

4. Explore Outputs
- Cluster labels and cleaned datasets can be used for CRM integration.
- Visualizations in notebooks provide insights into customer segments.