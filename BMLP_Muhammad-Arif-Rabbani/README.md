# 🔬 BMLP Project Submission
## 🧠 Project Overview
This project is a submission assignment. This project analyzes customer behavior by grouping several customers into several criteria groups. This project uses the clustering method using K-Means Clustering and then analyzed using Classification.
## 🎯 Objectives
- Group data using K-Means Clustering
- Analysis using several Classification models
## 📁 Dataset
[Bank Transaction Data](https://drive.google.com/drive/folders/1Zs7VmPZ-jNwsRlMKH65Ea-LApSwx6lKx?usp=drive_link)
## 🛠️ Methodology
- Exploratory Data Analysis (EDA)
  - Review the number of rows columns and data types in the dataset
  - Display descriptive statistics of the dataset
  - Display correlations between features
  - Display histograms for all numeric columns
  - Visualize correlation matrix using heatmap
- Data Preprocessing
  - Handling missing values
  - Handling duplicate data
  - Handling outliers
  - Feature scaling using Standard Scaler
  - Drop in the column that contains the ID and IP Address information
  - Perform feature encoding using Label Encoder for categorical features
- Clustering Model Development
  - Feature Scaling is done first, then the Elbow Method visualization is performed
  - Clustering using the K-Means Clustering algorithm
  - Creating a visualization of clustering results
- Interpretation of clustering results
- Inverse dataset to normal range for numeric and inverse encoded dataset to its original category
- Reinterpretation after inverse
- Classification Model Development
  - Data Splitting
  - Create a classification model using Decision Tree
  - Training models using classification algorithms other than Decision Tree
  - Displays the results of evaluating accuracy, precision, recall, and F1-Score
  - Saving models using joblib
  - Perform Hyperparameter Tuning
  - Saving Hyperparameter Tuning using joblib
## 📈 Results
- Cluster 0 Analysis:
  - Interpretation: High-Income Cluster
  - This cluster has a moderate number of transactions, not more than cluster 1 or a little like cluster 2. Likewise, in `CustomerAge` which has an adult age range that is not too old and a little at a young age. This cluster is very rich and has a lot of savings, unlike cluster 1 which has little savings or cluster 2 which has savings that are fairly moderate.Then this cluster is dominated by the professions of doctors and engineers who have high incomes in the `CustomerOccupation` feature.
- Cluster 1 Analysis:
  - Interpretation: High-Spending Youth Cluster
  - This cluster has characteristics with a fairly large number of transactions. It is considered very wasteful because the number of transactions is not balanced with the amount of savings owned. It can be seen in the `TransactionAmount` feature with the highest data distribution but the `AccountBalance` feature has the lowest data distribution. This cluster has an age range of only young people in the `CustomerAge` feature. This cluster is dominated by students and college students in the `CustomerOccupation` feature who basically do not have an income.
- Cluster 2 Analysis:
  - Interpretation: Retiree Cluster
  - This cluster is the most economical cluster with a small number of transactions and moderate savings. Seen in the `TransactionAmount` feature with the lowest data distribution and in the `AccountBalance` feature has a medium data distribution. This cluster has an old adult age range in the `CustomerAge` feature. This cluster is dominated by retired professions who are no longer working and followed by the engineering profession.
