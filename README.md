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

<img width="1584" height="926" alt="image" src="https://github.com/user-attachments/assets/883e8c6a-ea85-4e6f-822f-70899f8a01cf" />
<img width="496" height="492" alt="image" src="https://github.com/user-attachments/assets/cd79acf1-7f27-4b65-b429-1289d4ba517e" />
<img width="966" height="525" alt="image" src="https://github.com/user-attachments/assets/f87f4879-3010-41d4-8b53-919228fe2e86" />
<img width="966" height="523" alt="image" src="https://github.com/user-attachments/assets/eae2ebb8-b002-4b21-9338-ef320de7d1b5" />
<img width="967" height="524" alt="image" src="https://github.com/user-attachments/assets/30ed41ae-dc82-443d-b026-b7b91bad6c2c" />
<img width="969" height="526" alt="image" src="https://github.com/user-attachments/assets/87371e3a-42fc-43a9-9d84-1bfa7b51e0ea" />


Files Included:

Lab 5 Jupyter Notebook (.ipynb)

README.md

plaksha_Faculty.jpg

Dr_Shashi_Tharoor.jpg



Conclusion: 

This lab demonstrates practical implementation of distance-based clustering using real image data. It highlights the importance of feature extraction and visualization in understanding clustering behavior.
