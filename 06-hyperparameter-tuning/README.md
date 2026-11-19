# 6. Hyperparameter Tuning

Hyperparameters are the settings you choose before training, such as how deep a tree can grow or how big each learning step is. The model cannot learn them on its own. Tuning means trying different settings in an organised way and keeping the ones that score best on validation data. It matters because the same algorithm can go from mediocre to excellent with the right settings, and tuning carelessly is an easy way to overfit.

## Key concepts

- parameters vs. hyperparameters
- grid search
- random search
- Bayesian optimisation (Optuna)
- learning rate
- early stopping

## Resources

Work through these from top to bottom. You don't need to finish every one: stop when the idea clicks, then do the mini-project.

| Title | Type | Level | Why it's good |
|---|---|---|--- |
| [Google ML Crash Course: Hyperparameters](https://developers.google.com/machine-learning/crash-course/linear-regression/hyperparameters) | Article | Beginner | Explains learning rate, batch size and epochs in plain words with loss-curve pictures. |
| [Google ML Crash Course: Gradient descent exercise](https://developers.google.com/machine-learning/crash-course/linear-regression/gradient-descent-exercise) | Interactive | Beginner | Change the learning rate in your browser and watch training converge or blow up. |
| [Data School: How to find the best model parameters in scikit-learn](https://www.youtube.com/watch?v=Gol_qOgRqfA) | Video | Beginner | Walks through GridSearchCV and RandomizedSearchCV slowly, with the reasoning behind each step. |
| [Data School: 08_grid_search.ipynb](https://github.com/justmarkham/scikit-learn-videos/blob/master/08_grid_search.ipynb) ([Colab](https://colab.research.google.com/github/justmarkham/scikit-learn-videos/blob/master/08_grid_search.ipynb)) | Notebook | Beginner | The notebook from the video above. Run it and change the grid yourself. |
| INRIA scikit-learn MOOC: [grid search](https://github.com/INRIA/scikit-learn-mooc/blob/main/notebooks/parameter_tuning_grid_search.ipynb) ([Colab](https://colab.research.google.com/github/INRIA/scikit-learn-mooc/blob/main/notebooks/parameter_tuning_grid_search.ipynb)) and [randomized search](https://github.com/INRIA/scikit-learn-mooc/blob/main/notebooks/parameter_tuning_randomized_search.ipynb) ([Colab](https://colab.research.google.com/github/INRIA/scikit-learn-mooc/blob/main/notebooks/parameter_tuning_randomized_search.ipynb)) | Notebook | Beginner | Tunes a full pipeline on real census data and shows why random search scales better. |
| [Kaggle Learn (Intro to Deep Learning): Overfitting and Underfitting](https://www.kaggle.com/code/ryanholbrook/overfitting-and-underfitting) | Course | Beginner | Shows early stopping on learning curves in Keras, with a follow-up exercise. |
| [Abhishek Thakur: Hyperparameter Optimization - This Tutorial Is All You Need](https://www.youtube.com/watch?v=5nYqK-HaoKY) | Video | Intermediate | One live-coded session going from grid search to random search, Bayesian methods and Optuna. |
| [Distill: Exploring Bayesian Optimization](https://distill.pub/2020/bayesian-optimization/) | Interactive | Intermediate | Animated, step-by-step picture of how Bayesian optimisation picks the next setting to try. |
| [Optuna examples: quickstart.ipynb](https://github.com/optuna/optuna-examples/blob/main/quickstart.ipynb) ([Colab](https://colab.research.google.com/github/optuna/optuna-examples/blob/main/quickstart.ipynb)), then the [official Optuna tutorial](https://optuna.readthedocs.io/en/stable/tutorial/index.html) | Notebook | Intermediate | Official ten-minute Optuna notebook: define an objective, run a study, plot the results. |
| [Kaggle: Spaceship Titanic](https://www.kaggle.com/competitions/spaceship-titanic) | Practice | Beginner | Beginner competition where tuning a gradient-boosting model visibly moves your leaderboard score. |

## Mini-project

"Grid vs. random vs. Optuna." Use the California Housing dataset (built into scikit-learn as `fetch_california_housing`, described on the [scikit-learn datasets page](https://scikit-learn.org/stable/datasets/real_world.html)). Tune a `RandomForestRegressor` or `HistGradientBoostingRegressor` three ways with the same budget of about 30 trials each: `GridSearchCV`, `RandomizedSearchCV`, and an Optuna study. Record the best cross-validated RMSE and the time each took in a small table, then check the winner once on a held-out test set. Which method found the best settings fastest?

---

[← Feature Engineering](../05-feature-engineering/) · [All topics](../README.md) · [Neural Networks →](../07-neural-networks/)
