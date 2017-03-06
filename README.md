README.md
====================

# Titanic data inverstigation

During the Titanic disaster, who is the lucky one, which feature(s) may lead to higher survival rate?

The dataset is downloaded from Kaggle competetion, with **"train.csv"** and **"test.csv"**. 

First I did exploratory data analysis for the training data, as shown in **EDA_Titanic.ipynb**, then in order to user machine learning to make the prediction of the survival, in **Titanic_ML.ipynb**, I used Decisiontree, randomForest, and svc to make the prediction. 

## Prediction files##
my_solution_one.csv: Decisiontree
my_solution_two.csv: Decisiontree with more features included in the training
my_solution_three.csv: Decisiontree after creating one freature: Family size
my_solution_four.csv: Randomforest for the prediction
my_solution_svc.csv: Use SVC for the prediction

## Draw ##
An interactive figure was made with Dimple.js, to show the survival rate with cabinet class.

According to the analysis, cabinet class, sex, Age and Fare are the most important features for the survival during the disaster.
