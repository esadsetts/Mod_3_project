# Mod_3_project
Flatiron Mod 3 Project: Eric Adsetts & Joey Billet
## Project Overview
In recent years, the NBA has gained tremendous traction while skyrocketing in viewership. As players continue to tweak their game, it has always been interesting to see who ends up making it to the Hall of Fame. Our project focused on looking at different attributes of players to predict what will help them land themselves in the land of legends: The Hall of Fame.

A few questions we asked ourselves: 

Is there a relationship between average games played and making the Hall of Fame?
We used a two sample T-Test to look at this statistical relationship.

Is there a relationship between the position of a player and if they will make the Hall of Fame? 
We used a Chi-Squared Test to look at this statistical relationship.
As we looked through this relationship, we took a look at the amount fo players throughout every position and realized that there are more “Guards” in the NBA than any other position.

Is there a relationship between a players position and their height? 
We had a feeling there would be an obvious answer to this (that Center’s would be the tallest), but surprisingly, 

## The Approach
We first scraped our data from Basketball Reference 

Engineered unique features to give deeper insight and understanding to the dataset

Perform EDA on the dataset and create appropriate visualizations using Matplotlib and Seaborn 

Build and test multiple prediction models

Using a Two Sample T-Test we were able to reject the null hypothesis because our pvalue (9.540838228486468e-22) is less than 0.05 (alpha set at .05) when seeing if  there is a relationship between average games played and making the Hall of Fame

Using a Chi-Squared Test, were were able to reject the null hypothesis because chi square statistic (13.613) is greater than the critical value (12.592) when asking if there a relationship between the team position of a player and if they will make the Hall of Fame

Using a two sample t-test we failed to reject the null hypothesis that the mean height of players in the hall of fame is the same as players who aren’t

## Modeling

For modeling, we used five different types: KNN, Logistic Regression, Decision Tree, Random Forest, and XG Boost.

### Model Details
For KKN, our model received an F1 score of .69

For Logistic Regression, our model received an F1 score of .63

For Decision Tree, our model received an F1 score of .81

For Random Forest, our model received an F1 score of .74

For XG Boost, our model received an F1 score of .72
### Best Model
Our best model was Decision Tree with an F1 Score of 0.86. The most important feature was if the player had made an All Star Game Appearance. Surprisingly, points per game and total points were not very important features.