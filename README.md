# CreditCard_Fraud_Detection

Project Overview
This project focuses on detecting fraudulent credit card transactions using anomaly detection techniques. Due to the highly imbalanced nature of the dataset (fraudulent transactions are rare), unsupervised and semi-supervised learning approaches such as Isolation Forest and Autoencoders are applied to identify anomalies.
Dataset
The Credit Card Fraud Detection dataset is sourced from Kaggle. It contains transactions made by European cardholders in September 2013. The dataset includes features transformed using PCA for confidentiality, along with 'Time', 'Amount', and a 'Class' label indicating fraud (1) or legitimate (0).
Methodology
- Data Preprocessing: Scaling features and handling class imbalance.
- Feature Engineering: Used PCA features along with "Amount" and "Time".
- Model Training:
   • Isolation Forest: An unsupervised learning algorithm effective for anomaly detection.
   • Autoencoders: Neural networks trained to reconstruct non-fraudulent data, highlighting fraud as reconstruction error.
- Evaluation Metrics: Precision, Recall, F1-Score, ROC-AUC used to assess performance.
Technologies Used
- Python
- Scikit-learn
- TensorFlow / Keras (for Autoencoders)
- Pandas and NumPy
- Matplotlib and Seaborn for visualization
How to Run the Project
1. Clone the repository.
2. Install required libraries using pip (e.g., pip install -r requirements.txt).
3. Load the Kaggle dataset and preprocess it.
4. Train the Isolation Forest and/or Autoencoder models.
5. Evaluate and visualize model results.
Results
Both Isolation Forest and Autoencoders showed strong capability to detect fraudulent transactions. The Autoencoder model achieved a high ROC-AUC score and identified fraud with low false positive rates.

Distribution of Anomaly Scores:

<img width="868" height="547" alt="distribution_credit" src="https://github.com/user-attachments/assets/6a5aa719-a720-4bf5-acb8-e17cfd412c34" />

Distribution of Transaction Amount by Class:
<img width="704" height="547" alt="distribution_transaction_credit" src="https://github.com/user-attachments/assets/9acff325-3997-4ea1-a10a-78b3a60e6717" />

