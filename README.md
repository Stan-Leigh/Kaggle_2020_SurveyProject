# Kaggle_2020_SurveyProject

## Introduction
The Kaggle 2020 Survey project is an analysis of the different people that work in different positions in the Technology space. This project analyzes their answers to questions posed in the survey. Questions like Which programming language would you recommend to somebody, Favourite programming language, Educational Background, Age range, e.t.c. This project demonstrates usage of plotly, a library used to make interactive visualizations.

The dataset has a little over 20000 rows and 355 columns. This project would be focused on the role column, that is, the job the respondent currently held, and how this affects or is affected by other variables in the survey.

Questions that were explored are:
* Distribution of Age groups in the survey.
* Popularity of programming languages in the survey.
* Highest level of education of survey applicants.

And a few others.

## Data Wrangling
I divided the data into columns and put it inside a dictionary. The dictionary keys were the question numbers and the values were the responses to that particular question. Some of the questions asked filled multiple columns so the values for some of the keys were DataFrames while the values for others that required just an answer was Series.

## Data Exploration
In this stage, I answered the questions posed in the introduction. I made use of plotly visuals to better depict the story the data was telling. I also added filters by role for different visualizations so that you could drill down on a visual and filter results by a specific job role.

## Conclusions
Analysis of the Kaggle Developer Survey produced a lot of interesting insights. Some of the insights garnered are listed below:
* The survey participants were mostly filled by young people within the range of 18 and 40.
* As is probably expected, Years of coding experience had a positive relationship with Age. Older people had more years of coding experience.
* **Python** is the by far the most popular programming language used in this survey, used by more than **15,000** of survey respondents. SQL comes second at almost **8,000** users.
* Most of the survey respondents have their Bachelor's Degree and even more people have gone on to get their Master's Degrees.



# Analyzing Gender and Earning Potential in Tech

## Introduction
This is a continuation of the first survey analysis. In this project, I try to answer the question of whether there is gender inequality in the Technology industry. Seeing as the survey consists of 80% male respondents and about 20% female respondents, this answer is probably Yes, but how does this affect earning potential? In this project I use machine learning models to help me answer that question.

## Data Exploration
In this stage, I answered the question posed in the introduction. I made use of plotly visuals to better depict the story the data was telling. I also used machine learning models like **OLS Linear Regression** *(used this in order to be able to see summary statistics of the model easily)*, **Lasso Regression** *(to check for features whose coefficients were reduced to zero meaning they were not really important)* and **Random Forest** *(plotted a bar graph of feature importances in order to see which features are driving change in the dependent variable)* to predict male and female salaries.

## Conclusions
Analysis of the Kaggle Developer Survey produced a lot of interesting insights. Some of the insights garnered are listed below:
* Most of the female survey participants are well educated, at least better in proportion to males.
* The results of the models confirmed that men are infact earning more money than women. This could be due to a lot of factors, one of which could be that more men have a higher number of years of coding experience and this is a major factor that drives earning potential.
* The model shows that on average, women earn about **20%** less than the average male developer.

## Limitations
This results are not set in stone of course, as a lot of modifications could be done to better improve the models and give a more accurate report. 
* One of such modifications is dividing the data into train and test datasets, so that after fitting the model, the test set is used for predictions. 
* Another modification would be to try other models and see if they are better at predicting salaries. 
* Hyper parameter tuning is also a modification in order to get the most accurate result out of a model.
