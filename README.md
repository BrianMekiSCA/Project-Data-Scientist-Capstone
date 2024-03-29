

# Project Motivation
1. The main objective of this project is to create a method that can be used to predict a prognosis given a set of symptoms.
It is easy to see how such a tool could be valuable in the medical field where time is of the essence and precision is literally a matter of life and death

# Libraries Employed
The entire project was conducted with the aid of the following libraries:
* import networkx as nx
* import matplotlib.pyplot as plt
* import pandas as pd
* from sklearn.feature_selection import mutual_info_regression
* import numpy as np
* import seaborn as sns
* from sklearn.model_selection import train_test_split
* from sklearn.linear_model import LogisticRegression
* from sklearn.metrics import accuracy_score
* from sklearn.metrics import confusion_matrix

# Data, Wrangling and Cleaning
The data for this mission is called "Disease Prediction Data" and is sourced from https://www.kaggle.com/datasets/marslinoedward/disease-prediction-data (Edward, M. (Owner). (2024, Jan)). The data comprises 134 columns in total. 132 of these provide symptom data, 1 column comprises 42 diseases and is therefore the target variable and the last column is an unnamed variable. 
The data is originally split into the training and test sets.
Part of the cleaning process involved removing the unnamed variable and isolating the explanatory inputs from the response variable.
 
# Data Analysis
This portion began with analyzing the input data to check if the response variable was balanced and to understand the explanatory variables in terms of relative presence/absence of the symptoms among the cases studied.

# Train and Test Logistic Model
Next, a logistic regression was fit to the training set and evaluated on the test set mainly using the accuracy score to give the general performance measure of the model

# Results Interpretation
Both in-sample and out-of sample tests prove the model "perfect" for the data that it was presented. However, this analyst is aware that this outcome is almost taboo as it is possibly that the model could underperform were it presented with a more realistic dataset.

# Conclusion
According to the model, it is likely that if a logistic regression were fit to data comprising symptoms of known ailments then the underlying disease could potentially be well predicted given sufficiently adequate input. 

# Supporting Material
The entirity of the project can be found on Github in repo: https://github.com/BrianMekiSCA/Project-Data-Scientist-Capstone
The reader can also find a write-up of the project at https://medium.com/@brian.meki/life-or-death-aaa8e42dac6b
A collection of files is accompanies this project. These include:
* copies of training and test Disease Prediction Data in CSV format,
* plot outputs showing
* - proportions of diseases in the responce variable,
  - proprtions of presence/absence of symptoms
  - plot and datatable showing impact of each variable on the diagnostic outcome
  - and a confusion matrix from the evaluation of the model are included as well.
