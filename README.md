# Diabetes_Prediction
Developing predictive models to forecast diabetes 

The goal of this project is to build a model that identifies patients that have a diagnosis of Type 2 diabetes mellitus (T2DM). Diagnosis of T2DM is defined by a set of ICD9 codes: {'250', '250.0', 250.0, and 250.2} where 250.0 means '250.00', '250.10', '250.20', ... '250.90' and 250.2 means '250.02', '250.12', ... '250.92'.

Note that ICD9 codes 250.1 and 250.3 are for Type I diabetes mellitus and are not to be classified. ICD9 codes are found in the table SyncDiagnosis.

The datasetPracticeFusionDiabetes consist of 17 different files, 2 common files and 15 data set-specific files. They are in comma separated value (csv) format. Please refer to the data set dictionary for a description of the table elements and for a chart showing how the tables are connected.

There are a total of 9,948 patients in the data. The training set comprises 6,600 patients. The file training_SyncPatient.csv has an indicator column to show who has a diagnosis of Type 2 diabetes mellitus (T2DM). Use training data to do exploratory data analysis (distribution for diabetes based on male/female, smoking/non-smoking, age, and other data). Build a predictive model to forecast diabetes given the details of a patient in the same format as training_SyncPatient.csv. You will test the efficacy of your predictive model using test_SyncPatient.csv and output a file test_SyncPatientForecast.csv with a new column DMIndicatorForecast probability for each row. The format of the input file test_SyncPatient.csv is: PatientGuid Gender YearOfBirth State PracticeGuid The format of the ouput file test_SyncPatientForecast.csv is: PatientGuid DMIndicatorForecast Your model performance is going to be evaluated using the Brier score (https://en.wikipedia.org/wiki/Brier_scoreLinks to an external site.) that compares your T2DM probability with T2DM actual.
