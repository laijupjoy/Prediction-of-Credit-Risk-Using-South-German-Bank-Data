# Prediction of Credit Risk Using South German Bank-Data

## Table of Content
- Introduction
- Approach
- User Interface
- Deployment Link
- File Structure
- Installation
- Technology Used
- Document

## Introduction

When a bank receives a loan application the bank has to make a decision regarding whether to go ahead with the loan approval or not. 
The bank makes a decision on the loan based on the applicant’s profile. Bank must be able to reduce the risk of non-performing credit loans. 
The risk of providing loans can be minimized by studying patterns from existing lending data. One technique that can be used to solve this 
problem is to use data mining techniques. Data mining makes it possible to find hidden information from large data sets by way of classification.
  
**Input independent variables are:**
~~~
1. laufkont = status
2. laufzeit = duration
3. moral = credit_history
4. verw = purpose
5. hoehe = amount
6. sparkont = savings
7. beszeit = employment_duration
8. rate = installment_rate
9. famges = personal_status_sex
10. buerge = other_debtors
11. wohnzeit = present_residence
12. verm = property
13. alter = age
14. weitkred = other_installment_plans
15. wohn = housing
16. bishkred = number_credits
17. beruf = job
18. pers = people_liable
19. telef = telephone
20. gastarb = foreign_worker
~~~

**Output dependent variable:**

`1. kredit = credit_risk`

## Approach
~~~
1. Data Exploration     : Started exploring dataset using pandas,numpy,matplotlib and seaborn. 

2. Data visualization   : Ploted graphs to get insights about dependend and independed variables. 

3. Feature Selection    :  Drop few non important coloumns in dataset.

4. Feature  engineering :  Converting the categorical columns having ordinal values to Label Encoding
                           Converting the categorical columns having non-ordinal values to One Hot Encoding

5. Model Selection I    :  Trained Logistic Regression, Random Forest Classifier, Support Vector Machine, K- Nearest Neighbor and Naïve Bayes Classifier models.
                           Tested all trained models to check the accuracy and F1 score, and select higher F1 score model.
                       
6. Model Selection II   :  Performed Hyperparameter tuning using gridsearchCV in selected higher F1 score model and improve the model perfomance.

7. Pickle File          :  Selected model as per best F1 score and created pickle file using Python pickle module.

8. Webpage & deployment :  1. Created a web application that takes all the necessary inputs from user and shows output.
                           2. After Create we application, We had Deploy at Heroku Platform
                           3. And after We had deployed project on AWS Elastic elastic beanstalk.
~~~

## Web Application User Interface:

The Prediction of Bank Credit Risk Final Model Run in Local Enviornment

1. Home Page :

![Resources](bank1.png)

2. Result Page :

![Resources](bank2.png)

## Deployment Link

Heroku Link :

Heroku Link For Data Report : 

AWS Link : http:

AWS Link For Data Report :

## File Structure
~~~
Project
|
|
|
application_logging--|--logger.py
|
|
|
database_coonection--|
|                    |--Database.py
|                            
|
SouthGermanCredit--------------|
|                              |---codeable.txt
|                              |---Databse Credit.csv
|                              |---Final_Model.csv
|                              |---Preprocess.csv
|                              |---read_SouthGermanCredit.R
|                              |---SouthGermanCredit.asc
|
|logFiles----------------------|--application.log
|                              |--Database.log
|
|
templates----------------------|  
|                              |---index.html
|                              |---result.html
|                              |---German_Credit_Data.html
|venv
|
|app.py
|
|Credit_Data_RF.pkl
|
|Procfile
|
|requirements.txt
|
|runtime.txt
|
|
|secure-coonect-energyefficiency.zip
~~~

## Installtion
The Code is written in Python 3.6. If you don't have Python installed you can find it [your link here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) the repository.

~~~
Create a Virtual Env with conda create "Your Env name"
~~~
~~~
pip install -r requirements.txt
~~~
~~~
Run app.py file
~~~

## Technology Used
~~~
1. Python
2. Sklearn
3. Pandas
4. Numpy
5. Flask
6. HTML
7. CSS
8. Cassendra
9. AWS
10. Heroku
~~~

## Document
Below providing the link of all the document that are required for creating the project.

Link: [Document Link]()
