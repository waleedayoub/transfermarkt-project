## Midterm Project 2023

### Ideas
- User match level soccer data from [statsbomb](https://github.com/statsbomb/open-data/blob/master/doc/Open%20Data%20Matches%20v3.0.0.pdf) to predict the outcome of a match
    - Pass a pair of teams and use the history of their matchups to predict who will win

- Instead, use data from Transfermarkt to build a prediction service that given a match up between two teams, produces the top 3 most likely scorers for each team and the probability of each of them scoring

### Local project set up instructions
1. Clone this repo: 
2. Use poetry to install all dependencies:
    - ```poetry install```
3. Download the data using the kaggle API:
    - Go to the ```cd data```
    - You should have already installed the kaggle API through poetry, but you need a kaggle API token
    - To do that, log into Kaggle

### Data
- Source code from transfermarkt: https://github.com/dcaribou/transfermarkt-datasets
- While the source code above can be used to download the data and schedule it to update, it seems a bit easier to download it from Kaggle:
    - https://www.kaggle.com/datasets/davidcariboo/player-scores/data
- The easiest way to download the data is by following these steps:


    - To download from Kaggle, you can use their API: ```kaggle datasets download -d davidcariboo/player-scores```