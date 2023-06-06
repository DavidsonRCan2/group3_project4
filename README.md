# group3_project4

## Introduction
One of the most common cancers around the world is lung cancer. Since symptoms 
for lung cancer are similar to other prevalent respiratory diseases, detection and 
treatment rely heavily on image analysis and manual testing mechanisms. This 
poses several issues because only highly trained personnel are qualified to provide
a diagnosis, limiting the amount of people able to give an accurate result and 
results are subject to human error. To limit the risk of human error in lung cancer 
diagnosis we propose to create a model that is able to assess a variety of symptoms
and determine if the patient is at high, medium, or low risk of developing lung 
cancer. This model will be trained using a csv containing 1,000 patients with a range 
of ages and symptoms presenting a level of high, medium, or low risk of lung cancer
development. 

## Tableau
![image](https://github.com/DavidsonRCan2/group3_project4/assets/119651909/1c96f1f1-c5b3-41a6-a712-dcc6875eb429)
![image](https://github.com/DavidsonRCan2/group3_project4/assets/119651909/efe37e62-3596-4324-9095-27354c92546a)

## Data Cleaning
- Changed Low, Medium, and High classification level to 1, 2, 3
- Ran .corrwith() to look for correlations between symptoms and classification level
- Excluded symptoms with <30% correlation, accounted for 6 out of 23 symptoms and environmental exposures

## Unsupervised Machine Learning 
- We conducted principle component analysis to obtain the most relavent symptoms and factors that contribute to lung cancer risk. We then ran a logistic regression model with the 6 principle components that were produced by the PCA.
![image](https://github.com/DavidsonRCan2/group3_project4/assets/119651909/c5d1e560-f2a8-4273-9a45-9a99f6d8f61c)
- We ran the same components through a RandomForest model

![image](https://github.com/DavidsonRCan2/group3_project4/assets/119651909/a7737720-ac73-4e0c-a7ff-327b79e69b39)

## Supervised Learning 
- We then ran the full dataset through 
Logistic Regression
![image](https://github.com/DavidsonRCan2/group3_project4/assets/119651909/a3147994-9888-4778-a725-f5461ae06735)

RandomForest
![image](https://github.com/DavidsonRCan2/group3_project4/assets/119651909/96169880-13d8-4992-b5ec-3632c035242c)

KNN
![image](https://github.com/DavidsonRCan2/group3_project4/assets/119651909/1f3a1715-dac2-444c-8eee-b8f90beef36f)

## Summary
Based on the results we determined that the RandomForest and KNN models performed extremely well. We recognize the nature of our dataset and hypothesize that these perfect results may result from alterations done to the dataset previously to train a different model. 









