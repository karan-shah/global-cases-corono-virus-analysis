# COVID-19 Data Analysis

This repository contains data analysis of COVID-19.

# Table Of Contents
  - [Team Members:](#team-members)
  - [Objective](#objective)
  - [Project Introduction](#project-introduction)
  - [Data and Domain](#data-and-domain)

### Team Members:
  1. Karan Hirenkumar Shah (kshah51@uncc.edu)
  2. Sarang Suhas Padalkar (spadalka@uncc.edu)
  3. Abhishek Tanwer (atanwer@uncc.edu)
  4. Janhvi Chitnis (jchitnis@uncc.edu)
  5. Kruti Raval (kraval@uncc.edu)

## Objective: 
Create awareness about the Corona Virus Disease(COVID-19) and understand in an easier manner the people affected and other attributes related to the disease with the help of data analysis.

We'll try to answer the following questions:
*	Who are most affected by COVID -19? (age, gender, class.. etc)
*	Which country contains majority of patients?
*	How many of these affected patients have traveled to Wuhan?
*	Do all the affected patients show same symptoms (age, gender, class.. etc)?
*	What is the impact of the COVID-19 (Death vs Recovery of paitents )?

## Project Introduction:
From the World Health Organization - On 31 December 2019, WHO was alerted to several cases of pneumonia in Wuhan City, Hubei Province of China. The virus did not match any other known virus. This raised concern because when a virus is new, we do not know how it affects people. So daily level information on the affected people can give some interesting insights when it is made available to the broader data science community. Johns Hopkins University has made an excellent dashboard using the affected cases data. Data is extracted from the google sheets associated and made available.

## Data and Domain:
2019 Novel Coronavirus (2019-nCoV) is a virus (more specifically, a coronavirus) identified as the cause of an outbreak of respiratory illness first detected in Wuhan, China. Early on, many of the patients in the outbreak in Wuhan, China reportedly had some link to a large seafood and animal market, suggesting animal-to-person spread. However, a growing number of patients reportedly have not had exposure to animal markets, indicating person-to-person spread is occurring. At this time, it’s unclear how easily or sustainably this virus is spreading between people.

* **Source Description** 
    
    The dataset is acquired from [Kaggle](https://www.kaggle.com/). Kaggle is a subsidiary of Google LLC, is an online community of data scientists and machine learning practitioners.
  
* **Data Description**
    
    Dataset Link- [COVID-19 Dataset](https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset#COVID19_open_line_list.csv)

    There are mainly 6 different files are provided. Main file in this dataset is [covid_19_data.csv](https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset#covid_19_data.csv). Other three files contains the list of confirmed, recovered and death cases on a perticular day in various countries. This dataset contains data from 22nd January, 2020 to 14th March, 2020 as of now. There are some empty attributes and missing values in the dataset so data preprocessing is required. The dataset contains 57 attributes and approaximately 20,000 records. Main data file attributes description is as follows:

    * Sno - Serial number
    * ObservationDate - Date of the observation in MM/DD/YYYY
    * Province/State - Province or state of the observation (Could be empty when missing)
    * Country/Region - Country of observation
    * Last Update - Time in UTC at which the row is updated for the given province or country. (Not standardised and so please clean before using it)
    * Confirmed - Cumulative number of confirmed cases till that date
    * Deaths - Cumulative number of of deaths till that date
    * Recovered - Cumulative number of recovered cases till that date
 

* **Tentative plan for analysis on GCP**

    1. EDA and Data Preprocessing
    2. GCP Dashboard
    3. Machine Learning on GCP
    4. Evaluation of results



