<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Sharks vs Dragons

*Group project, week 3*
*Imogen, Julia, Anton*

*August 2020 cohort, Berlin, 28.08.20*

## Content
- [Project Description](#project-description)
- [Questions & Hypotheses](#questions-hypotheses)
- [Dataset](#dataset)
- [Database](#database)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)

## Project Description

We decided to examine data from the reality TV show franchises 'Dragon's Den' (UK) and 'Shark Tank' (USA). In the show, entrepreneurs pitch business ideas or businesses to a panel of investors (referred to as 'Dragons' or 'Sharks', respectively), and the investors then decide whether to invest in the company. We were interested in comparing the two franchises to look for points of commonality and difference. 


## Questions & Hypotheses

The aim of the project at hand is to merge different datasets and to prepare them for a deeper data analysis on the differences and similarities between Shark Tank US and Dragon's Den UK.

The following questions are to be addressed:
1. What number of episodes exist in total and per season?
2. What are the top ten overall products with the highest valuation and how can they be categorized?
3. What is the av. valuation per company?

## Dataset

We were able to locate two suitable datasets in csv form for the American franchise, Shark Tank. However, we could not locate a suitable dataset for Dragon's Den, and therefore had to use web scraping to access comparable information. 

The project dataset was obtained through directly downloading raw data as well as webscraping:

**dataset_1: shark_tank.csv as "shark_ent" (shark entrepreneurs)**  
- download of raw data  
Link: https://www.kaggle.com/rahulsathyajit/shark-tank-pitches  
Source:www.kaggle.com  
Last edited: 2017  
Last accessed: 28 Aug 2020

**dataset_2: shark_deals.csv as "shark_inv" (shark investors)**  
- download of raw data  
Link: https://www.kaggle.com/neiljs/all-shark-tank-us-pitches-deals  
Source: www.kaggle.com   
Last edited: 2017  
Last accessed: 27 Aug 2020  

**dataset_3: dragons_den.csv**  
- webscraping  
Link:https://en.wikipedia.org/wiki/Dragons'_Den_(British_TV_programme)#Statistics   
Source: www.wikipedia.org  
Last edited: 23 Aug 2020  
Last accessed: 27 Aug 2020  


## Database

Dataset_1 and dataset_2 focus on Shark Tank US, while dataset_3 focuses on Dragon's Den UK.

While dataset_1 focuses more on shark entrepreneurs, dataset_2 has additional information on shark investors.
The datasets are merged on shark investors on the product name, taking dataset_2 as a base.

Dataset_3 was obtained for comparison through webscrapping data present in similar form in the merge of dataset_1 and dataset_2.


## Workflow

First we decided on our topic and began a broad search for data. We compared various data sources found, before deciding to use two csv files on Shark Tank. Julia and Imogen merged those two datasets and cleaned them, while Anton webscraped the Wikipedia page on Dragon's Den. We then examined our datasets and began to conduct small analyses on them. 

**Cleaning the merged Shark Tank dataset involved the following methods:**
- Improved column names
- Changed values in columns
- Reduced missing values
- Removed duplicate columns
- Fixed incorrect data types
- Reset index


## Organization

We created a kanban board on Trello to organise and coordinate work among ourselves. That way, we could distinguish between tasks that needed to be done and tasks that would be nice to have if time permits. The kanban board also allowed us to assign tasks to one or more of us, making it easier to keep track of who was doing what. 

Our repository contains the following files:
- this README file
- csv files:
    - dataset_1: dataset_1_shark_ent.csv (shark entrepreneurs)
    - dataset_2: dataset_2_shark_inv.csv (shark investors)
    - dataset_3 (webscraped dataset on dragons den): dataset_3_dragons_den.csv.csv
    - dataset_4 (merged shark datasets): dataset_4_shark_merged.csv
    - dataset_5 (cleaned shark dataset_4): dataset_5_shark_merged_clean.csv
- jupyter notebook files:
    - jupyter file_1 (merging 2 shark tank datasets): jn_1_shark_merged.ipynb
    - jupyter file_2 (cleaning the merged shark tank dataset): jn_2_shark_merged_cleaning.ipynb
    - jupyter file_3 (webscraping Dragon's Den dataset):  jn_3_dragon_web_scraping.ipynb
    - jupyter file_4 (start of analysis of data): jn_4_descriptive_statistics.ipynb


## Links

[Repository](https://github.com/fctonio/Shark_vs_dragons)  

[Trello](https://trello.com/b/HXCiA8Xj/sharks-vs-dragons)
