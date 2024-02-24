# CalculatingFootballSoccerOdds
This is an approach to the way bookies calculate football match odds using PCA, Kmeans, SVM, and RF; Serie A and Bundesliga data are used.

The logic is very simple: group teams by their performance stats using Kmeans to form clusters, then from the history of results of each team vs opponent team's cluster and the history of results between clusters then, get the proportions of wins, draws, and defeats.

Append the history sum to every game and train the SVM or RF model with past results.

And there you go. Our odds model is done, you can calculate the probability of upcoming matches just by getting the cluster's history results.
