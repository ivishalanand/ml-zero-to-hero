# 4. Model Evaluation

Model evaluation is how you find out whether your model has really learned something or has just memorised its training data. You hide part of the data, let the model predict it, and score the predictions with a metric that fits the problem. It matters because a model that looks 99% accurate on data it has already seen can fail badly on new data, and the wrong metric can hide that failure.

## Key concepts

- train / validation / test split
- cross-validation
- overfitting vs. underfitting (bias-variance)
- confusion matrix
- precision, recall, F1
- ROC curve and AUC
- regression metrics (MAE, RMSE, R²)

## Resources

Work through these from top to bottom. You don't need to finish every one: stop when the idea clicks, then do the mini-project.

| Title | Type | Level | Why it's good |
|---|---|---|--- |
| [MLU-Explain: The Importance of Data Splitting (train, test, validation)](https://mlu-explain.github.io/train-test-validation/) | Interactive | Beginner | Scroll-through animation shows why you need three separate sets. No code needed. |
| [StatQuest: Machine Learning Fundamentals: Cross Validation](https://www.youtube.com/watch?v=fSytzGwwBVw) | Video | Beginner | Six-minute, jargon-free explanation of k-fold cross-validation. |
| [MLU-Explain: The Bias Variance Tradeoff](https://mlu-explain.github.io/bias-variance/) | Interactive | Beginner | Drag sliders and watch a model go from underfit to overfit. |
| [Data School: 07_cross_validation.ipynb](https://github.com/justmarkham/scikit-learn-videos/blob/master/07_cross_validation.ipynb) ([Colab](https://colab.research.google.com/github/justmarkham/scikit-learn-videos/blob/master/07_cross_validation.ipynb), [matching video](https://www.youtube.com/watch?v=6dbrR-WymjI)) | Notebook | Beginner | First hands-on code: train/test split versus k-fold in scikit-learn, with a video walkthrough. |
| StatQuest: [The Confusion Matrix](https://www.youtube.com/watch?v=Kdsp6soqA7o), then [ROC and AUC, Clearly Explained](https://www.youtube.com/watch?v=4jRBRDbJemM) | Video | Beginner | The clearest short videos on classification metrics. Watch in this order. |
| MLU-Explain: [Precision & Recall](https://mlu-explain.github.io/precision-recall/) and [ROC & AUC](https://mlu-explain.github.io/roc-auc/) | Interactive | Beginner | Move the decision threshold yourself and see each metric change live. |
| [Google ML Crash Course: Classification](https://developers.google.com/machine-learning/crash-course/classification) | Course | Beginner | Short written module on thresholds, accuracy, precision, recall, ROC-AUC with quizzes. No sign-up. |
| INRIA scikit-learn MOOC: [metrics_classification.ipynb](https://github.com/INRIA/scikit-learn-mooc/blob/main/notebooks/metrics_classification.ipynb) ([Colab](https://colab.research.google.com/github/INRIA/scikit-learn-mooc/blob/main/notebooks/metrics_classification.ipynb)) and [metrics_regression.ipynb](https://github.com/INRIA/scikit-learn-mooc/blob/main/notebooks/metrics_regression.ipynb) ([Colab](https://colab.research.google.com/github/INRIA/scikit-learn-mooc/blob/main/notebooks/metrics_regression.ipynb)) | Notebook | Beginner | Written by scikit-learn's own developers. Covers both classification and regression metrics (MAE, MSE, R²). |
| [Hands-On ML (3rd ed.): 03_classification.ipynb](https://github.com/ageron/handson-ml3/blob/main/03_classification.ipynb) ([Colab](https://colab.research.google.com/github/ageron/handson-ml3/blob/main/03_classification.ipynb)) | Notebook | Intermediate | Full worked example on MNIST: confusion matrix, precision/recall trade-off, ROC curves. |
| [Kaggle: Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic) | Practice | Beginner | Evaluate your own model with cross-validation, then compare with the hidden-test leaderboard score. |

## Mini-project

"Is accuracy lying to me?" Use the Breast Cancer Wisconsin dataset (built into scikit-learn as `load_breast_cancer`, also on the [UCI repository](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)). Train a logistic regression and a decision tree. For each, report 5-fold cross-validated accuracy, then on a held-out test set print the confusion matrix, precision, recall, F1 and plot the ROC curve. Finish with two sentences: which model would you give a doctor, and why is recall more important than accuracy here?

---

[← Unsupervised Learning](../03-unsupervised-learning/) · [All topics](../README.md) · [Feature Engineering →](../05-feature-engineering/)
