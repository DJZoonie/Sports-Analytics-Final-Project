# Sports-Analytics-Final-Project
The goal of my project is to analyze the 2018-19 Raptors playoff series and determine whether they played better or worse than in the regular season

## How to run the model
To run this model, we need 3 main variables:
  -The team ID's for the team I'm looking to analyze as well as their opponents.
  -The player ID's for each player in those teams.
  -The game ID's for the games I'm looking to analyze as well as the Regular Season games used to train the logistic regression model.
  
  ### The player ID's for each player can be obtained using their full name in getPlayerID() function.
  ### The team ID's can be obtained by inputing player ID for a player on that team in getTeamID() function.
  ### The game ID's can be obtained by inputing a date and the games after that date will be displayed. We can choose a game ID from that list


Once we have those variables, we can use the shotChartData to receive the data for each shot attempt for a team during that game. With this we can 
get our training datasets of shot attempts for the team we are analyzing and their opponents.

Shot charts for the games used for the training set as well as the bar graphs with data regarding the features used in the model will be displayed.

## Model creation and evaluation
With this data, we can create 3 logistic regression models, one for each team involved.
These models can be used to estimate how many points we're supposed to get depending on the locations of the shots taken during the games I want to analyze.
Accuracy, f1-score and confusion matrix for the model is then displayed.
Actual and predicted shot charts for each game analyzed are also displayed.
Predictions for the expected points during the games are done for each team and results are printed.
