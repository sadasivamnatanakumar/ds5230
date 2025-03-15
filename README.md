Drug Recommendation System
📌 Overview
This project aims to build a reliable drug recommendation system using collaborative filtering and autoencoders. It helps users find over-the-counter (OTC) medications while considering drug interactions and review-based effectiveness.

💡 Problem Statement
Searching for OTC drugs online lacks clarity and accuracy.
Current sources may miss drug interactions and rely on unreliable ratings.
Many similar projects lack public datasets or have gone behind paywalls.
🏥 Data Sources
Stanford BioSNAP – 5.5M+ drug-drug interaction samples.
DrugBank – Drug ID, names, and synonyms.
UCI Drug Review Dataset – 23K+ drug-condition-review combinations.
🛠 Methodology
1️⃣ ALS (Alternating Least Squares)
Treats conditions as rows and drugs as columns.
Uses weighted ratings to improve reliability.
Embeddings capture patterns for better recommendations.
2️⃣ Autoencoder-Based RecSys
Neural Network-based dimensionality reduction for user-item interactions.
7-layer model with ReLU activation and a learning rate of 0.001.
Trained using t-SNE for latent space visualization.
3️⃣ Collaborative Filtering with SVD
Singular Value Decomposition (SVD) on drug-condition data.
Captures 95% of variance using 5 components.
Ensures safe recommendations by mentioning negative drug interactions.
🎯 Key Outcomes
More reliable drug recommendations than search engines.
Identifies harmful drug interactions users should avoid.
Helps both general users and healthcare professionals.
📈 Results
Successfully recommended drugs for Pneumonia with strong validation.
MSE of 0.184 for Autoencoder-based recommendations.
SVD captured 95% variance, ensuring high accuracy.
