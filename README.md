# Investigating Bias in Insurance Premium Prediction

As the importance of data collection and interpretation has been proven in the past decade, more and more companies, organizations, 
and government branches have invented and deployed the ADS (automated decision-making system) to assist them 
to make decisions under various scenarios. However, the discussion of these ADS applications also arises, 
arguing such a technique is constantly bringing unfairness into production which exerts a negative impact on society from various angles. 

The ADS focused in this project aims to use customers past medical expenses 
and their features such as sex, age, BMI, and etc. to predict their future expenses, 
ultimately to help insurance companies make decisions on premium charges. 
The purpose of this project is to investigate the methodology and implementation of the ADS and 
assess whether there exists bias where the system favors one group over another unfairly, 
such as charging a particular group with the same feature values over another group.

# Data
The data we used can be found here [here](https://www.kaggle.com/noordeen/insurance-premium-prediction). This dataset contains 1338 samples and 7 features. Four of the features are numerical including age, BMI, children, and expenses. Three of the features are nominal including sex, smoker, and region. The goal of this system is to analyze the relationship between different features and how they impact medical expenses, in order to help insurance companies compute predicted medical expenses in the future and price their premiums accordingly. 

# ADS
The code we will be analyzing for this project is found [here](https://www.kaggle.com/klmsathishkumar/predicting-insurance-premium). The code implemented several different machine learning algorithms but ultimately suggested the Random Forest model as it gave the best accuracy. Thus, we will be focusing our analysis on the potential bias given by the chosen Random Forest model.

# notebooks
* [1_1_EDA.ipynb](https://github.com/cc6580/RDS_insurance_bias/blob/main/codes/1_1_EDA.ipynb): explores distributions of features and correlations to the target variable.
* [1_2_ADS_Implementation.ipynb](https://github.com/cc6580/RDS_insurance_bias/blob/main/codes/1_2_ADS_Implementation.ipynb): analyzes the fairness of the model by assessing its accuracy, misclassification errors, statistical fairness, and stability across privileged and unprivileged subpopulations. 
