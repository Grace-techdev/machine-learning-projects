# Face Classification with Random Forest and PCA (Python)

This project explores **face classification** using **Random Forest classifiers**,  
with and without **Principal Component Analysis (PCA)**, based on the  
**Labeled Faces in the Wild (LFW)** dataset.

The analysis focuses on two related approaches:
- a **Random Forest classifier** trained on high-dimensional raw pixel features  
- a **Random Forest classifier** trained on PCA-transformed features for dimensionality reduction  

The goal is to understand how **dimensionality reduction** affects model performance,  
training efficiency, and feature importance in high-dimensional image classification tasks,  
and to explore the trade-offs between accuracy and computational efficiency.

## What This Project Covers

- Loading and exploring the LFW face dataset  
- Stratified train–test splitting under class imbalance  
- Random Forest classification as a baseline model  
- Principal Component Analysis (PCA) for dimensionality reduction  
- Visualization of explained variance and eigenfaces  
- Training and evaluating Random Forests with and without PCA  
- Comparison of classification performance, training time, and feature importance  

## Key Observations

- Random Forests trained on raw pixel features achieve higher classification performance.  
- PCA significantly reduces dimensionality (from 2914 to 150 features) and speeds up training.  
- Dimensionality reduction leads to performance degradation, especially for minority classes.  
- PCA-based models produce more interpretable and structured feature importance maps.  
- Eigenfaces preserve global facial structure but lose fine-grained discriminative details.  

## How to Run

```bash
pip install -r requirements.txt
```

This project was originally developed for
University of Western Australia – CITS5508 Machine Learning (Assignments 2).