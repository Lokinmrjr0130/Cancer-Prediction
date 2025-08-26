# Gene Expression-Based Cancer Subtype Classification

This repository contains the code and results for a machine learning and deep learning based study on classifying cancer subtypes from gene expression data. The work focuses on building a complete pipeline—from preprocessing to model comparison—to demonstrate how computational methods can be used to uncover molecular signatures of cancer and support precision medicine.

# Project Overview

Cancer is a heterogeneous disease, and differences at the molecular level make diagnosis and treatment challenging. This project aims to build robust classifiers that can distinguish between major cancer types using transcriptomic (gene expression) profiles.

By combining statistical methods, classic machine learning, and deep learning, this project highlights how computational approaches can improve both predictive performance and biological understanding.

# Dataset

Source: Public dataset (ICMR, available via Kaggle)

Samples: ~802 patient samples

Cancer Types (5 classes):

BRCA – Breast Cancer

KIRC – Kidney Renal Cancer

COAD – Colon Cancer

LUAD – Lung Cancer

PRAD – Prostate Cancer

Features: ~20,000 gene expression values per patient

# Methodology
1. Data Preprocessing

Handling missing values

Scaling and normalization

Ensuring data consistency for modeling

2. Dimensionality Reduction

PCA (Principal Component Analysis): Reduced ~20,000 genes into a smaller set of components while preserving most of the variance.

3. Clustering (Unsupervised Exploration)

K-Means Clustering: Revealed natural groupings that aligned well with cancer subtypes.

Hierarchical Clustering (Ward’s Linkage): Offered insights into relationships between samples and cancer types.

4. Feature Selection

ANOVA (Analysis of Variance): Identified statistically significant genes.

Example: gene_9651 was highlighted as a strong predictor of subtype.

5. Model Implementation

We tested a wide range of models:

Deep Learning Models

1D Convolutional Neural Network (CNN):

Custom 2-layer CNN architecture

Achieved 99.38% validation accuracy

Machine Learning Models

Support Vector Machine (SVM): 97.9% accuracy

Gradient Boosting: 97.9% accuracy

Random Forest: 97.5% accuracy (also useful for feature importance analysis)

# Results & Insights

Performance: Deep learning models (especially CNN) achieved the best accuracy.

Biological Insights: ANOVA-based feature selection highlighted key genes that may serve as biomarkers.

Data Structure: Clustering confirmed that the cancer types form distinct molecular groups.
