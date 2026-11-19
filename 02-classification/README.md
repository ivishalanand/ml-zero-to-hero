# 2. Classification

Classification is how a computer learns to sort things into categories: spam or not spam, which species of flower, whether a tumour is benign. You show it labelled examples and it learns a rule for drawing boundaries between the groups. Most real-world ML (fraud detection, medical screening, image labels) is classification, and each algorithm here draws those boundaries in a different way.

## Key concepts

- Decision boundary and predicted probability (sigmoid)
- Train / test split and cross-validation
- Confusion matrix, accuracy, precision, recall
- Distance and "nearest neighbours" (k-NN)
- Tree splits (Gini / entropy) and ensembles (random forests)
- Margin and kernels (SVM); Bayes' rule (naive Bayes)

## Resources

Work through these from top to bottom. You don't need to finish every one: stop when the idea clicks, then do the mini-project.

| Title | Type | Level | Why it's good |
|---|---|---|--- |
| [R2D3: A Visual Introduction to Machine Learning](https://r2d3.us/visual-intro-to-machine-learning-part-1/) | Interactive | Beginner | Animated story that builds a decision tree classifier as you scroll; zero prerequisites. |
| [StatQuest: Logistic Regression](https://www.youtube.com/watch?v=yIYKR4sgzI8) | Video | Beginner | Explains how a line becomes an S-curve that outputs probabilities. |
| [MLU-Explain: Logistic Regression](https://mlu-explain.github.io/logistic-regression/) | Interactive | Beginner | Move the threshold and data points and see predictions flip live. |
| [Google ML Crash Course: Classification](https://developers.google.com/machine-learning/crash-course/classification) | Course | Beginner | Clear lessons on thresholds, confusion matrix, precision, recall and ROC with quizzes. |
| [StatQuest: Decision and Classification Trees](https://www.youtube.com/watch?v=_L39rN6gz7Y), then [k-NN](https://www.youtube.com/watch?v=HVXime0nQeI), [Naive Bayes](https://www.youtube.com/watch?v=O2L2Uv9pdDA), [Random Forests](https://www.youtube.com/watch?v=J4Wdy0Wc_xQ), [SVM](https://www.youtube.com/watch?v=efR1C6CvhmE) | Video | Beginner | One short, friendly video per algorithm; watch in this order. |
| [MLU-Explain: Decision Tree](https://mlu-explain.github.io/decision-tree/) and [Random Forest](https://mlu-explain.github.io/random-forest/) | Interactive | Beginner | Watch a tree grow split by split, then see many trees vote. |
| [Microsoft ML-For-Beginners: Classification lessons](https://github.com/microsoft/ML-For-Beginners/tree/main/4-Classification) | Repo | Beginner | Four lessons classifying cuisines with logistic regression, k-NN, SVM and forests. |
| [Raschka, ML with PyTorch and Scikit-Learn: Ch. 3, A Tour of Classifiers](https://github.com/rasbt/machine-learning-book/blob/main/ch03/ch03.ipynb) | Notebook | Intermediate | Logistic regression, SVM, trees, forests and k-NN on Iris in one notebook. |
| Python Data Science Handbook: [Naive Bayes](https://github.com/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.05-Naive-Bayes.ipynb), [SVM](https://github.com/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.07-Support-Vector-Machines.ipynb), [Decision Trees and Random Forests](https://github.com/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.08-Random-Forests.ipynb) | Notebook | Intermediate | Three in-depth notebooks with great plots and real examples (text, faces, digits). |
| [Kaggle: Titanic competition](https://www.kaggle.com/competitions/titanic) (with the official [Titanic Tutorial](https://www.kaggle.com/code/alexisbcook/titanic-tutorial)) | Practice | Beginner | The standard first classification project; tutorial gets you to a submission. |

## Mini-project

Classify penguin species from body measurements using the [Palmer Penguins dataset](https://allisonhorst.github.io/palmerpenguins/) (free; one line in Python: `seaborn.load_dataset("penguins")`). Train logistic regression, k-NN, a decision tree and a random forest, compare them with a confusion matrix and cross-validated accuracy, and plot the decision tree to see which measurements matter most.

## Want more?

[scikit-learn: classifier comparison](https://scikit-learn.org/stable/auto_examples/classification/plot_classifier_comparison.html) (every classifier's boundary side by side) · [scikit-learn guide: Supervised learning](https://scikit-learn.org/stable/supervised_learning.html) · [INRIA scikit-learn MOOC](https://inria.github.io/scikit-learn-mooc/) · [StatQuest Machine Learning playlist](https://www.youtube.com/playlist?list=PLblh5JKOoLUICTaGLRoHQDuF_7q2GfuJF) · [UCI: Breast Cancer Wisconsin dataset](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)

---

[← Regression](../01-regression/) · [All topics](../README.md) · [Unsupervised Learning →](../03-unsupervised-learning/)
