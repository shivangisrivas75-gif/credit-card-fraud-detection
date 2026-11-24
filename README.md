# credit-card-fraud-detection                                                                                                         
Comparing Logistic Regression and Isolation Forest for credit card fraud detection (Python, scikit-learn)                             
Credit Card Fraud Detection (Python, scikit-learn)                                                                                    
Dataset: Public, anonymized credit card transactions (ULB Machine Learning Group, Kaggle): 284,807 transactions, 492 frauds (0.173%). 
Method: Scaled Amount, dropped Time, and made an 80/20 stratified train-test split. Compared Logistic Regression (class-weight balanced) with Isolation Forest (unsupervised anomaly detection).                                                                     
Results (test set, 98 frauds): Logistic Regression: precision 0.059, recall 0.918, F1 0.110, PR-AUC 0.716. Isolation Forest: precision 0.320, recall 0.327, F1 0.323, PR-AUC 0.171.                                                                                
Takeaway: Logistic Regression catches most fraud but creates many false alerts. Isolation Forest raises fewer false alerts but misses about two-thirds of fraud. Accuracy is misleading here (99.8%) because of heavy class imbalance.                               
Limitations: Single train-test split, no threshold tuning, anonymized features, and 2013 data. This is a learning project and not a production system.
