### Table of Contents

1. [Introduction](#introduction)
1. [Contents](#contents)
2. [Installation](#installation)
3. [Project Motivation](#motivation)
4. [Project Definition](#definiton)
5. [Project Analysis](#analysis)
6. [Project Conclusions](#conclusions)
7. [Observations](#observations)
8. [Licensing, Authors, and Acknowledgements](#licensing)

## Introduction <a name="introduction"></a>

The work presented here is the capstone project for Udacity's Data Scientist Nanodegree Program. And so, I saw that
as an opportunity to put my data scientist skills to the test by tackling a problem that would not just testing my
knowledge of the tools used to work with data, but also challenge my capacity to create a method for understanding 
and dealing with data.

The project consists of an exploratory study on Machine Learning predictive models using Starbucks's data.

An article for this project was written and published on Medium on the following url:
https://higorpr.medium.com/an-exploratory-study-on-machine-learning-models-the-starbucks-case-study-660c02a4f2b7

## Contents <a name="contents"></a>

This project's main folder contains:
- data (folder): folder containing the data sets provided by Starbucks and where some files assembled throughout
the notebook execution are stored;
- Starbucks_Project_rev_A (Jupyter notebook): notebook holding the code and markdowns for the development process
of the predictive model.

The files in the data folder are:
- portfolio (json file): data set containing information about Starbuck's offers;
- profile (json file): data set containing information about the customers;
- transcript (json file): data set containing information about the transactions and offers status.

## Installation <a name="installation"></a>

In order to run the cells in the notebook, it is necessary to previously install the following packages:
- matplotlib
- numpy
- pandas
- sklearn
- seaborn

These packages can be installed by entering the following code on the terminal:
"pip install *package_name*" 

Where "package_name" is the package to be installed.

The code should run with no issues using Python versions 3.*.

## Project Motivation <a name="motivation"></a>

Among the themes presented by Udacity, the one that caught my attention was the Starbucks Project. That choice was
based on the belief that the project, as presented by Udacity, would be complex enough for me to combine the need
I felt for improving my data wrangling skills and my curiosity on the performance of some Machine Learning methods 
provided by Sklearn's library.

## Project Definition <a name="definition"></a>

The data set provided to me contained simulated data that mimics customer behavior on the Starbucks mobile app. 
Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement
(informational offer) for a drink or an actual offer such as a discount or BOGO (buy one get one free). 
Some users might not receive any offer during certain weeks. 

The project consisted in combining transactions, customer demographic and offer data to determine which demographic 
groups best responds to each offer.

Every offer has a validity period before the offer expires. It is assumed that this is the period in which the 
customer is feeling the influence of the offer. 

The data provided by Starbucks consisted on transactional data showing user purchases made on the app including 
the timestamp of purchase and the amount of money spent on a purchase. This transactional data also has a record 
for each offer that a user receives as well as a record for when a user actually views the offer. There are also 
records for when a user completes an offer. 

It is important to mention that purchases could be made using the app without having received or viewed an offer.

An offer is successful if a customer receives, views and completes it in the validity period.

The expected result of this project is the creation of a prediction model using Sklearn: Given a customer demographic 
(sex, age and income range and time as a Starbucks member), which offers are most likely to be completed?

## Project Analysis <a name="analysis"></a>

This project covered all the steps for the building of a predictive model:
- Data Examination;
- Data Wrangling and Visualization;
- Pre-processing of Machine Learning model data;
- Definition of performance metrics;
- Comparison of differente prediction models;
- Optimization of model's hyperparameters;
- Creation of user friendly function for prediction using the chosen classification model.

## Project Conclusions <a name="conclusions"></a>

The conclusions obtained from the data provided by Starbucks after the process of data wrangling:
- The most completed offers in absolute numbers were Discount and BOGO;
- The age range which offers are less effective is between 18 and 40 years old;
- Men tend to complete less offers than women;
- Offers are less effective for customers in the lowest income range;

Concerning the Machine Learning model, the conclusions obtained were:
- The best results for the performance metrics of the classification problem came from Ensemble methods;
- In general, linear model and SVM classifiers did not perform well;
- The process of optimization of hyperparameters using GridSearchCV did not have a major influence on the chosen
performance metrics.

## Observations<a name="observations"></a>

Possible improvements for this project is the implementation of neural networks for the classification model creation 
and later comparison against the prediction models provided by Sklearn methods.

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Credits to Starbucks for the data, without it this project would have not been possible.

## Author: Higor Pêgas Rosa de Faria
=======
