# HealthCare: Diabetes

Application of machine learning to some publicly available healthcare data.

This dataset is a part of original larger dataset from the National Institute of Diabetes and Digestive and Kidney Diseases.
Here the objective is to predict whether a patient has diabetes based on diagnostic measurements

Several constraints were placed on the selection of these instances from a larger database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.

    Pregnancies: Number of times pregnant
    Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
    BloodPressure: Diastolic blood pressure (mm Hg)
    SkinThickness: Triceps skin fold thickness (mm)
    Insulin: 2-Hour serum insulin (mu U/ml)
    BMI: Body mass index (weight in kg/(height in m)^2)
    DiabetesPedigreeFunction: Diabetes pedigree function
    Age: Age (years)
    Outcome: Class variable (0 or 1)

Number of Instances: 768
Number of Attributes: 8 plus class
For Each Attribute: (all numeric-valued)

# Explorative data analysis
All the features have no missing values.
the distribution of all the features looks like this:-
![histograms](images/histogram.png)

# Creation of additional features

https://www.medicinenet.com/what_is_a_high_insulin_level/article.htm#what_are_normal_insulin_levels  
Based on normal insulin level (16 - 166 mIU/L) three addition class of insulin as low, normal and high were created.

# Model Selection
First I compared seven classification models to find the top three performers. 

Then I tuned these best models using GridSearchCV to find the best model.
I also compared the models before tuning and after tuning.
