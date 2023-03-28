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

# Standards
**Standard 1:** In the matches table, 11 players from each team are listed. I assumed that these 11 players are the only players that participated in the specific game, although this is highly unlikely.<BR>
**Standard 2:** I changed all column headers to follow the specific format of capitalizing the first letter of each word and connecting the words without underscore, like this example: "CountryID".<BR>
**Standard 3:** If a column contained more than 75% missing data, I eliminated that column from the table.<BR>
**Standard 4:** To keep the data as concise as possible, I dropped any column that I deemed unnecessary or useful to achieve the goals of this report.

# Biases
**Bias 1:** Clear information about players in each team is not part of this data set. This may be because the players can change at any moment in the game and this information is not entered.<BR>
**Bias 2:** I have no expertise in football. There may be parts of the data that I have overlooked that may have been most important and I may have given importance to parts of the data that may have had little significance.

# Conclusions
**The Analysis of the Data:** I reviewed nearly 200,000 data points related to the European football matches. <br>
**The Goals:** The major goal of this analysis was to find a model that could predict the outcome of a match.
I utilized the 8 models listed below and the accuracy score of each model.
<BR>
    1. Logistic Regression: 52 <BR>
    2. Logistic Regression with Elastic Net Regularization: 50 <BR>
    3. Decision Tree: 47 <BR>
    4. Random Forest: 45 <BR>
    5. Random Forest with Grid Search: 50 <BR>
    6. Random Forest with Randomized Search: 51 <BR>
    7. Support Vector Classification (SVC): 53 <BR>
    8. Principle Component Analysis (SVC): 52 <BR>
<BR>
**Overall Conclusion:** As can be seen by their performance analyses, none of the models I utilized in this report can be relied on to predict the outcome of a match. This analysis seems to indicate that it is not possible to adequately predict the outcome of a football match based on the data from the datasets I analyzed. Based on my analysis, I recommend creating a business based on betting on such matches with much caution.
