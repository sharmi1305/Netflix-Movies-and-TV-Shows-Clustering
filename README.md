Netflix Movies and TV Shows Clustering


📌 Project Overview
This project focuses on clustering Netflix movies and TV shows using unsupervised machine learning.
The aim is to group similar content based on genre, rating, duration, and other attributes, enabling better recommendations and content discovery.

Key Goals:

Cluster Netflix movies and TV shows by key attributes.

Gain insights into content patterns and trends.

Visualize clusters to understand content similarity.

Tech Stack:

Languages/Libraries: Python, Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn

ML Techniques: K-Means, Hierarchical Clustering, DBSCAN

NLP: TF-IDF Vectorization

📂 Dataset Description
The dataset contains Netflix movies and TV shows with the following columns:

Column Name	Description
show_id	Unique identifier for each show
type	Movie or TV Show
title	Title of the content
director	Director name (can be missing)
cast	Main cast (can be missing)
country	Country of production
date_added	Date added to Netflix
release_year	Year of release
rating	Content rating (e.g., PG, TV-MA)
duration	Duration in minutes or seasons
listed_in	Genres/categories
description	Short description

🛠 Data Processing
Handling Missing Data: Missing director, cast, and country filled with "Unknown" or dropped if too sparse.

Encoding: One-hot encoding for categorical variables (type, rating, listed_in).

Standardization: Scaled numerical features to zero mean and unit variance.

NLP Features: TF-IDF applied on listed_in and description.

🔍 Feature Engineering
Content Age: current_year - release_year

Genre Count: Number of genres listed in listed_in

Text Vectorization: Represent genres/themes as numerical features.

🤖 Clustering Models
K-Means: Optimized k via Elbow Method & Silhouette Score.

Hierarchical Clustering: Explored nested groups using dendrograms.

DBSCAN: Detected clusters of varying densities & outliers.

📊 Visualization
Cluster Plots: PCA/t-SNE for 2D visualization of clusters.

Heatmaps: Feature-cluster relationships.

Trend Charts: Release year trends, genre popularity, and ratings distribution.

📈 Evaluation Metrics
Silhouette Score

Davies-Bouldin Index

K-Means Inertia

💡 Key Insights
Clear clusters identified, e.g., modern TV dramas, international horror, family movies.

Genre trends show dominance of drama and international content in certain clusters.

Surge in TV series content in recent years.

K-Means + DBSCAN combination proved most effective.

📜 Conclusion
The project demonstrates how clustering and feature engineering can be used to categorize streaming content effectively.
This approach is valuable for recommendation systems and audience segmentation.

