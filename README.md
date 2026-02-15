# mlpr_lab
Overview

This lab implements face detection and clustering using color-based features. Faces are detected using a Haar Cascade classifier. Mean Hue and Saturation values are extracted from each detected face and used as features for K-Means clustering. A template image is then classified into one of the learned clusters.

Aim

The objective of this lab is to:

Detect faces in an image using OpenCV

Extract HSV-based features from detected faces

Perform clustering using K-Means

Classify a new template image based on cluster assignment

Visualize clusters and centroids in feature space

Methodology

Face Detection
The image plaksha_Faculty.jpg is read using OpenCV and converted to grayscale. A Haar Cascade classifier is used to detect faces. Bounding boxes are drawn around detected faces.

Feature Extraction
The original image is converted from BGR to HSV color space. For each detected face, the mean Hue and Saturation values are computed. These values form a 2-dimensional feature vector for clustering.

K-Means Clustering
K-Means clustering is applied with two clusters. The algorithm groups faces based on similarity in HSV feature space. Cluster centroids are computed and visualized.

Template Classification
The image Dr_Shashi_Tharoor.jpg is processed in the same manner:

Face detection

HSV conversion

Mean Hue and Saturation extraction

The extracted feature vector is passed to the trained K-Means model to predict its cluster label.

Visualization
Scatter plots are generated to show:

Data points for each cluster

Cluster centroids

Template image classification in feature space

Distance-Based Learning Concept

K-Means is a distance-based algorithm that uses Euclidean distance to assign points to clusters. It minimizes within-cluster variance by iteratively updating centroids and reassigning data pts.

This lab demonstrates how clustering can be applied to image data using simple color-based features.

Key Observations

HSV features can differentiate images based on color characteristics.

K-Means groups faces with similar color distributions.

The template image can be classified using proximity to learned cluster centroids.

Files Included:

Lab 5 Jupyter Notebook (.ipynb)

README.md

plaksha_Faculty.jpg

Dr_Shashi_Tharoor.jpg



Conclusion: 

This lab demonstrates practical implementation of distance-based clustering using real image data. It highlights the importance of feature extraction and visualization in understanding clustering behavior.
