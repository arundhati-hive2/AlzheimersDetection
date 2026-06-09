# AlzheimersDetection
This project uses the 'OASIS Cross-Sectional MRI dataset' from kaggle to build a binary classifier that distinguishes between (class 0) demented and (class 1) non-demented individuals.

Dataset: (https://www.kaggle.com/datasets/jboysen/mri-and-alzheimers)
150 subjects, 12 features
CDR was excluded to avoid data leakage


COLUMN - DESCRIPTION 
- ID - Subject identifier 
- M/F - Gender 
- Hand - Handedness 
- Age - Age in years 
- Educ - Years of education 
- SES - Socioeconomic status (1–5) 
- MMSE - Mini-Mental State Exam score (0–30) 
- CDR - Clinical Dementia Rating 
- eTIV - Estimated Total Intracranial Volume 
- nWBV - Normalized Whole Brain Volume 
- ASF - Atlas Scaling Factor 
- Delay - Gap between scan sessions (mostly empty) 

Approach:
- KNN for missing values
- SMOTE for class balancing
- Compared Logistic Regression, Random Forest, SVM, Gradient Boosting
- Random Forest was the best model

Key Finding: nWBV and MMSE are the strongest predictors
