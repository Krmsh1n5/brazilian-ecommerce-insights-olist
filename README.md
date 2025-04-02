# Brazilian E-Commerce Insights: Olist Dataset Analysis  

## Overview  
This project analyzes **100k+ orders** from Olist, Brazil's largest e-commerce marketplace, to identify trends in customer behavior, seller efficiency, and regional pricing strategies. Leveraging Python’s data science stack, the analysis provides actionable recommendations to improve operational efficiency and customer retention.

**Dataset**: [Kaggle Link](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)  
**Notebook**: [sales-and-logistics-insights.ipynb](sales-and-logistics-insights.ipynb)  

## Key Skills Demonstrated
- **Data Preprocessing**: Handling missing values, outliers, anomalies, and geolocation validation.
- **Statistical Analysis**: Hypothesis testing (Kruskal-Wallis, Spearman), correlation analysis.
- **Visualization**: Interactive maps (Plotly), regression plots (Seaborn), and application of Dimensionality reduction using PCA for better visualization of customer segmentation

## Tools & Libraries
 - **Python**: Pandas, NumPy

 - **Visualization**: Matplotlib, Seaborn, Plotly

 - **Statistics**: SciPy, Scikit-learn

## Analysis Insights

### Statistical Findings:
During the analysis of the Brazilian e-commerce dataset, several key insights were uncovered through statistical methods and exploratory data analysis:

1. **Regional Pricing Bias**:
   - A Kruskal-Wallis test revealed statistically significant differences in product pricing across regions (`SP`, `RJ`, `MG`).
   - For example, median prices for the `health_beauty` category were higher in `MG` compared to `SP` and `RJ`, with a p-value < 0.001, indicating regional pricing variations.

2. **Delivery Time and Customer Satisfaction**:
   - Spearman correlation analysis showed a negative correlation between delivery time and review scores, suggesting that longer delivery times lead to lower customer satisfaction.
   - Customers in regions with higher average delivery times (e.g., North) tended to leave lower review scores compared to regions with faster delivery times.

3. **Customer Segmentation**:
   - PCA and KMeans clustering identified three distinct customer groups:
     - **High-Spend, Frequent Buyers**: Customers with high total spending and frequent orders.
     - **Low-Spend, Infrequent Buyers**: Customers with minimal spending and fewer orders.
     - **Moderate-Spend, Patient Buyers**: Customers with moderate spending and higher tolerance for delivery delays.
   - These segments provide actionable insights for targeted marketing and service optimization.

4. **Seller Performance**:
   - Analysis of seller geolocation data revealed that 8% of sellers had incomplete or invalid geolocation entries, potentially impacting delivery efficiency.
   - Sellers with faster average delivery times received higher review scores, highlighting the importance of operational efficiency.
