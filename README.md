# Wholesale Distributor Customer Segmentation with K-Means Clustering

![Python](https://img.shields.io/badge/Python-3.8+-green)
![Jupyter Notebook](https://img.shields.io/badge/Tools-Jupyter%20Notebook-orange)
![Scikit-learn](https://img.shields.io/badge/Library-Scikit--learn-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-yellow)
![Matplotlib](https://img.shields.io/badge/Library-Matplotlib-lightblue)

## Project Overview

Customer segmentation is a crucial process for businesses to identify distinct groups within their customer base. This project applies K-Means Clustering, an unsupervised learning algorithm, to segment customers based on their purchasing behaviors and demographic information. The objective is to help businesses understand different customer profiles and tailor their strategies accordingly.

## Table of Contents

- [Introduction](#introduction)
- [Objective](#objective)
- [Dataset Description](#dataset-description)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Modelling](#modelling)
- [K Means Clustering](#k-means-clustering)
- [Model Evaluation](#model-evaluation)
- [Reasult](#reasult)
- [Dependencies](#dependencies)
- [How to Run](#how-to-run)

## Introduction

Customer segmentation involves grouping customers with similar characteristics to enable targeted marketing and personalized service. K-Means Clustering is a popular technique for this task, as it partitions data into clusters based on feature similarity. This project demonstrates how to use K-Means Clustering to identify distinct customer segments.

# Objective
The main objectives of this project are:

-Segment Customers: Use K-Means Clustering to divide customers into distinct segments.

-Analyze Segments: Understand the characteristics of each segment.

-Provide Insights: Offer actionable insights to improve marketing strategies and customer engagement.

## Dataset Description

The dataset contains information on annual spending by clients in six distinct product categories. These categories reflect the customer's purchasing behaviour and provide a basis for segmentation

The data set refers to clients of a wholesale distributor. It includes the annual spending in monetary units (m.u.) on diverse product categories.

The dataset for this project can be found on the UCI Machine Learning Repository. For the purposes of this project, the features 'Channel' and 'Region' will be excluded in the analysis — with focus instead on the six product categories recorded for customers.

Description of Categories

-FRESH:                           annual spending (m.u.) on fresh products (Continuous)

-MILK:                            annual spending (m.u.) on milk products (Continuous)

-GROCERY:                         annual spending (m.u.) on grocery products (Continuous)

-FROZEN:                          annual spending (m.u.)on frozen products (Continuous)

-DETERGENTS_PAPER:                annual spending (m.u.) on detergents and paper products (Continuous)

-DELICATESSEN:                      annual spending (m.u.) on and delicatessen products (Continuous)


"A store selling cold cuts, cheeses, and a variety of salads, as well as a selection of unusual or foreign prepared foods."

Dataset link : https://www.kaggle.com/datasets/muhammadyasirsaleem/customer-segmentation-dataset

## Data Preprocessing

Data preprocessing involves preparing the data for clustering. Steps include:

-Handling Missing Values: Check for and address any missing values.

-Feature Scaling: Normalize features to ensure they are on the same scale.

-Feature Selection: Use relevant features for clustering.


## Exploratory Data Analysis

EDA helps to understand the data and identify patterns. Key analyses include:

-Distribution Analysis: Examine the distribution of annual income and spending score.

-Correlation Analysis: Investigate relationships between features.

-Visualization: Plot data to identify potential clusters.


# Modelling

## K Means Clustering
K-means clustering is used to partition the data into k clusters. Each cluster represents a group of customers with similar characteristics.

# Model Evaluation
Evaluating the performance of a K-Means Clustering model involves assessing the quality and effectiveness of the clustering results. Since K-Means is an unsupervised learning algorithm, traditional evaluation metrics like accuracy are not applicable. Instead, we use various techniques to evaluate the clustering results.

Key Evaluation Techniques

-**Within-Cluster Sum of Squares (WCSS)**:

The Within-Cluster Sum of Squares measures the total distance between data points and their corresponding cluster centers. A lower WCSS indicates tighter and more distinct clusters.


-**lbow Method**:

The Elbow Method helps in choosing the optimal number of clusters by plotting WCSS against different values of k. The "elbow" point in the plot indicates the optimal number of clusters.


-**Silhouette Score**:

The Silhouette Score evaluates how well each data point fits within its cluster compared to other clusters. The score ranges from -1 to 1, with higher values indicating better-defined clusters


-**Cluster Visualization**:

Visualizing the clusters helps in qualitatively assessing the clustering results. By plotting the clusters, you can visually inspect the separation between different clusters and ensure they are well-formed

# Reasult

After running K-Means Clustering, the dataset is segmented into distinct clusters. Each cluster represents a customer segment with similar spending behaviors and income levels.

## Cluster Analysis

![image](https://github.com/user-attachments/assets/44afad2c-ce06-4ebd-9ae3-139631dc7f55)

red colour are less fresh blue colour are more fres.


# Dependencies
This project requires the following libraries:

-Python 3.8+

-Jupyter Notebook

-Pandas

-Scikit-Learn

-Seaborn

-Matplotlib

-NumPy


## How to Run

To run the project:
1. Clone this repository.
2. Install the required dependencies.
3. Open the Jupyter Notebook and execute the cells to train and evaluate the model.

```bash
git clone https://github.com/yasirsaleem502/Customer-Segmentation-with-K-Means-Clustering.git
cd customer-segmentation
pip install -r requirements.txt
