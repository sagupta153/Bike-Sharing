# Bike Sharing Assignment - by Sankalp Gupta
> This assignment is about developing a linear regression model to predict the demand for bikes on rental for a bike-sharing company, which has completed 2 years of business

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- Assignment Obective: To build a linear model to predict expected bike-rentals
- Data-set: Containing daily records of 1st 2 years of business. Total 730 records - 365 for each year
- Each record had the following information
- 1. Temperature: 2 columns - temp and atemp - actual temperature and feeling temperature
- 2. Information about the day: 4 columns - date, weekday number, a flag indicating whether its a holiday, a flag indicating whether its a working day
- 3. Weather information: 2 columns - season (4 seasons), weathersit (4 weather situations)
- 4. Daily Rentals: 3 columns - cnt (total rentals), registered (rentals by registered users), casual (rentals by casual users)

## Conclusions
> A preliminary visual analysis revealed a lot of inter-dependency among some variables. This was expected, as can be seen from the groupings made above
> While modelling, these inter-dependencies came up as high VIF values
> A total of 3 models were made
> Best Model Fit has the following features
- 1. The model is: No. of Rentals = 2042 * yr - 623 * holiday + 134 * workingday + 130 * atemp + 794 * summer + 1227 * winter - 2408 * light-snow - 677 * misty + 510 * Aug + 969 * Sep

- 2. The results of the regression indicated that 7 predictors explained 97% of the variance. These are: year, holiday, working day, feeling temperature, season (summer / winter), weather situation (light snow / misty) and month (Aug / Sep)

> The main features are:
- 1. Working day: Generally rentals are more on working days compared to holidays or weekends 
- 2. Temperature: Generally rentals are higher on days with higher temperatures
- 3. Weather Situation: Clear Days are the best for bike rentals
- 4. Year of operation: 1st year was low in business, but business in 2nd year was quite high.


## Technologies Used
- operating system - microsoft windows - version Windows 11 Home edition
- programming language - python 3 - version 3.9.7 
- jupyter notebook - version 6.4.5
- pandas library - version 1.3.4
- numpy library - version 1.20.3
- matplotlib library - version 3.4.3
- seaborn library - version 0.11.2
- statsmodels library - version 0.12.2
- scipy library - version 1.7.1
- sklearn library - version 0.24.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by Bike Sharing Assignment in Machine Learning 1 course
- References : Bike Sharing Assignment, Module-2, Machine Learning Course-1, as a part of PG course in AI & ML by IIITB and upGrad
- This project was based on [Machine Learning-1](https://learn.upgrad.com/course/1994/segment/13375/109590/331557/1723023).


## Contact
Created by [@sagupta153] - feel free to contact me!