# NFL Big Data Bowl

![image](https://user-images.githubusercontent.com/40786348/70203528-87bf9380-1760-11ea-8f0d-224044c271bd.png)

<br>

## Objective

- Develop model to better predict what contributes to a succesful run play. 
- How many yards can the runner earn for each play?

<br>

## Evaluation Metric
**Continuous Ranked Probability Score (CRPS)** - [explained here](https://stats.stackexchange.com/questions/246649/how-to-discretize-continuous-rank-probability-score)


<br>

## Winning Solutions

- 1st place solution [here](https://www.kaggle.com/c/nfl-big-data-bowl-2020/discussion/119400#latest-688670)

- 2nd place solution [here](https://www.kaggle.com/c/nfl-big-data-bowl-2020/discussion/119484#latest-684433)

- 3rd place solution [here](https://www.kaggle.com/c/nfl-big-data-bowl-2020/discussion/119314#latest-685891)

- 4th place solution [here](https://www.kaggle.com/c/nfl-big-data-bowl-2020/discussion/119885#latest-686046)

- 5th place solution [here](https://www.kaggle.com/c/nfl-big-data-bowl-2020/discussion/119357#latest-684386)

<br>

## some review about the competition 

- replace S feature with 10*Dis both for 2017 and 2018 (Data cleansing)
- using CNN architecture / x-axis 10 offensive players, y-axis defensive players, features on channels (1st place solution)
- can augment the data by flipping the coordinates of the players (when using CNN)
- stable CV strategy (seed averaging is necessary for neural network)
  - 5-fold GroupKFold on GameId, but in validation folds only consider data from 2018 (2018 dataset is more similar to 2019)
- going deeper, SE-module, residual networks didn't work (simple works best sometimes)