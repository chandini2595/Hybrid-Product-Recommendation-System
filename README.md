# Hybrid-Product-Recommendation-System

A scalable hybrid recommendation system that combines Singular Value Decomposition (SVD), TF-IDF, and Random Forest to provide personalized product recommendations.

![GitHub](https://img.shields.io/github/license/chandini2595/Hybrid-Product-Recommendation-System)
![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

# Overview

This project implements a hybrid recommendation system combining three approaches:
- Collaborative Filtering using SVD (Singular Value Decomposition)
- Content-Based Filtering using TF-IDF
- Hybrid approach using Random Forest to combine both methods
<img width="593" alt="image" src="https://github.com/user-attachments/assets/ab350625-6196-4263-a254-a620a35cbae9">

# High Level Architecture 

<img width="569" alt="image" src="https://github.com/user-attachments/assets/788b5fd9-ffd3-4fd9-bb4b-705fd4186a0e">

# Dataflow diagram

![image](https://github.com/user-attachments/assets/07ebf81c-7f64-4696-bce6-f963c97fe612)

# Sequence diagram

![image](https://github.com/user-attachments/assets/d272256d-3827-48c1-b7e5-64faeeb625e3)

# Component level design

![image](https://github.com/user-attachments/assets/708865a1-e14a-4100-98cc-60b4728a8091)

# Dataset

https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

# Features

## Collaborative Filtering (SVD)
- Matrix factorization for user-item interactions
- Handles sparse rating matrices efficiently
- Captures latent features from user behavior

## Content-Based Filtering (TF-IDF)
- Text analysis of product descriptions
- Feature extraction from product attributes
- Cosine similarity for item matching

## Hybrid Approach (Random Forest)
- Combines predictions from both models
- Optimizes weights dynamically
- Handles cold-start problems effectively

I'll help you add the KDD (Knowledge Discovery in Databases) steps we incorporated in the project.

# KDD

## 1. Data Selection
- Selected relevant data sources:
  - User-item interaction data (reviews/purchases)
  - Product metadata (descriptions, categories)
  - User demographic information
- Identified target variables for recommendation

## 2. Data Preprocessing
- **Data Cleaning**
  - Handled missing values
  - Removed duplicates
  - Fixed inconsistent data
- **Feature Engineering**
  - Created user interaction features
  - Extracted text features from product descriptions
  - Generated temporal features

## 3. Data Transformation
- **Text Processing**
  - Applied TF-IDF vectorization on product descriptions
  - Tokenization and lemmatization
  - Removed stop words
- **Normalization**
  - Scaled numerical features
  - Encoded categorical variables
- **Dimensionality Reduction**
  - Applied SVD for collaborative filtering
  - Reduced feature space for efficient processing

## 4. Data Mining
- **Collaborative Filtering**
  - Implemented SVD for matrix factorization
  - Captured latent features from user-item interactions
- **Content-Based Filtering**
  - Used TF-IDF for text analysis
  - Computed item similarities
- **Hybrid Model**
  - Implemented Random Forest
  - Combined predictions from both approaches

## 5. Evaluation
- **Metrics Used**
  - RMSE (Root Mean Square Error)
- **Validation Strategies**
  - Cross-validation (nfold)
  - Train-test split
  - Temporal validation
- **Performance Analysis**
  - Cold start handling effectiveness
  - Recommendation diversity
  - Scalability testing

## 6. Knowledge Representation
- **Visualization**
  - User interaction patterns
  - Item similarity patterns
  - Model performance metrics
- **Insights**
  - User behavior patterns
  - Product relationships
  - Model effectiveness analysis

# Full Demo Youtube Link: 

https://youtu.be/pKpgschLBFc

# Application Run with Gradio UI Demo Youtube Link: 

https://youtu.be/35OBaW7t4B4

# Interpretability

<img width="450" alt="image" src="https://github.com/user-attachments/assets/40df5561-bd5e-4c46-b38d-d093fa96fbd0">





