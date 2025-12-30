# SVM and Voting Classifiers for Medical Diagnosis (Python)

This project explores **supervised classification models** for medical diagnosis using the  
**UCI Breast Cancer Wisconsin (Diagnostic)** dataset.

The analysis focuses on two related approaches:
- a **Support Vector Machine (SVM)** classifier with feature scaling and hyperparameter tuning  
- a **Voting Classifier** that combines multiple base models to improve robustness and recall  

The goal is to understand how different classification strategies behave in settings where  
**false negatives are costly**, and how model choice, hyperparameters, and decision strategies  
affect precision–recall trade-offs rather than accuracy alone.

## What This Project Covers

- Exploratory data analysis (EDA) on medical diagnostic features  
- Support Vector Machine (SVM) training with recall-oriented hyperparameter tuning  
- Feature scaling and correlation-based feature reduction  
- Decision threshold adjustment using precision–recall curves  
- Ensemble learning using a soft Voting Classifier  
- Comparison of base models and ensemble performance  

## Key Observations

- SVM achieves strong performance when optimized for recall, which is critical in medical screening.  
- Feature scaling and correlation reduction improve model stability.  
- Adjusting the decision threshold significantly increases recall with acceptable precision loss.  
- The Voting Classifier outperforms individual models by combining diverse decision boundaries.  
- Soft voting performs better than hard voting on this moderately imbalanced dataset.

## How to Run

```bash
pip install -r requirements.txt
```

This project was originally developed for
University of Western Australia – CITS5508 Machine Learning (Assignments 1 & 2).