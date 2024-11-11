---
title: "Grassroot Innovation Analysis"
excerpt: "Short description of portfolio item number 1<br/><img src='/images/MCA.png'>"
collection: portfolio
---

# Project Overview 

In this project, I explored grassroots innovation data using Multiple Correspondence Analysis (MCA) to identify key patterns across various categories, such as demographics, career paths, and urban vs. rural innovation contexts. This project involved several steps in data preprocessing, analysis, and visualization that culminated in a published study.

# Data Preparation and Analysis
The dataset included categorical variables representing different aspects of grassroots innovators. To handle this data effectively:

1. **Data Cleaning**: Rows with missing values were removed to ensure a balanced dataset.
2. **Variable Transformation**: Categorical variables were transformed into factors, enabling them to be analyzed with MCA.
   
# MCA Implementation

The MCA was conducted using the FactoMineR and factoextra libraries in R. This technique helped us reduce the data’s dimensionality, capturing the most significant relationships among the variables:

* **Optimal Dimensions**: An eigenvalue scree plot was used to determine the optimal number of dimensions, ensuring the analysis retained the most variance.
Variance Explained: The selected dimensions captured significant variance, allowing us to interpret the positions of categories and individuals in a reduced space.

# Visualizations

Using ggplot2 and factoextra, I generated visualizations to display the analysis results effectively:

* **Variable Factor Map**: The MCA factor map (see figure below) illustrates the relationships among variables. Categories with similar response patterns are located closer together, suggesting potential clusters or groupings of grassroots innovators.

Contribution Plot: Additional visualizations displayed the contribution of each variable to the MCA dimensions, which helped to identify the most influential categories in the dataset.

Clustering Analysis: K-means clustering was performed on the MCA output to group similar observations. I used the Elbow, Silhouette, and Gap Statistic methods to identify the optimal number of clusters. The final cluster plot (see figure) reveals clear groups within the data, with ellipses representing confidence intervals around each cluster, providing insights into distinct types of grassroots innovators.

# Technical Challenges and Solutions

Implementing the MCA required careful selection of variables and interpretation of dimensions. For example, identifying statistically significant categories and investigating R-squared values for each category ensured robustness in the analysis. Additionally, the clustering results were overlaid on the MCA plot using the ggplot2 library’s advanced features, creating an intuitive visualization that highlighted key insights.

# Results
This analysis revealed distinct clusters among grassroots innovators, categorized by factors such as career background and innovation field. The findings provide valuable insights into how these clusters vary by region and demographics, contributing to targeted policy suggestions aimed at supporting innovation in diverse contexts.

**Suggested Citation**: Ghadimi, A., Samnadar Ali Eshtehardi, M., Saviz, M., Mahdad, M., (2023) Grassroots Innovations and innovators: the case of Iran, Journal of Innovation and Development, 1-24. DOI: [https://doi.org/10.1080/2157930X.2023.2233208](https://doi.org/10.1080/2157930X.2023.2233208)

# Images:

<img src="/images/grassrootImage/GrassrootsInnovators.png" alt="Figure 1: The distribution of grassroots innovations by grassroots innovators">

Figure 1. The distribution of grassroots innovations by grassroots innovators
