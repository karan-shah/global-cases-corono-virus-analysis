# COVID-19 Data Analysis

This repository contains data analysis of COVID-19.

# Table Of Contents
  - [Team Members:](#team-members)
  - [Objective](#objective)
  - [Project Introduction](#project-introduction)
  - [Data and Domain](#data-and-domain)
  - [Data Processing](#data-processing)
  - [User Dashboard](#user-dashboard)
  - [Tentative Plan for Analysis on GCP](#tentative-plan-for-analysis-on-gcp)
  - [Credits](#credits)

### Team Members:
  1. Karan Hirenkumar Shah (kshah51@uncc.edu)
  2. Sarang Suhas Padalkar (spadalka@uncc.edu)
  3. Abhishek Tanwer (atanwer@uncc.edu)
  4. Janhvi Chitnis (jchitnis@uncc.edu)
  5. Kruti Raval (kraval@uncc.edu)

## Objective: 
Create awareness about the Corona Virus Disease(COVID-19) and understand in an easier manner the people affected and other attributes related to the disease with the help of data analysis. 

This analysis can help wide range of audience such as government officials, who want to control
the spread of this pandemic diseases.

We'll try to answer the following questions:
*	Which country contains majority of patients?
*	What is the impact of the COVID-19 (Death vs Confirm of patients)?

## Project Introduction:
From the World Health Organization - On 31 December 2019, WHO was alerted to several cases of pneumonia in Wuhan City, Hubei Province of China. The virus did not match any other known virus. This raised concern because when a virus is new, we do not know how it affects people. So daily level information on the affected people can give some interesting insights when it is made available to the broader data science community. Johns Hopkins University has made an excellent dashboard using the affected cases data. Data is extracted from the google sheets associated and made available.

## Data and Domain:
2019 Novel Coronavirus (2019-nCoV) is a virus (more specifically, a coronavirus) identified as the cause of an outbreak of respiratory illness first detected in Wuhan, China. Early on, many of the patients in the outbreak in Wuhan, China reportedly had some link to a large seafood and animal market, suggesting animal-to-person spread. However, a growing number of patients reportedly have not had exposure to animal markets, indicating person-to-person spread is occurring. At this time, it’s unclear how easily or sustainably this virus is spreading between people.

* **Source Description** 
    
    The dataset is acquired from data.world(https://data.world/). Data.world is home to the world's largest collaborative data community, which is free and open for public. It is one of the platform where users can discover data and share analysis.
  
* **Data Description**
    
    Dataset Link- [COVID-19 dataset](https://data.world/covid-19-data-resource-hub/covid-19-case-counts/workspace/file?filename=COVID-19+Cases.hyper)

    This dataset contains data from 23rd January, 2020 to 5th April, 2020 as of now. There are some empty attributes and missing values in the dataset so data preprocessing is required. The dataset contains 13attributes and approaximately 5,26,200 records. Main data file attributes description is as follows:

    * case_type - Confirmed Cases and total deaths
    * cases - Point in time snapshot of to-date totals
    * country_region - Provided for all countries
    * province_state - Provided for Australia, Canada, China, Denmark, France, Netherlands, United Kingdom, United States
    * admin2 - US only - County name
    * combined_key - US only - Combination of Admin 2, State_Province, and Country_Region
    * fips - US only - 5-digit Federal Information Processing Standard
    * lat - Latitude
    * lng- Longitude
    * table_names - The Table Name is used to delineate the specific Johns Hopkins datasets that were used
    * prep_flow_runtime - Date when the ETL job ran
  
## Data Processing
  As the dataset was very clean and structured, minimal preprocessing was needed to prepare the data for machine learning. All the python code for preprocessing can be found in [Data-Preprocessing.ipynb](https://github.com/karan-shah/global-cases-corono-virus-analysis/blob/master/Data-Preprocessing.ipynb).

## User Dashboard
  ![User Dashboard](https://github.com/karan-shah/global-cases-corono-virus-analysis/blob/master/image.png)

## Tentative plan for analysis on GCP

  1. EDA and Preprocessing: Data has been already pre processed. We can directly work on it and start analysis.
  2. Dashboard for User group: We have already created a dashboard for the user group. 
  3. Machine Learning on GCP: We will use various analysis techniques offered by GCP like PySpark, BigQuery. 
  4. Evaluation of results: We will be evaluating our result by RMSE(Root Mean Square Error). The smaller the value is the accurate result will be.
  5. Production Model: We will try to develop couple of models and the best performing model will be choosen for the production model. 
  
## Credits
  
  * https://www.academia.edu/40111185/Effect_of_Noisy_Data_on_Performance_of_Machine_Learning
  
    This paper shows the impact of the noisy data. In this paper they experimented in two ways and the outcome of it is very insightful. It clearly shows that a dataset should be processed very well and there should be no noisy data like empty values or outliers etc.

  * https://www.tableau.com/covid-19-coronavirus-data-resources
   We received the data from this source. This link includes reported cases at the country level and province/state in select countries. 

  * https://github.com/CSSEGISandData/COVID-19
  
    We were inspired a lot by this repository by Johns Hopkins CSSE. He has developed some beautiful visulizations and provided various useful resource links.



