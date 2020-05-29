# Ranking players using a bayesian model on match history data
The model used is a variation of the TrueSkill that was taught in STA414 (Statistical Methods for Machine Learning II) at the University of Toronto.

It is implemented from scratch and uses stochastic variational inference to estimate the posterior distribution. StarCraft II matches are used as the data is, comparatively, simple. There are two players in any match, with one winner and one loser. The lack of ties and larger team sizes makes the implementation slightly easier. TrueSkill was developed for use in multiplayer competetive games, with multiple players per team, possible draws, or in some cases, more than one teams.

The dataset is obtained from kaggle: https://www.kaggle.com/alimbekovkz/starcraft-ii-matches-history
It consists of tournament games and their outcomes, played by professional players.
The primary goal is to (try to) observe the distribution of skill among the players in the dataset, and see what the model thinks the relative rankings of these professional players should be, based on their performance in these tournaments.
