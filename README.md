![Alt_Text](https://github.com/KevinNourian/Football/blob/main/Images/football.png)
# Important
Open the FootballProject.ipynb file first.

# Introduction
Football is believed to have originated in China in the third century BC. It is the world’s most popular ball game in number of players and spectators. Football is a game in which two teams of 11 players, use any part of their bodies except their hands and arms to maneuver the ball into the opposing team’s goal. Only the goalkeeper is permitted to use his hands and may do so only within the penalty area surrounding the goal. The team that scores the most goals wins. The standard length of a game is 90 minutes with a short break, known as "half time," at the 45-minute mark. Only America and Canada call the sport soccer.

European football clubs operate as independent entities that are typically owned by a group of investors or a single owner. They are generally organized into leagues, which are typically organized at the national level. For example, in England, there is the Premier League, in Spain there is La Liga, in Germany there is the Bundesliga, and so on. Within each league, teams compete against each other over the course of a season. At the end of the season, the team with the most points become the champions of the league.

In addition to competing in their national leagues, European football clubs also compete in a variety of other competitions, including international club competitions like the UEFA Champions League and Europa League, as well as domestic cup competitions.

Revenue for professional football clubs in Europe comes from a variety of sources, including ticket sales, merchandising, and broadcast rights. The largest and most successful clubs are often able to generate significant revenue through these channels, which allows them to attract top talent and remain competitive both domestically and internationally.

Football’s governing body is the Fédération Internationale de Football Association (FIFA).

# Goal
In this report, I analyze the data of the Ultimate 25k+ Matches Football Database (European) from Kaggle to determine if there are ways to gain an advantage in predicting the outcome of a game for purposes of betting.

# Jupyter Notebooks
For this project, I created a separate Jupyter Notebook for the data overview and preprocessing part of this report. Therefore, this project is comprised of two Jupyter Notebooks:
1. Data Overview and preprocessing Notebook
2. The Project Notebook
Open the Project Notebook. It will import the Data Overview and Cleaning Notebook.

# Technical Requirements
1. Perform Data cleaning, exploratory data analysis and feature engineering.
2. Use parameters that gives the most important statistical insights of the data.
3. Create visualizations.
4. Perform statistical inferences and hypothesis testing. Set appropriate significance levels and create confidence intervals for the variables of interest.
5. Apply linear machine learning models and use them for forecasting.
6. Use cross validation, information criteria, and other methods to specify correct modeling.
7. Choose and use appropriate metrics to measure models' performances.
8. Provide clear explanations.
9. Provide conclusions and suggest how the analysis can be improved.

# Datasets
I used the Ultimate 25k+ Matches Football Database - European dataset from Kaggle. This data set is comprised of seven (7) tables.
    1. Country
    2. League
    3. Player
    4. Plater Attribute
    5. Team
    6. Team Attribute
    7. Match

# Conclusions
**The Analysis of the Data:** I reviewed nearly 200,000 data points related to European football games. <br>
**The Goal of the Project:** The major goal of this project was to find a model that could classify the outcome of a match with an adequate level of certainty.
I utilized the 9 models. According to Standard 6, I decided to create a model that captures as many wins as possible. I was not interested in capturing losses or draws. So, the Recall Score for wins in each model is of ultimate interest to me. My standard for an acceptable Recall Score for wins is 75%.
**Recall Scores for Wins:** All models, except for Random Forest and Random Forest with Grid Search exceed my standard.
**Performance of ML Models:** The other scores indicate that this model is poor at capturing losses or draws.  
**Feature Engineering and Hyperparameter Testing:** I tried feature engineering and hyperparameter testing with techniques such as PCA or Grid Search. PCA showed similar results as the other models. Random Forest with Grid Search improved the Recall Score for wins over the Random Forest model without Grid Search.
**Amount and Quality of Data:** In many cases with ML, having better and more data is MUCH more important than the model used. I tried my best with the data I had and tried to use different models. My results did not improve.
**Stochastic System:** A football match is a stochastic system. Two matches even with the same seemingly initial conditions like the players, place or weather can have varying results. This makes classifying the result of a football match extremely difficult. Human behavior is hard to classify. It cannot be easily capsulized in numbers. This is one of the reasons, it would be hard to classify the outcome of a game. For example, an important player could have fought with his wife or been involved in a traffic accident on the day of the game. This could have affected his performance and the outcome of the game, and this is not something that can be measured by the statistical information given in this dataset. Similarly, a low-performing player could have performed exceptionally well in a particular match, creating a win for his team that was unexpected.
**Simple Guesses:** From some of the measures, like the number of goals, crossings and penalties, teams usually did better when they played at home than when they played away from home. Without any other data to rely on, a safe "guess" may be to pick the winner of a match simply based on if a team is playing at home or away from home.
**Business Recommendation:** I recommend moving with caution if one decides to create a business based on betting on such matches.
