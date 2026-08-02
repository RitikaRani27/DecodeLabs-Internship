# Customer Segmentation using K-Means Clustering

## Overview

This project was developed as part of my Data Science Internship at **DecodeLabs**.

The project applies unsupervised machine learning techniques to segment customers based on their demographic characteristics, purchasing behavior, and income. The goal is to identify groups of customers with similar characteristics to help businesses design targeted marketing campaigns, improve customer retention, and deliver personalized promotions.

The project follows a complete data science workflow, including data exploration, data cleaning, feature engineering, exploratory data analysis (EDA), feature scaling, dimensionality reduction using Principal Component Analysis (PCA), cluster optimization using the Elbow Method and Silhouette Score, and customer segmentation using the K-Means clustering algorithm.

---

## Project Objectives

* Explore and understand customer demographic and purchasing data.
* Clean and pre-process the dataset for machine learning.
* Engineer meaningful features to improve clustering.
* Reduce data dimensionality using PCA.
* Determine the optimal number of clusters.
* Perform customer segmentation using K-Means.
* Analyze customer groups and generate actionable business insights.

---

## Dataset

**Dataset:** Customer Personality Analysis

The dataset contains customer information such as:

* Demographic information
* Education level
* Marital status
* Income
* Product spending
* Purchase behavior
* Customer enrollment date
* Campaign responses

---

## Project Workflow

### 1. Dataset Exploration

* Loaded the dataset into Google Colab.
* Examined dataset dimensions.
* Inspected data types.
* Generated summary statistics.
* Checked for missing values.
* Identified potential preprocessing requirements.

---

### 2. Data Cleaning & Preprocessing

The following preprocessing steps were performed:

* Missing values in the **Income** column were replaced using median imputation.
* Removed unnecessary columns:

  * ID
  * Z_CostContact
  * Z_Revenue
* Converted **Dt_Customer** into **Customer_For_Days** to represent customer tenure.
* Encoded categorical variables using Label Encoding.
* Produced a fully numerical dataset suitable for machine learning.

---

### 3. Feature Engineering

Additional features were created to improve customer representation.

* Age
* Total_Spending
* Total_Purchases
* Customer_For_Days

These engineered features provide richer information for clustering.

---

### 4. Exploratory Data Analysis (EDA)

Several visualizations were created to better understand the data.

Analysis included:

* Feature distributions
* Income distribution
* Spending behavior
* Purchase frequency
* Correlation heatmap
* Boxplots for outlier detection
* Customer demographics

---

### 5. Feature Scaling

The numerical features were standardized using **StandardScaler**.

Standardization ensures that all features contribute equally to distance calculations used by PCA and K-Means.

---

### 6. Principal Component Analysis (PCA)

PCA was applied to reduce the dimensionality of the dataset.

Benefits include:

* Reduced computational complexity
* Easier visualization
* Reduced feature redundancy
* Two principal components used for visualization

---

### 7. Cluster Optimization

Two methods were used to determine the optimal number of clusters.

#### Elbow Method

* Calculated Within-Cluster Sum of Squares (WCSS)
* Compared cluster sizes from 1 to 10
* Identified the elbow point

#### Silhouette Score

* Calculated silhouette scores for cluster values from 2 to 10
* Selected the cluster count with the highest score

---

### 8. K-Means Clustering

The final K-Means model was trained using the optimal number of clusters.

Each customer was assigned to a cluster.

The resulting customer segments were analyzed to identify common characteristics and business opportunities.

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Machine Learning Techniques

* Data Cleaning
* Feature Engineering
* Label Encoding
* StandardScaler
* Principal Component Analysis (PCA)
* K-Means Clustering
* Elbow Method
* Silhouette Score

---

## Results

The project successfully segmented customers into meaningful groups based on purchasing behavior and demographic information.

The identified customer segments can be used for:

* Targeted marketing campaigns
* Customer retention strategies
* Personalized product recommendations
* Business decision-making
* Customer relationship management



---

## Project Structure

```
Project_3_Unsupervised_Learning_Customer_Segmentation
│
├── Project_3_Unsupervised_Learning_(Customer_Segmentation).ipynb
├── marketing_campaign.csv
├── Customer_Segmentation_Result.csv
├── kmeans_customer_segmentation.pkl
└── README.md
```

---


## Future Improvements

* Compare K-Means with DBSCAN and Hierarchical Clustering.
* Perform hyperparameter tuning.
* Deploy the clustering model using Streamlit.
* Build an interactive customer segmentation dashboard.
* Automate customer persona generation.

---

## Conclusion

This project demonstrates a complete unsupervised machine learning pipeline for customer segmentation. Starting from raw customer data, the project performs preprocessing, feature engineering, exploratory analysis, dimensionality reduction, cluster optimization, and K-Means clustering to identify meaningful customer groups.

The resulting customer segments provide valuable business insights that can support data-driven marketing strategies, improve customer engagement, and enable more personalized business decisions.

---

## Author

**Ritika Rani**

Data Science Intern

DecodeLabs Internship
