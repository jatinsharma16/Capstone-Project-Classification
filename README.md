# Capstone-Project-Classification
Cardiovascular risk prediction is really important for any patient who might get affected due by this problem, therefore it becomes a major concern to detect the risk beforehand to provide suitable treatment to the patient and prevent any major problems.
The data that we are provided is from an ongoing study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients' information. It includes over 3,000 records and 15 attributes. Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk factors.
To prevent the patient from any major problem, it becomes a priority to detect any problem and tackle the same before it is too late to take any action which in turn helps the doctors or the hospitals to reduce the mortality rate and provide better treatment to the patient. This helps hospitals to build a good relationship with the patients and many lives are also saved.

Some of the insights that we derived from the data are 
- Out of all the patients, only 15.1% of patients have the risk of CHD.
- Analyzing the age of the patients, patients aged 35 to 70 face the risk of CHD. Analyzing the data with respect to sex shows us that both males and females are equally at risk of CHD despite the age factor.
- Analyzing the sex factor shows us that although more female patients are there, the number of patients affected by CHD is higher among males.
- Talking about education, we found that the number of patients decreases as the education level increases. The knowledge about having a healthy lifestyle can be the reason behind this.
- Among the patients, the ratio of people who smoke and do not smoke is 50-50. Also analyzing the patients with risk shows that smoking does not have any prominent effect on the CHD risk.
- Analyzing the column of BPMeds shows us that although BP medicines do not show any visible effect on the CHD risk but columns like prevalent stroke, hypertension, and diabetes show that they affect the CHD risk up to an extent.
- Talking about total cholesterol, sysBP, and diaBP they all show an increased trend in the values for those who are affected by the CHD risk.
- The same trend is shown by the columns like BMI, heart rate, and glucose.
- Finally analyzing the correlation heat map, we can see that age, hypertension, diabetes, sysBP, diaBP, and glucose are some of the most prominent variables contributing to the value of the dependent column.

Since the dataset was highly imbalanced therefore we made use of SMOTE (Synthetic Minority Oversampling Technique) to handle the class imbalance. Although we were not getting desired results initially but after using SMOTE, we were able to make models that gave acceptable results. The best result we got was obtained by making the use of XGBoost model, which is an Extreme Gradient Boosting algorithm. After performing multiple iterations of hyperparameter tuning over the XGBoost, the best result we obtained was 90% for precision, recall as well as f1 score, although the recall for the positive class is 93%.
