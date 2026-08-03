# Credit Card Fraud Detection using K-Means Clustering

## Introduction

This project focuses on detecting fraudulent credit card transactions using unsupervised learning techniques. Since fraud cases are rare, anomaly detection is used instead of traditional classification methods.

## Objective

To identify anomalous (fraudulent) transactions by applying clustering techniques and analyzing the distance of data points from cluster centroids.

## Dataset

The dataset contains credit card transactions with anonymized features (V1–V28), along with Time and Amount.  

- Class = 0 → Normal transaction  
- Class = 1 → Fraudulent transaction  

## Methodology

### 1. Data Understanding
- Loaded and explored dataset  
- Checked missing values
- Identified and removed duplicate rows   
- Analyzed class imbalance  

### 2. Data Preprocessing
- Removed target column for training  
- Applied feature scaling  

### 3. Clustering
- Used K-Means algorithm  
- Applied Elbow Method to find optimal clusters (K ≈ 4)  

### 4. Anomaly Detection
- Calculated distance from cluster centroids  
- Selected top 1% farthest points as anomalies  

### 5. Evaluation
- Compared predicted anomalies with actual labels  
- Used Confusion Matrix, Precision, and Recall  

### 6. Visualization
- Applied PCA to reduce dimensions  
- Visualized clusters and anomalies  

## Results

- Normal transactions formed dense clusters  
- Anomalies appeared scattered and far from cluster centers  
- The model successfully identified unusual transaction patterns  

## Conclusion

K-Means clustering combined with distance-based anomaly detection effectively identified potential fraudulent transactions. While the method may produce some false positives, it provides a useful approach for detecting suspicious activity in highly imbalanced datasets.

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  

## How to Run

1. Load the dataset  
2. Run the notebook step by step  
3. Observe clustering results and evaluation metrics
