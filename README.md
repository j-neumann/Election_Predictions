# Why turn out to vote if there's no one to vote for?

## Problem Statement

Does the presence of competitive local elections impact overall voter turnout?  

In this project, I create a voter turnout model that includes the presence of competitive state legislative races and assess the significance of that variable as a predictor, as well as the overall success of my model.  

There is lots of research on what factors contribute to voter turnout: women vote more than men, as do old people. There is research that shows that uncompetitive federal elections decrease turnout. There is very limited similar research published on local elections, so I wanted to build a model that tested that.

My hypothesis was that an increase in uncontested elections would lead to a decrease in voter turnout. I wanted to build both a frequentist and bayesian model to understand this question.  


## Executive Summary

I built a turnout prediction model that predicted county turnout for the state of Pennsylvania at 93% accuracy. I failed to reject the null hypothesis, and cannot conclusively say that an increase in non-competitive races decreases turnout.

### Contents of Notebooks:
- Data collection, cleaning, and feature engineering.
- Data Exploration
- Model Preparation
- Model Analysis

### Data:

For this project, I examined data only from Pennsylvania at the county level. I analyzed county results from 2000-2018 in both midterm and presidential election years. During those years, Pennsylvania has local state legislative elections, but no other local elections. All county and municipal elections in Pennsylvania are in odd years.

I collected data from dozens of sources. My primary source for turnout and registration data was the Pennsylvania Secretary of State's office. I also relied on historical data from University. My demographic data came from several Census surveys, and my economic data came from both the Census and the Bureau of Labor Statistics.

All data was collected at the county level except for controls that accounted for the national climate of the election year.


### Models Evaluated:

To evaluate this problem, I used a linear regression model. There was no regularization that improved model accuracy. My final model included 24 different variables including demographic controls, economic data, historic turnout data, and data regarding the political climate.

Additionally, I worked to build out a model using Bayesian statistics. I was unable to build a Bayesian model that was highly accurate (or included more than 3 variables), but it did suggest a negative relationship between voter turnout and uncompetitive elections.

## Conclusions

I was unable to reject the null hypothesis for my project, but I was able to create a highly accurate turnout model! Although, my model found the following to be significant:
- Prior turnout and national turnout
- Whether it was a presidential year and whether the top of the ticket was an incumbent
- Unemployment rate, education rate, median income
- The percent of voters who were registered as Democrat or Republican
- Age- the older your county, the more it voted.

To continue this project, I would like to:
- Improve Bayesian model
- Build a precinct-level model to improve accuracy
- Adjust and train this model on other states/outside of the safe controls of Pennsylvania






