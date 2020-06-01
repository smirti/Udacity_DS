# Udacity_DS

# Covid-19 Dataset


### This Project demostrates the countries suffering from this virus. The 10 most virus infected countries.I have also analyzed the dataset for New Zealand where there is only 1 active cases and seen their testing. I wanted to see how some countries are doing really good interms of controlling and some countries are not able to contain. USA is currently the top and New Zealand is in the lowest.

### I have used two dataset owid-covid-data and full_data csv. The first "owid" consists of the testing numbers of the countries and second full_date consists of the new cases and new deaths all over the world.The dataset was downloaded from https://ourworldindata.org/coronavirus-testing and kaggle.com. 

### I have used basic analysis and seen the top 10 countries in terms of the new cases and new deaths. I have also attempted to perform a time series forecast using ARIMA. 

### I found that USA is in the top list in terms of the virus and the major reason is the no of tests being conducted and the lack of strict stay at home order. New Zealand conducted the highest number of tests although their active cases were less within 5, the no of test conducted were more than 5000 per day. The lockdown was done more strictly and in the very beginning phase. That is the reason, New Zealand is a successful story. 

### I have used CRISP_DM methodology to work through my process. There are two python files. The DataScience python file consists of the analysis for COVID-19 and the mostly the descriptive analysis for covid-19 within countries. Overall, there are few nulls and since i restricted the date, there were 0.002 % nulls. The second python file consists of forecasting for new cases within USA. I tried to implement using CRISP-DM. I have first formulated the question and then collected the dataset. I have seen the overall data and what is the correlation between the features. I have dropped nulls where all the four fields new_cases, new_deaths, total_cases and total_deaths were null. For forecasting, I have used ARIMA model. It shows derease in the new_cases for USA. 

### The second DataScience python file, I have used group by and plotted column charts to see the 10 countries in terms of new_cases, new_deaths and new_tests. I was also interested to see the New Zealand's testing number as currently the no is zero.

### This analysis has provided my the clarity of CRISP-DM, I developed business understanding and the questions that I needed to ask.I have prepared the dataset by dropping null values. I also resctricted on the countries i was performing analysis for.  I got the answers through panda analysis and using group by method. I eveluated the method based on the internet's numbers for new_cases, new_deaths. 

### Overall, I found that although USA has highest number of tests, it is not implementing strict lockdowns as Italy or New Zealand, that is one of the major reason, the number of cases and deaths is higher than any other country.
