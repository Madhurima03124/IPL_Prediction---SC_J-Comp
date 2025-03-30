# IPL Match Winner Prediction - Soft Computing J-Component by G Madhurima(21MIS1155) & P V J Srikanth Reddy(21MIS1095)

## Overview
This project aims to predict the winner of an Indian Premier League (IPL) match using a Deep Learning model. The deep neural network was selected for the prediction based on its performance after hyperparameter tuning.

## Project Structure
- **Data Preprocessing**: Categorical data encoding, feature scaling, and data splitting.
- **Model Building**: A Deep Learning model was built and trained on the dataset.
- **Evaluation**: The model's performance was evaluated using metrics like Mean Absolute Error (MAE).
- **Interactive Tool**: An interface using `ipywidgets` allows users to input match features and get real-time predictions.

## Dataset
The dataset consists of the following attributes related to IPL matches:
- `mid`: Match ID
- `date`: Date of the match
- `venue`: Venue of the match
- `bat_team`: Batting team
- `bowl_team`: Bowling team
- `batsman`: Name of the batsman on strike
- `bowler`: Name of the bowler
- `runs`: Runs scored by the batting team up to that point
- `wickets`: Number of wickets lost by the batting team
- `overs`: Total overs bowled in the match up to that point
- `runs_last_5`: Runs scored in the last 5 overs
- `wickets_last_5`: Number of wickets lost in the last 5 overs
- `striker`: Current batsman on strike
- `non-striker`: Batsman not on strike
- `total`: Final score of the batting team

## Deep Learning Model
The project used a fully connected Deep Neural Network (DNN) for the prediction of IPL match scores. The network was optimized using hyperparameters such as:
- Number of layers and neurons in each layer
- Activation functions
- Optimizers
- Batch size
- Learning rate
- Epochs

Hyperparameter tuning was performed using `RandomizedSearchCV` to achieve the best model performance.

## Best Model
- The final Deep Learning model, trained with the optimized hyperparameters, provided the best prediction accuracy for the task of IPL score prediction.

## Prerequisites
To run the project, you need the following libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn keras tensorflow ipywidgets
