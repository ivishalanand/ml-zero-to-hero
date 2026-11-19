# 1. Regression

Regression is how a computer learns to predict a number, like the price of a house or tomorrow's temperature, from examples. It finds the line (or curve) that best fits past data, then uses it to guess new values. It is the first model almost everyone learns, and the ideas behind it (a loss to measure error, gradient descent to reduce it, regularization to avoid overfitting) power almost every other model, including neural networks.

## Key concepts

- Features, target, and the fitted line (weights and bias)
- Loss function (mean squared error)
- Gradient descent and learning rate
- Polynomial features (fitting curves)
- Overfitting vs. underfitting
- Regularization (Ridge / L2, Lasso / L1)

## Resources

Work through these from top to bottom. You don't need to finish every one: stop when the idea clicks, then do the mini-project.

| Title | Type | Level | Why it's good |
|---|---|---|--- |
| [StatQuest: The Main Ideas of Fitting a Line to Data](https://www.youtube.com/watch?v=PaFPbb66DxQ) | Video | Beginner | Nine-minute, no-jargon picture of least squares; the best first watch. |
| [MLU-Explain: Linear Regression](https://mlu-explain.github.io/linear-regression/) | Interactive | Beginner | Scroll-driven visuals; drag the line yourself and watch the error change. |
| [Google ML Crash Course: Linear Regression](https://developers.google.com/machine-learning/crash-course/linear-regression) (with the [gradient descent exercise](https://developers.google.com/machine-learning/crash-course/linear-regression/gradient-descent-exercise)) | Course | Beginner | Short written lessons on loss and gradient descent with in-browser sliders and a quiz. |
| [StatQuest: Gradient Descent, Step-by-Step](https://www.youtube.com/watch?v=sDv4f4s2SB8) | Video | Beginner | Works through gradient descent with real numbers, one step at a time. |
| [Andrew Ng: Machine Learning Specialization (full playlist)](https://www.youtube.com/playlist?list=PLkDaE6sCZn6FNC6YRfRQc_FbeQrF8BwGI) | Video | Beginner | The classic course, free on YouTube; first part covers linear regression and gradient descent. |
| [Microsoft ML-For-Beginners: Regression lessons](https://github.com/microsoft/ML-For-Beginners/tree/main/2-Regression) (start with the [linear and polynomial notebook](https://github.com/microsoft/ML-For-Beginners/blob/main/2-Regression/3-Linear/notebook.ipynb)) | Repo | Beginner | Four guided lessons on pumpkin-price data with quizzes, assignments and solutions. |
| [Python Data Science Handbook: In Depth: Linear Regression](https://github.com/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.06-Linear-Regression.ipynb) ([read online](https://jakevdp.github.io/PythonDataScienceHandbook/05.06-linear-regression.html)) | Notebook | Beginner | One notebook covers linear, polynomial, Ridge and Lasso with scikit-learn. |
| [StatQuest: Regularization Part 1: Ridge (L2) Regression](https://www.youtube.com/watch?v=Q81RR3yKn30) (then [Part 2: Lasso](https://www.youtube.com/watch?v=NGf0voTMlcs)) | Video | Beginner | Shows why a slightly worse fit on training data predicts better. |
| [Hands-On ML (3rd ed.): Chapter 4, Training Linear Models](https://github.com/ageron/handson-ml3/blob/main/04_training_linear_models.ipynb) | Notebook | Intermediate | Codes batch, stochastic and mini-batch gradient descent, polynomial and regularized models. |
| [Kaggle: House Prices competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) (pair with [Kaggle Learn: Intro to Machine Learning](https://www.kaggle.com/learn/intro-to-machine-learning)) | Practice | Beginner | Never-ending beginner competition; the course walks you to a first submission. |

## Mini-project

Predict California house prices. Load the California Housing dataset with `sklearn.datasets.fetch_california_housing()` (free, no account; [dataset docs](https://scikit-learn.org/stable/datasets/real_world.html)). Fit a plain linear regression, then add polynomial features, then Ridge. Compare the three on a held-out test set with RMSE and plot predicted vs. actual prices.

## Want more?

[trekhleb/homemade-machine-learning](https://github.com/trekhleb/homemade-machine-learning) (algorithms coded from scratch) · [Seeing Theory: Regression Analysis](https://seeing-theory.brown.edu/regression-analysis/index.html) (interactive) · [Setosa: Ordinary Least Squares](https://setosa.io/ev/ordinary-least-squares-regression/) (interactive) · [Raschka: Ch. 9, Regression](https://github.com/rasbt/machine-learning-book/blob/main/ch09/ch09.ipynb) · [scikit-learn guide: Linear Models](https://scikit-learn.org/stable/modules/linear_model.html) · [3Blue1Brown: Gradient descent](https://www.youtube.com/watch?v=IHZwWFHWa-w)

---

[All topics](../README.md) · [Classification →](../02-classification/)
