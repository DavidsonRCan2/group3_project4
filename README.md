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
- Excluded symptoms with <30% correlation, accounted for 6 out of 23 symptoms and environmental exposures.








