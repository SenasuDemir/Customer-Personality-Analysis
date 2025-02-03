# 📊 Customer Personality Analysis 🛍️

## 🎯 Project Aim

The aim of this project is to perform **customer personality analysis** using clustering algorithms, such as **K-Means**, to identify meaningful customer segments. We will utilize various features from the dataset, including demographic information (e.g., age, marital status, income) and behavioral data (e.g., purchase history, product preferences, customer complaints) to form customer clusters. By doing so, we hope to provide businesses with actionable insights that will help them better understand their customers and improve marketing strategies, product offerings, and customer service. 🚀

## 📚 Dataset Explanation

The dataset used in this project contains a variety of customer attributes that can be used to analyze their personalities and behaviors. The columns in the dataset are as follows:

- **ID**: Unique identifier for each customer. 🆔
- **Year_Birth**: The year the customer was born (used to determine the age of the customer). 🎂
- **Education**: The educational level of the customer (e.g., Graduation, PhD). 🎓
- **Marital_Status**: The marital status of the customer (e.g., Single, Married, Together). 💍
- **Income**: The income of the customer. 💵
- **Kidhome**: Number of children living at home. 👶
- **Teenhome**: Number of teenagers living at home. 👦👧
- **Dt_Customer**: The date the customer joined the company. 📅
- **Recency**: The number of days since the last purchase. 🕒
- **MntWines, MntFruits, MntMeatProducts, MntFishProducts, MntSweetProducts, MntGoldProds**: Amount spent on various product categories. 🍷🍎🍖🐟🍬💍
- **NumDealsPurchases, NumWebPurchases, NumCatalogPurchases, NumStorePurchases**: The number of purchases made through different channels (deals, web, catalog, store). 🛒
- **NumWebVisitsMonth**: The number of visits to the website per month. 🌐
- **AcceptedCmp1, AcceptedCmp2, AcceptedCmp3, AcceptedCmp4, AcceptedCmp5**: Whether the customer accepted various marketing campaigns (binary variable: 0 = not accepted, 1 = accepted). 📧
- **Complain**: Whether the customer has complained (binary variable: 0 = no complaint, 1 = complaint). 😤
- **Z_CostContact**: The cost of contacting the customer. 💸
- **Z_Revenue**: The revenue generated from the customer. 💰
- **Response**: Whether the customer responded to the last marketing campaign (binary variable: 0 = no response, 1 = responded). 📬

This data provides a comprehensive view of each customer’s demographics, purchasing behavior, and responses to marketing campaigns. These features will be used to create customer clusters and analyze their personalities. 📊

## 🔍 Cluster Group Interpretation

Given the 4 customer groups (Stars, Need Attention, High Potential, and Leaky Bucket), here’s how the **Silhouette Score** can be interpreted in relation to each cluster:

- **🌟 Stars**: Old customers with high income and high spending. If this cluster is well-defined, it will positively impact the score.
- **🚨 Need Attention**: New customers with below-average income and low spending. They might overlap with **Leaky Bucket** or **High Potential**, causing ambiguity.
- **🔥 High Potential**: New customers with high income and high spending. Overlap with **Stars** can negatively affect the score.
- **💧 Leaky Bucket**: Old customers with below-average income and low spending. Difficult to distinguish from **Need Attention**, leading to lower separation between clusters.

## 📉 Silhouette Score Interpretation

The **Silhouette Score** of **0.28** indicates that the clustering model has weakly defined clusters, with significant overlap or ambiguity between some customer segments. 
