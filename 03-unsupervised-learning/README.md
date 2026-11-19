# 3. Unsupervised Learning

Unsupervised learning finds patterns in data that has no labels or right answers. Clustering groups similar things together (customers with similar habits, similar songs), and dimensionality reduction squeezes data with hundreds of columns down to two or three so you can plot and understand it. It matters because most of the world's data is unlabelled, and these tools are how you explore it before doing anything else.

## Key concepts

- Clusters, centroids and distance
- Choosing k (elbow method, silhouette score)
- Dendrograms (hierarchical clustering)
- Density and noise points (DBSCAN)
- Principal components and explained variance (PCA)
- Embeddings for visualisation (t-SNE, UMAP) and feature scaling

## Resources

Work through these from top to bottom. You don't need to finish every one: stop when the idea clicks, then do the mini-project.

| Title | Type | Level | Why it's good |
|---|---|---|--- |
| [StatQuest: K-means clustering](https://www.youtube.com/watch?v=4b5d3muPQmA), then [Hierarchical Clustering](https://www.youtube.com/watch?v=7xHsRkOdVwo) and [DBSCAN](https://www.youtube.com/watch?v=RDZUdRSDOok) | Video | Beginner | Three short videos giving the plain-English idea behind each clustering method. |
| [Naftali Harris: Visualizing K-Means Clustering](https://www.naftaliharris.com/blog/visualizing-k-means-clustering/) (and [Visualizing DBSCAN](https://www.naftaliharris.com/blog/visualizing-dbscan-clustering/)) | Interactive | Beginner | Step through the algorithm click by click on shapes where it works and fails. |
| [Google: Clustering course](https://developers.google.com/machine-learning/clustering) | Course | Beginner | Short written course on what clustering is, k-means, and judging results. |
| [Microsoft ML-For-Beginners: Clustering lessons](https://github.com/microsoft/ML-For-Beginners/tree/main/5-Clustering) (see the [K-Means notebook](https://github.com/microsoft/ML-For-Beginners/blob/main/5-Clustering/2-K-Means/notebook.ipynb)) | Repo | Beginner | Two guided lessons clustering Nigerian music data, with quizzes and solutions. |
| Python Data Science Handbook: [k-Means Clustering](https://github.com/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.11-K-Means.ipynb) and [Principal Component Analysis](https://github.com/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/05.09-Principal-Component-Analysis.ipynb) | Notebook | Beginner | Runnable notebooks with step-by-step plots; clusters digits and compresses images. |
| [StatQuest: Principal Component Analysis (PCA), Step-by-Step](https://www.youtube.com/watch?v=FgakZw6K1QQ) | Video | Beginner | Builds PCA from a two-point scatter plot with no linear algebra needed. |
| [Setosa: Principal Component Analysis Explained Visually](https://setosa.io/ev/principal-component-analysis/) | Interactive | Beginner | Drag points and watch the principal components rotate in real time. |
| [Hands-On ML (3rd ed.): Chapter 9, Unsupervised Learning](https://github.com/ageron/handson-ml3/blob/main/09_unsupervised_learning.ipynb) (and [Chapter 8, Dimensionality Reduction](https://github.com/ageron/handson-ml3/blob/main/08_dimensionality_reduction.ipynb)) | Notebook | Intermediate | Full code for k-means, DBSCAN, choosing k, PCA and more. |
| [Distill: How to Use t-SNE Effectively](https://distill.pub/2016/misread-tsne/) and [Google PAIR: Understanding UMAP](https://pair-code.github.io/understanding-umap/) (videos: [t-SNE](https://www.youtube.com/watch?v=NEaUSP4YerM), [UMAP](https://www.youtube.com/watch?v=eN0wFzBA4Sc)) | Interactive | Intermediate | Play with the settings and learn what these plots can and cannot tell you. |
| Kaggle Learn exercises: [Clustering With K-Means](https://www.kaggle.com/code/ryanholbrook/clustering-with-k-means) and [Principal Component Analysis](https://www.kaggle.com/code/ryanholbrook/principal-component-analysis) (lessons 4 and 5 of [Feature Engineering](https://www.kaggle.com/learn/feature-engineering)) | Practice | Intermediate | Short tutorials each followed by a graded hands-on exercise in the browser. |

## Mini-project

Segment shoppers with the [Mall Customer Segmentation dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python) (200 rows; free Kaggle account to download). Scale the features, run k-means, pick k with the elbow method, and plot income vs. spending score coloured by cluster. Then try DBSCAN on the same data and describe each customer group in one sentence. No-account alternative: cluster the built-in wine data, `sklearn.datasets.load_wine()` ([docs](https://scikit-learn.org/stable/datasets/toy_dataset.html)), and use PCA to plot it in 2D.

## Want more?

[scikit-learn: clustering comparison](https://scikit-learn.org/stable/auto_examples/cluster/plot_cluster_comparison.html) (every method on the same shapes) · [scikit-learn guide: Clustering](https://scikit-learn.org/stable/modules/clustering.html) · [EduClust](https://educlust.dbvis.de/) (interactive) · [Raschka: Ch. 10, Clustering](https://github.com/rasbt/machine-learning-book/blob/main/ch10/ch10.ipynb) · [TensorFlow Embedding Projector](https://projector.tensorflow.org/) (interactive)

---

[← Classification](../02-classification/) · [All topics](../README.md) · [Model Evaluation →](../04-model-evaluation/)
