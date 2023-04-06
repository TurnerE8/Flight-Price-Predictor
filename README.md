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
   - Prelimenary Results 
    - Prior to running our models, we did the following:
     
     - convert 'flight date' to a number format by the day of the week and then convert that into a series using: 
       
   <img width="754" alt="conversion_to_series" src="https://user-images.githubusercontent.com/115503996/228992224-da0ffae0-819c-47eb-a1ea-55797c1b956b.png">
   
     - Based on the visualizations created in Tableau, the 'isRefundable' column was dropped: 

   <img width="755" alt="isRefundable" src="https://user-images.githubusercontent.com/115503996/228993108-837aaf2f-3866-4841-96a1-aa1cd99c8fad.png">

     - Verified that the datatypes were numeric 

  - We used two different machine learning models: 1) Linear Regression and 2) Random Forester Regressor 
   
    1) Linear Regression
     - In lieu of a confusion matrix, we looked at the metric root mean squared error - which predicts the avg. difference in price between what we were predicting versus the actual fare
     - Results: 
       - root_mean_squared error of:  145.8444780015335 
       - R-Score: .43
    2) Random Forester Regression
     - Results: 
       - root_mean_squared error of:  222.66356853100055
       - R-Score: .33
  - Based on our two initial machine learning models, utilizing the linear regression model brings us closer to the actual fare price by a margin of ~$145 dollars.

  - Coefficient/Measures of Importance based on testing (Linear/Random Forester Regression) 
  
  ![lr_coef](https://user-images.githubusercontent.com/115503996/228997182-e3025233-316a-4e5d-8725-7ce96518e6cf.png)
  
  ![Forest_Importance](https://user-images.githubusercontent.com/115503996/228997431-65367f9b-6518-4325-ac41-912551b383ac.png)

- Presentation 
  - https://docs.google.com/presentation/d/1Z56M_mGBR6sp_d1H0qI4IJTkHNKHgsX0X9bci015TuQ/edit?usp=sharing
  
# Segment 3 Deliverable: Final Presentation 
- Content 
  - We used one final machine learning model 
  
    1) 
