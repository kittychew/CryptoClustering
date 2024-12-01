# CryptoClustering
# Cryptocurrency Market Analysis using PCA & K-means Clustering

This project involves analyzing cryptocurrency market data using **Principal Component Analysis (PCA)** and **K-means clustering**. The goal was to explore and segment cryptocurrencies based on their price and market data, helping to identify patterns and groups that exhibit similar market behaviors. The analysis was done using Python, data visualization tools, and machine learning techniques.

## Project Overview

The goal of this project was to analyze cryptocurrency market data, reduce its dimensionality using **PCA**, and apply **K-means clustering** to group cryptocurrencies based on their market behaviors (such as price change percentages). This allows us to find patterns in the data and categorize similar cryptocurrencies into clusters.

Key steps in the analysis:
1. **Data Collection**: Cryptocurrency market data was sourced and cleaned.
2. **Data Scaling**: Features were scaled to ensure consistent contribution to the model.
3. **PCA**: The dimensionality of the data was reduced to 3 principal components.
4. **K-means Clustering**: The optimal number of clusters was identified using the elbow method, and K-means clustering was applied.
5. **Data Visualization**: Results were visualized using scatter plots to interpret and analyze the clusters.

## Skills & Technologies

- **Programming Languages**:
  - Python
  
- **Libraries & Tools**:
  - Pandas
  - NumPy
  - Scikit-learn
  - Matplotlib
  - hvPlot
  
- **Techniques**:
  - Principal Component Analysis (PCA)
  - K-means Clustering
  - Elbow Method
  - Data Visualization (Scatter Plots, Color Mapping)

## Data

The dataset used in this analysis is related to cryptocurrency market data. The features include:
- `coin_id`: Unique identifier for each cryptocurrency.
- `price_change_percentage_24h`: The percentage change in the cryptocurrency's price over the last 24 hours.
- `price_change_percentage_7d`: The percentage change in the cryptocurrency's price over the last 7 days.
- Other market data such as market capitalization and trading volume (not used in the clustering model).

## Steps in the Analysis

1. **Data Collection & Preparation**:
    - Collected cryptocurrency market data.
    - Cleaned and prepared the data for analysis, ensuring there were no missing values.
    
2. **Scaling the Data**:
    - Scaled the data to standardize features and ensure proper weighting for PCA and K-means clustering.
    
3. **Principal Component Analysis (PCA)**:
    - Reduced the dimensionality of the data to 3 principal components, which capture most of the variance in the data.
    
4. **K-means Clustering**:
    - Applied the elbow method to determine the optimal number of clusters (k).
    - Performed K-means clustering on the data to group cryptocurrencies into distinct clusters.

5. **Visualization**:
    - Used scatter plots to visualize the results of the clustering.
    - Plotted the relationship between the 24-hour and 7-day price change percentages, coloring the data points based on their cluster labels.

    ### Elbow Curve (Layered)
    
    Below is the layered elbow curve showing the inertia values for different k-values, which was used to determine the optimal number of clusters.
    
    ![Elbow Curve](./Images/OG_PGA_elbow.png)
    
    ### Clustering Results
    
    Below are the scatter plots showing the clustering results for the original data and PCA-reduced data side by side. These plots visualize how the cryptocurrencies are grouped based on the features.
    
    ![Original Data Clusters](./Images/OG_AND_PGA_scatter.png)


## Results

- **Elbow Method**: After applying the elbow method, the optimal number of clusters for the dataset was found to be **4**. This suggests that there are 4 distinct groups of cryptocurrencies with similar market behaviors.
- **Cluster Visualization**: The scatter plot based on the PCA components shows how cryptocurrencies are grouped together based on the clusters formed by K-means.
