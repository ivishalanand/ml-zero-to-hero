# 5. Feature Engineering

Feature engineering means turning raw, messy data into columns a model can actually learn from: filling in gaps, converting text categories into numbers, putting numbers on a similar scale, and inventing new columns that make patterns obvious. It matters because on tabular data, better features usually help more than a fancier algorithm. It is also where the most common beginner mistake happens: data leakage, where information from the test set sneaks into training.

## Key concepts

- missing-value imputation
- one-hot / ordinal / target encoding
- scaling (standardisation, normalisation)
- creating new features
- feature selection
- pipelines and data leakage

## Resources

Work through these from top to bottom. You don't need to finish every one: stop when the idea clicks, then do the mini-project.

| Title | Type | Level | Why it's good |
|---|---|---|--- |
| [Kaggle Learn: Intermediate Machine Learning](https://www.kaggle.com/learn/intermediate-machine-learning) (key lesson: [Data Leakage](https://www.kaggle.com/code/alexisbcook/data-leakage)) | Course | Beginner | Short lessons with exercises on missing values, categorical variables, pipelines and leakage. Best starting point. |
| [StatQuest: One-Hot, Label, Target and K-Fold Target Encoding](https://www.youtube.com/watch?v=589nCGeWG1w) | Video | Beginner | Explains every common way to turn categories into numbers, with pictures. |
| Google ML Crash Course: [Working with numerical data](https://developers.google.com/machine-learning/crash-course/numerical-data) and [Working with categorical data](https://developers.google.com/machine-learning/crash-course/categorical-data) | Course | Beginner | Clear written guide to scaling, binning, outliers and encoding, with quizzes. No sign-up. |
| [Google ML Crash Course: Feature cross exercises](https://developers.google.com/machine-learning/crash-course/categorical-data/feature-cross-exercises) | Interactive | Beginner | In-browser playground: combine two features and watch the model suddenly fit the data. |
| INRIA scikit-learn MOOC: [scaling](https://github.com/INRIA/scikit-learn-mooc/blob/main/notebooks/02_numerical_pipeline_scaling.ipynb) ([Colab](https://colab.research.google.com/github/INRIA/scikit-learn-mooc/blob/main/notebooks/02_numerical_pipeline_scaling.ipynb)), [categorical encoding](https://github.com/INRIA/scikit-learn-mooc/blob/main/notebooks/03_categorical_pipeline.ipynb) ([Colab](https://colab.research.google.com/github/INRIA/scikit-learn-mooc/blob/main/notebooks/03_categorical_pipeline.ipynb)), [ColumnTransformer](https://github.com/INRIA/scikit-learn-mooc/blob/main/notebooks/03_categorical_pipeline_column_transformer.ipynb) ([Colab](https://colab.research.google.com/github/INRIA/scikit-learn-mooc/blob/main/notebooks/03_categorical_pipeline_column_transformer.ipynb)) | Notebook | Beginner | Three notebooks that build a leak-free preprocessing pipeline step by step. Exercises included in the repo. |
| [Data School: How do I encode categorical features using scikit-learn?](https://www.youtube.com/watch?v=irHhDMbw3xo) | Video | Beginner | Live-coded OneHotEncoder, ColumnTransformer and Pipeline on Titanic. Shows the correct workflow. |
| [Python Data Science Handbook: 05.04-Feature-Engineering.ipynb](https://github.com/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.04-Feature-Engineering.ipynb) ([Colab](https://colab.research.google.com/github/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.04-Feature-Engineering.ipynb)) | Notebook | Beginner | One compact chapter: categorical, text, derived features, imputation and pipelines. |
| [Kaggle Learn: Feature Engineering](https://www.kaggle.com/learn/feature-engineering) | Course | Intermediate | Teaches creating features and ranking them with mutual information. Each lesson has an exercise. |
| [Yimeng-Zhang/feature-engineering-and-feature-selection](https://github.com/Yimeng-Zhang/feature-engineering-and-feature-selection) | Repo | Intermediate | A notebook per technique (missing data, outliers, encoding, selection). Good reference to keep open. |
| [Kaggle: House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) | Practice | Beginner | 79 messy columns with gaps and categories. The classic feature-engineering playground. |

## Mini-project

"Does feature engineering beat a better model?" Use the [Kaggle Titanic](https://www.kaggle.com/competitions/titanic) dataset. First build a baseline with only the numeric columns and note the cross-validated accuracy. Then build one scikit-learn `Pipeline` that imputes missing ages, one-hot encodes `Sex` and `Embarked`, scales the numbers, and adds two features you invent (for example `FamilySize = SibSp + Parch + 1` and a title pulled from the `Name` column). Compare the scores and write down which single feature helped most.

---

[← Model Evaluation](../04-model-evaluation/) · [All topics](../README.md) · [Hyperparameter Tuning →](../06-hyperparameter-tuning/)
