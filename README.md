# Flight Price Predictor 

# Introduction

## What do we hope to achieve? 
The goal of this project is to answer several questions based on the databases we are working with in regard to flight travel data. Essentially, we want to be able to predict how much a flight will be based on several different factors. This could be based on the following: 
 - Starting City 
 - Destination City 
 - Departure Date 
 - Return Date 

The idea is to build our machine learning model to test against these factors in order to come to an answer based on the input. 

## Data Sources 

https://www.kaggle.com/datasets/dilwong/flightprices

https://www.bts.gov/browse-statistical-products-and-data


# Role Assignments For our Project 

## Role Assignment:

- ReadMe in Github @ Turner
- Machine Learning @ Travis
- Cleaning Data @ Nick
- Visualizations via Tableau @ Allie
- Presentation @ Max

# Segment 1 Deliverable: Data Cleaning and Presentation
- Content 
  - Clean data by eliminating unnecessary columns (legID, fairBasisCode, elapsed Days, baseFare, seatsRemaining, 'segment' columns)
  
  <img width="759" alt="image" src="https://user-images.githubusercontent.com/115503996/227391808-63d52e99-54b9-45ab-b7f7-6c5537369fc5.png">
  
   - creation of a new column named: "searchDaysBeforeFlight"
   
   <img width="764" alt="image" src="https://user-images.githubusercontent.com/115503996/227392089-173f9715-1d07-4e85-ad31-37eaa354d9c3.png">

   - store the five files into dataframes, convert to csv and merge into one dataframe
   
   <img width="763" alt="image" src="https://user-images.githubusercontent.com/115503996/227392359-7ca0f796-a608-4a46-bdc2-310d574273da.png">
  
  - Creation of one stored data table 
  
  <img width="769" alt="image" src="https://user-images.githubusercontent.com/115503996/227392600-849a18c6-5627-4261-ba84-51444c6dd870.png">

- Presentation (See Answers above in the Introduction)
  - Selected topic and reasoning behind the selection 
  - A description of the data 
  - Question(s) we plan to answer 
  
# Segment 2 Deliverable: Machine Learning
- Content 
  - Machine learning model with a confusion matrix and accuracy score 
- Presentation 
  - Description of data exploration 
  - Technologies, languages, tools and algorithms that the team used throughout the project
