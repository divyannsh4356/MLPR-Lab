# Face Detection and Clustering using K-Means

## Overview

This project implements a complete computer vision pipeline that detects faces in a group image, extracts color-based features, applies K-Means clustering, and classifies a new template face into one of the learned clusters.

The project demonstrates how face detection and unsupervised learning can be combined for facial grouping based on color characteristics.

---

## Aim

The objective of this project is to:

- Detect faces in a group image using Haar Cascade.
- Extract average Hue and Saturation values from each detected face.
- Perform clustering using K-Means.
- Classify a new template face into one of the clusters.
- Visualize clustering results.

---

## Methodology

### 1. Face Detection

Faces were detected using OpenCV’s Haar Cascade classifier.

### 2. Feature Extraction

- Each detected face was converted from BGR to HSV color space.
- The average Hue and Saturation values were computed.
- These values were used as feature vectors.

### 3. K-Means Clustering

- K-Means with 2 clusters was applied.
- Faces were grouped based on similarity in Hue and Saturation.
- Cluster centroids were computed and visualized.

### 4. Template Face Classification

- A new face image was processed similarly.
- Its Hue and Saturation were extracted.
- The trained K-Means model predicted its cluster.
- The template face was plotted in the feature space.

---

## Results

### Face Detection
<img width="2048" height="1366" alt="image" src="https://github.com/user-attachments/assets/9f8f93e0-be87-418e-a36f-b7d1eaa64f85" />


### K-Means Clustering Visualization
<img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/b767204e-2c9e-40a2-9cd6-45ff4ad28b18" />


### Two-Cluster Plot with Centroids
<img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/129387ae-4c7d-4c14-9291-6be3101f064e" />

### Template Face Detection
<img width="400" height="400" alt="image" src="https://github.com/user-attachments/assets/e6fffe06-0ddc-4ce8-91fe-ab1ed9894547" />

### Template Face Added
<img width="1083" height="622" alt="image" src="https://github.com/user-attachments/assets/4b3b1fb4-8187-44a6-8032-fd6a7a891b47" />

### K-Means Clustering Visualization
<img width="1005" height="545" alt="image" src="https://github.com/user-attachments/assets/5b02916f-205c-4b4d-a10d-b5617f09f946" />


---

## Key Findings

- HSV color space provides useful features for facial grouping.
- Hue and Saturation allow meaningful separation using K-Means.
- Two distinct clusters were formed.
- The template face was successfully assigned to one of the clusters.
- Cluster centroids represent average color characteristics of each group.

---

## Conclusion

This project shows that basic feature extraction combined with unsupervised learning can effectively group faces based on visual similarity. 

---
