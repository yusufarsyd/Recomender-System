# Neural Collaborative Filtering (NCF) - Recommender System 1

## Overview
This project implements Neural Collaborative Filtering (NCF) on the MovieLens 1M dataset to predict user-item interactions. The model combines linear (GMF) and nonlinear (MLP) representations.

## Dataset
- Users: 6038  
- Items: 3533  
- Split: 70% train, 15% validation, 15% test  

## Model
- GMF (linear interactions)  
- MLP (nonlinear interactions)  
- Fusion layer  

## Training
- Loss: Binary Cross-Entropy  
- Optimizer: Adam  
- Negative sampling: 2 and 4 per positive interaction  
- Dynamic negative sampling (regenerated each epoch)  
- Early stopping based on validation loss  

## Evaluation
- Full-ranking evaluation  
- Recall@10  
- NDCG@10  

## Results
Best model performance:
- Recall@10 ≈ 0.0862
- NDCG@10 ≈ 0.1342

## How to Run
1. Install dependencies:
pip install pandas numpy scikit-learn torch matplotlib

2. Run:
Recommender_System_1.ipynb