# Write a DataScience Blog Project

## Project Motivation
> I have selected <b>Covid-19 Dataset</b> for this project. This virus is one of the dangerous virus which stopped the whole world. So, I was wanting to see how it is effecting the countries and how well each of the countries are doing to contain this virus. I am doing two types of analysis : descriptive analysis and Machine Learning model(forecast the number of deaths). 

### Dataset Used:
> I have used two dataset owid-covid-data.csv and full_data csv. The first "owid" consists of the testing numbers of the countries and second full_date consists of the new cases and new deaths all over the world.The dataset was downloaded from https://ourworldindata.org/coronavirus-testing and kaggle.com.


## Description of Repository:
> This github repo consists of three files. They are:

#### DataScienceProject.pynb
> This python file consists of the analysis on the data(owid-covid-data.csv). I have used pandas,groupby for the analysis.

#### forecast.pynb
> This python file consists of the forecast of new_cases data in the file full_data csv. I have used ARIMA methodology to predict the new_cases specific to <b>USA</b>.

## Libraries used:
> I have used python to code.
> The libraries used are: Pandas, Numpy, Matplotlib.

The pandas are dataframe which is easy to perform analysis on dataset. This gives flexibility similar to write queries as SQL to manipulate the data.
I have used numpy to replace 0 with np.nan in order to drop those values.


## Methodology:

For this project, I followed the CRISP-DM methodology. They are explained below:

The project is divided into 6 phases based on CRISP-DM.

<b> i. Phase 1 - Business Understanding </b>
    In this phase, I decided on the questions that i need answers for. I knew the problem type were descriptive and forecasting. The questions formulated were:
       1. <b> Top 10 Countries with highest no of Cases </b>
       2. <b> Top 10 Countries with highest no of deaths </b>
       3. <b> Top 10 Countries with highest no of Tests </b>
       4. <b> New Zealand's Strategy </b>
       5. <b> Forecast for No of Casees </b>
    
 <b> ii. Phase 2 - Data Understanding & Phase 3 - Data Preparation </b>   
     In this phase, I used describe() and corr() methods to understand the datasets. I found there was strong correlation between the features. The dataset didnt consists of high number of NaNs.Although, there were 0's in the dataset.There were no categorical features so i didnt have to do one hot encoding. I removed the NaNs if there were any as it would effect the execution time. The final dataset for both csvs (owid-covid-data) and (finaldata.csv) were clean and didnt have to do lot of manipulation. Hence, I have mixed the phase 3 and phase 3. As my analysis specific to countries and to a certain features, NaNs in other fields didnt effect as well.However, for New Zealand and USA, i created a separate dataframe, to perform the analysis and Modeling.The date field were intially object so used datetime to convert them into date format for easy analysis.
      
<b> iii. Phase 4 - Modeling </b>
    As for the first file datascienceproject.pynb, the analysis was descriptive,I have used group by and plotted column charts to see the 10 countries in terms of new_cases, new_deaths and new_tests. I used groupby on New Zealand's data to see how many tests they were performing on per day basis. For the second file, I have used ARIMA model to perform the time series forecasting.I limited the country to USA and performed forescast on the new_cases features.
    
 <b> iv. Phase 5 - Evaluation </b>
   I evaluated my forecast model based on the graph. In the initial phase, the model didnt do very well, however it has predicted less new_cases going forward which is actually happening. The questions asked were answered through the analysis. However, I would dig dipper into the data in future to get more clarity.
   
 <b> v. Phase 6 -  Deployment </b>
  I have blogged about the result set on medium and posted on github as well.I will improve further after getting feedback from people and follow the CRISP-DM process to implement any changes going further.
  
 ###  Results
 
 >This Project demostrates the countries suffering from this virus. The 10 most virus infected countries.I have also analyzed the dataset for New Zealand where there is only 1 active cases and seen their testing. I wanted to see how some countries are doing really good interms of controlling and some countries are not able to contain. USA is currently the top and New Zealand is in the lowest.I have used basic analysis and seen the top 10 countries in terms of the new cases and new deaths. I have also attempted to perform a time series forecast using ARIMA. 

>I found that USA is in the top list in terms of the virus and the major reason is the no of tests being conducted and the lack of strict stay at home order. New Zealand conducted the highest number of tests although their active cases were less within 5, the no of test conducted were more than 5000 per day. The lockdown was done more strictly and in the very beginning phase. That is the reason, New Zealand is a successful story. Overall, I found that although USA has highest number of tests, it is not implementing strict lockdowns as Italy or New Zealand, that is one of the major reason, the number of cases and deaths is higher than any other country.




