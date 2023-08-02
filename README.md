# Online_Retail_Customer_Segmentation (Unsupervised ML)
The objective of this project is to identify major customer segments of a online retail store using the unsupervised machine learning.
# Problem Statement
In this project, our task is to identify major customer segments on a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.
# Dataset Overview:
The dataset consists of 541,909 rows and 8 columns. The columns include Invoice No, Stock Code, Description, Quantity, Invoice Date, Unit Price, Customer ID, and Country. It contains both numerical and categorical data types. We also observed missing values in the Customer ID and Description columns, duplicate values in the dataset, and other data peculiarities.
# Exploratory Data Analysis (EDA):
During exploratory data analysis (EDA), we made interesting discoveries. We found that total sales had grown significantly from 2010 to 2011, indicating business growth. Sales peaked during November and December, suggesting higher demand during the holiday season. We also observed that Thursdays had the highest sales, while Sundays had the lowest. Most of our customers were from the United Kingdom, with substantial numbers from Germany, France, EIRE, Spain, etc.
# Data Pre-processing and Feature Engineering:
To enhance the data for clustering analysis, we performed data pre-processing and feature engineering steps. This involved removing irrelevant features related to transaction details and focusing on more relevant features Recency, Frequency, and Monetary. We also applied outlier treatment techniques using the interquartile range (IQR) method and conducted data transformations, including logarithmic transformations, to normalize the data and reduce the impact of outliers. Finally, we used data scaling techniques, such as standard scaling, to bring different features to a common scale.
# Machine Learning Models:
We implemented two machine learning models for customer segmentation: K-Means clustering and Hierarchical clustering.

K-Means Clustering:
First, we used the K-Means clustering algorithm. We determined the optimal number of clusters using the elbow curve method and evaluated the model's performance using metrics such as silhouette score, Davies-Bouldin index, and Calinski-Harabasz index. We performed cross-validation and hyperparameter tuning using GridSearchCV to find the best combination of hyperparameters. These parameters helped achieve effective clustering of the customer data.

Hierarchical Clustering:
Next, we employed hierarchical clustering, which groups data into hierarchical structures based on similarities. We again performed cross-validation and hyperparameter tuning using GridSearchCV to find the optimal combination of hyperparameters.We evaluated the model's performance using metrics similar to the K-Means model.
# Evaluation and Model Selection:
Based on the evaluation metrics, the hyperparameter-tuned K-Means model with five clusters emerged as the optimal choice for customer segmentation. Although the Hierarchical Clustering model with two clusters had a higher silhouette score, the hyperparameter-tuned model demonstrated better visual separation of customer groups, aligning with our business objective of wide customer segmentation.
# Conclusion:
In conclusion, the project "Online Retail Customer Segmentation" successfully employed unsupervised machine learning techniques to identify distinct customer segments and gain valuable insights into customer behavior. The hyperparameter-tuned K-Means model with five clusters emerged as the optimal choice for customer segmentation, providing a comprehensive understanding of customer preferences and enabling targeted marketing strategies. The insights derived from our analysis can be utilized to enhance customer retention, optimize pricing, and improve inventory management, thereby positively impacting business outcomes.
