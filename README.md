# Credit Card Customer Segmentation using Clustering

![Customer Segmentation](https://example.com/segmentation-image.png)  

*Image Source: Unsplash*

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Objective](#objective)
- [Project Steps](#project-steps)
- [Data Preprocessing](#data-preprocessing)
  - [Handling Missing Values](#handling-missing-values)
  - [Outlier Detection and Treatment](#outlier-detection-and-treatment)
- [Clustering Models](#clustering-models)
  - [Hierarchical Clustering](#hierarchical-clustering)
  - [K-Means Clustering](#k-means-clustering)
  - [Cluster Visualization](#cluster-visualization)
- [Model Improvement Techniques](#model-improvement-techniques)
  - [Feature Scaling](#feature-scaling)
  - [Evaluation Metrics](#evaluation-metrics)
- [How to Run the Project](#how-to-run-the-project)
- [Real-World Applications](#real-world-applications)
- [Visualizations](#visualizations)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)
- [Contact Information](#contact-information)

---

## Project Overview
This project performs customer segmentation using clustering techniques on a credit card dataset containing the usage behavior of approximately 9,000 credit card holders over a 6-month period. The aim is to group customers based on spending patterns, payment behavior, and credit limit, enabling businesses to develop personalized marketing strategies.

## Dataset Description
The dataset contains features related to the spending behavior of credit card users:
- **CUST_ID**: Unique customer ID.
- **BALANCE**: Customer’s current balance.
- **PURCHASES**: Total amount spent on purchases.
- **CREDIT_LIMIT**: Maximum credit limit assigned to the customer.
- **PAYMENTS**: Total amount paid by the customer.

### Dataset Source:
Kaggle - [Credit Card Dataset for Clustering](https://www.kaggle.com/arjunbhasin2013/ccdata)

## Objective
The goal is to segment credit card customers into groups using clustering algorithms, facilitating the creation of targeted marketing strategies and personalized offers.

## Project Steps
1. **Data Exploration**: Analyze the dataset for missing values, outliers, and general trends.
2. **Data Preprocessing**: Handle missing data, detect outliers, and scale the features for clustering.
3. **Modeling**: Apply clustering algorithms such as K-Means and Hierarchical Clustering.
4. **Model Evaluation**: Evaluate the effectiveness of the clustering solutions using visualization techniques.
5. **Insights**: Interpret the characteristics of each cluster to identify customer behavior patterns.

---

## Data Preprocessing

### Handling Missing Values
Missing values were found in the **CREDIT_LIMIT** column, and rows with missing values were removed to ensure data integrity.

### Outlier Detection and Treatment
Outliers in **PURCHASES** and **CREDIT_LIMIT** were detected using the **Z-Score** method and removed to prevent skewed results in clustering.

---

## Clustering Models

### Hierarchical Clustering
- **Dendrogram**: Created to help determine the optimal number of clusters. A threshold was set at a height of 15, yielding two clear customer groups.
- **Agglomerative Clustering**: Applied with 2 clusters using Euclidean distance and Ward’s linkage method for effective grouping.

### K-Means Clustering
- **Elbow Method**: Used to find the optimal number of clusters, resulting in 4 clusters.
- **K-Means Algorithm**: Performed clustering using 4 groups, which aligned with different customer spending profiles.

### Cluster Visualization
Clusters were visualized on a 2D scatter plot using **PURCHASES** and **CREDIT_LIMIT** to differentiate customer segments.

---

## Model Improvement Techniques

### Feature Scaling
Features were normalized using L2 norm to bring all attributes to a comparable scale, ensuring better performance from distance-based clustering algorithms.

### Evaluation Metrics
- **Silhouette Score**: Used to evaluate the quality of the clusters, with higher values indicating better-defined clusters.

---

## How to Run the Project
1. **Clone the repository** and install dependencies from the `requirements.txt`.
2. **Download the dataset** from the provided Kaggle link.
3. **Run the Jupyter Notebook** to preprocess the data, apply clustering algorithms, and generate visualizations.
4. **Analyze the results** to identify customer segments and their characteristics.

---

## Real-World Applications
- **Targeted Marketing**: Businesses can create custom campaigns based on customer segmentation, increasing customer engagement and sales.
- **Customer Retention**: Identify high-value customers and offer personalized services or rewards to enhance loyalty.
- **Credit Risk Analysis**: Banks can use segmentation to assess credit risk more accurately by understanding customer behavior patterns.

---

## Visualizations
### Dendrogram for Hierarchical Clustering:
![Dendrogram](https://github.com/cliffordnwanna/CREDIT_CARD_CUSTOMER_SEGMENTATION/blob/main/IMAGES/Dendogram.png)

### Cluster Scatter Plot for Hierarchical Clustering :
![Hierarchical Clustering](https://github.com/cliffordnwanna/CREDIT_CARD_CUSTOMER_SEGMENTATION/blob/main/IMAGES/Hierarchical%20Clustering.png)

### Elbow Point Graph
![Elbow Point Graph](https://github.com/cliffordnwanna/CREDIT_CARD_CUSTOMER_SEGMENTATION/blob/main/IMAGES/Elbow%20Point%20Graph.png)

### Visualization of clusters
![Cluster Visualizations](https://github.com/cliffordnwanna/CREDIT_CARD_CUSTOMER_SEGMENTATION/blob/main/IMAGES/Visualzation%20of%20Clusters%20and%20Centroids.png)

---

## Conclusion
- Hierarchical Clustering revealed two distinct customer segments, while K-Means Clustering provided a more granular segmentation into four groups.
- The results provide insights into customer behavior, helping businesses tailor their strategies based on different customer profiles.

---

## Future Work
- **Feature Expansion**: Incorporate additional features, such as **PAYMENTS** or **BALANCE_FREQUENCY**, for more detailed clustering.
- **Dimensionality Reduction**: Use techniques like **PCA** to simplify data for better visualization and clustering performance.
- **Further Clustering Techniques**: Explore more advanced clustering techniques like **DBSCAN** or **Gaussian Mixture Models** for more refined segmentation.

---

## Contributing
We welcome contributions to enhance this project. To contribute:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) for details.

---

## Contact Information
For inquiries, please reach out:

**Clifford Nwanna**  
*Email*: [nwannachumaclifford@gmail.com](mailto:nwannachumaclifford@gmail.com)  

