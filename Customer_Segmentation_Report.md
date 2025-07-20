
# Customer Segmentation Using Clustering

## Executive Summary

This project focuses on unsupervised customer segmentation using clustering algorithms. The goal is to divide customers into distinct groups based on similarities in demographics and purchasing behavior. Using clustering helps businesses tailor their products, marketing strategies, and services to better fit each customer segment.

## Dataset Overview

- **Source:** Kaggle - Customer Personality Analysis
- **Size:** ~2,200 customer records
- **Attributes:** Demographic data (Age, Income, Marital Status), behavioral traits (Spending on wines, fruits, meat, etc.), and enrollment dates.

## Objectives

- Identify natural groupings of customers based on behavior and lifestyle
- Improve business decision-making and customer engagement
- Use cluster insights to suggest data-driven marketing strategies

## Methodology

1. **Data Cleaning**
   - Dropped missing values in `Income`
   - Converted `Dt_Customer` to datetime
   - Encoded categorical variables using Label Encoding

2. **Feature Engineering**
   - Created derived metrics such as Total Spending
   - Standardized the data before clustering

3. **Dimensionality Reduction**
   - Applied PCA (Principal Component Analysis) for visualization
   - Retained key variance-contributing features

4. **Clustering Techniques**
   - **KMeans Clustering** with optimal `k` based on Elbow Method
   - **Agglomerative Hierarchical Clustering**
   - **DBSCAN** for noise/outlier detection

5. **Evaluation**
   - Used Silhouette Scores and PCA plots to evaluate clusters
   - Compared methods to validate clustering consistency

6. **Cluster Profiling**
   - Labeled clusters based on characteristics (e.g., High Spenders, Budget Families, Young Singles)
   - Business implications discussed for each segment

## Conclusion

The customer segmentation project enabled data-driven grouping of customers, which can enhance targeted marketing, loyalty programs, and personalized promotions. The clustering models revealed patterns that a business could use to increase engagement and retention.

## Future Improvements

- Add temporal data (e.g., purchase recency)
- Integrate web/app behavioral tracking
- Deploy clustering in a production environment for live segmentation

## References

- [Kaggle Dataset](https://www.kaggle.com/imakash3011/customer-personality-analysis)
- Scikit-learn Documentation
- Unsupervised Machine Learning Research Articles
