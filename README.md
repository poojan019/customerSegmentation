# Customer Segmentation Analysis

## Overview
This project performs customer segmentation analysis on retail transaction data using RFM (Recency, Frequency, Monetary Value) metrics and K-means clustering. The analysis identifies distinct customer groups to enable targeted marketing strategies.

## Features
- Data cleaning and preprocessing of retail transaction data
- Feature engineering using RFM metrics
- Outlier detection and handling
- K-means clustering with optimal cluster selection
- Visualization of customer segments

## Technical Stack
- Python 3.x
- Key Libraries:
  - pandas: Data manipulation and analysis
  - scikit-learn: Machine learning (K-means clustering)
  - matplotlib & seaborn: Data visualization
  - numpy: Numerical computations

## Data Processing
1. **Data Cleaning**
   - Removed invalid transactions
   - Handled missing customer IDs
   - Filtered out non-standard stock codes
   - Removed zero-price transactions

2. **Feature Engineering**
   - Calculated RFM metrics:
     - Recency: Days since last purchase
     - Frequency: Number of purchases
     - Monetary Value: Total spending

3. **Outlier Handling**
   - Identified outliers using IQR method
   - Separated outliers into special segments

## Customer Segments
### Main Clusters
1. **RETAIN** (Cluster 0)
   - High-value customers with regular purchases
   - Focus: Retention efforts and loyalty programs

2. **RE-ENGAGE** (Cluster 1)
   - Lower-value, infrequent buyers
   - Focus: Re-engagement campaigns

3. **NURTURE** (Cluster 2)
   - Recent but low-value customers
   - Focus: Relationship building

4. **REWARD** (Cluster 3)
   - High-value, frequent buyers
   - Focus: Loyalty rewards

### Outlier Segments
1. **PAMPER** (Monetary Outliers)
   - High spenders with infrequent purchases
   - Focus: Personalized luxury services

2. **UPSELL** (Frequency Outliers)
   - Frequent buyers with lower spending
   - Focus: Upselling opportunities

3. **DELIGHT** (Monetary & Frequency Outliers)
   - Top-tier customers
   - Focus: VIP treatment

## Visualization
The project includes various visualizations:
- 3D scatter plots of customer segments
- Distribution plots of RFM metrics
- Cluster analysis visualizations
- Segment size and characteristics comparison

## Usage
1. Load and preprocess the retail data
2. Run feature engineering to calculate RFM metrics
3. Perform clustering analysis
4. Visualize results
5. Apply business strategies based on segments

## Future Improvements
- Include additional customer attributes
- Implement time-series analysis
- Add predictive modeling for customer behavior
- Develop automated segmentation updates
