# Credit_Risk_Analysis
Module 17: Machine Learning

# Project Overview of the Analysis
A peer-to-peer lending services company will use the credit card credit dataset from LendingClub to oversample the data using the RandomOverSampler and SMOTE algorithms and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over and undersampling using the SMOTEENN algorithm. Next, we will compare the two new machine learning models that reduce bias, BalancedRandomForestClassifier, and EasyEnsembleClassifier, to predict credit risk. The performance of these models and a written recommendation on whether or not to foretell credit risk will be asses after the completion of the analysis.

# Resources
- Data: LoanStats_2019Q1.csv from LendingClub
- Software and tools: Jupyter notebook; pandas, numpy, scikit-learn, imbalanced-learn libraries

# Results
## Oversample algorithms
- Naive RandomOverSampler Results

<img width="918" alt="Screen Shot 2022-10-04 at 9 32 52 AM" src="https://user-images.githubusercontent.com/105765150/193833334-8c531a75-8ac5-49c4-866f-be85983857dd.png">

- SMOTE Oversampler Results

<img width="813" alt="Screen Shot 2022-10-04 at 9 37 13 AM" src="https://user-images.githubusercontent.com/105765150/193834596-0516c0ef-46f1-4f76-9985-70f71dd450d5.png">

## Undersample
- ClusterCentroids results
<img width="907" alt="Screen Shot 2022-10-04 at 9 43 05 AM" src="https://user-images.githubusercontent.com/105765150/193835657-37c3e117-e6a2-4f6e-825a-6dafa45fc20e.png">

## Combination (Over and Under) Sampling
<img width="868" alt="Screen Shot 2022-10-04 at 9 47 07 AM" src="https://user-images.githubusercontent.com/105765150/193836695-b74472d0-af8c-443d-afde-2779f093732a.png">

## Ensemble Learners Algorithms
- Balanced Random Forest Classifier
<img width="1042" alt="Screen Shot 2022-10-04 at 9 51 46 AM" src="https://user-images.githubusercontent.com/105765150/193837732-70284d73-90f0-41d2-af4e-0d3e8c6a8624.png">

- Easy Ensemble AdaBoost Classifier
<img width="1018" alt="Screen Shot 2022-10-04 at 9 53 32 AM" src="https://user-images.githubusercontent.com/105765150/193838140-9dcf4f96-1d18-4584-b94e-af139c7d4ea4.png">

# Summary
The models used to present the credit risk analysis show weak precision in determining if credit risk is high—for example, the Ensemble model, especially on the sensitivity of the increased risk credits. For instance, while the Adaboost algorithm shows a recall sensitivity of 92%, it detects almost all high-risk credit. In addition, the BalancedRandomForest algorithm did not show any significant improvement, with a significance of 70% from linear regression with oversampling or downsampling. On the other hand, in all models with low precision to detect high-risk loans, many low-risk credits will still be falsely seen as high risk, penalizing the bank's credit strategy. Therefore, these models are insufficient to predict credit risk for commercial applications.

