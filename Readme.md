Idea: using the dataset flood.csv from kaggle will try to develop a ML to predict flood in areas using different parameters

I this practice project I used to methods to train.

### 1. RandomForest Regressor
- using the random forest regressor with a data split of 80% for test and train this simple technique gave a result of 0.7317 r2_score while
the MSE was at 0.0006715741405000005.


### 2. Using HyperParameter tuning
To further improve the results i tried hyper parameter tuning.
which included:
    - limiting random_states = 42
    - "n_estimators": [100, 200, 400],  # more trees => stabler, but slower
    - "max_depth": [10, 20, None],  # limit depth to prevent overfitting
    - "min_samples_split": [2, 10, 20], 
    - "min_samples_leaf": [1, 2, 4],
    - "bootstrap": [True, False],


this gave results = 
