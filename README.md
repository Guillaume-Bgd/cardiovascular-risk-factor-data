# cardiovascular-risk-factor-data

Etude machine learning

28/06/2023

Exercice consistant à utiliser un dataset dans l'objectif d'entraîner différents algorithmes de machine learning.

Origine du dataset : kaggle.com "cardiovascular-risk-factor-data" : To predict the 10-year risk of future coronary heart disease (CHD) in patients 
https://www.kaggle.com/datasets/mamta1999/cardiovascular-risk-data

### Variables Description

Demographic:

Sex: male or female ("M" or "F") 

Age: Age of the patient (Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous) 

Education: The level of education of the patient (categorical values - 1,2,3,4) 


Behavioral:

is_smoking: whether or not the patient is a current smoker ("YES" or "NO") 

Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarettes, even half a cigarette.) 


Medical (history):

BP Meds: whether or not the patient was on blood pressure medication (Nominal) 

Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal) 

Prevalent Hyp: whether or not the patient was hypertensive (Nominal) 

Diabetes: whether or not the patient had diabetes (Nominal) 


Medical (current):

Tot Chol: total cholesterol level (Continuous) 

Sys BP: systolic blood pressure (Continuous) 

Dia BP: diastolic blood pressure (Continuous) 

BMI: Body Mass Index (Continuous) 

Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though in fact discrete, yet are considered continuous because of large number of possible values.) 

Glucose: glucose level (Continuous) 


Predict variable (desired target):

10-year risk of coronary heart disease CHD(binary: “1”, means “Yes”, “0” means “No”)"

### 1ere partie - préparation

import des librairies
import du dataset et pré-processing
datavisualisation rapide
split

### 2e partie - classification

LinearSVC
KNeighbors Classifier
SVC
Randomforest Classifier


### 3e partie - conclusion

Pour chaque modèle utilisé, la méthode est toujours la même :

création du modèle avec hyperparamètres par défaut
score
recherche des meilleurs hyperparamètres
optimisation du modèle
nouveau score
matrice de confusion
courbe d'apprentissage
