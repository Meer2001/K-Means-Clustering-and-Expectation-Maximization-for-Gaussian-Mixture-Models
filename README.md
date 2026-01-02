# K-Means-Clustering-and-Expectation-Maximization-for-Gaussian-Mixture-Models

## PROJECT OVERVIEW

This project explores unsupervised learning using two major clustering techniques:
(1) K-Means Clustering with Random and k-means++ initialization
(2) Gaussian Mixture Models (GMM) with Full and Diagonal covariance

The datasets analyzed are Blobs (well-separated, spherical clusters) and Moons (non-convex, crescent-shaped clusters).

The project objective is to evaluate how well K-Means and GMM capture different types of cluster structures, understand the effect of initialization and covariance assumptions, and compute the optimal number of clusters/components using Silhouette Score, ICSSD, Log-Likelihood, and BIC.

## PROJECT STRUCTURE

```text
clustering-project/
│
├── MachineLearning_Project4_Part1_and_Part2.ipynb # K-Means and GMM code
├── blobs_dataset.npy # Synthetic blobs (Imported using sklearn)
├── moons_dataset.npy # Synthetic moons (Imported using sklearn)
├── README.md # Project documentation
└── REPORT.pdf # Full written report and discussion
└──AI TRANSCRIPTS #AI Prompts
```

## DATASETS USED

1. Blobs Dataset
This is a synthetic dataset with 3 spherical, well-separated clusters. It is ideal for algorithms assuming isotropic cluster shapes such as K-means and other clustering algorithms.
2. Moons Dataset
It is a dataset with non-convex, crescent-shaped clusters. It is used to test algorithms on non-spherical structures and it highlights the scenarios where K-Means performs poorly and examines the advantages and disadvantages of Gaussian Mixture Models (GMMs).
Both datasets are 2D and generated using sklearn.datasets.

## DEPENDENCIES

The project uses Python version 3.9+ with the following libraries:
● numpy — for numerical operations
● scikit-learn — for implementing clustering algorithms and for evaluation metrics
● matplotlib — for data visualizations
● pandas — result tables & transformations

The requirements can be installed with following commands:
pip install numpy pandas scikit-learn matplotlib

## INSTALLATION AND SETUP

1. Download or clone the entire project folder.
2. Ensure dependencies are installed.
3. Open either .ipynb file in Google Colab or any other code editor, or Jupyter Notebook.

## HOW TO RUN THE PROJECT

Open MachineLearning_Project4_Part1_and_Part2.ipynb and run all cells.
The script automatically performs generation of dataset.

**PART1: K-Means**
- Performs K-Means for k = 2 to 5
- Computes Silhouette and ICSSD
- Plots clusters and elbow curves

**PART2: GMM**
- Fits GMMs using full & diagonal covariance
- Computes Silhouette, Log-Likelihood, BIC
- Visualizes clusters and likelihood/BIC trends

## STEPS USED IN THIS PROJECT

**Part 1: K-Means**
1. Dataset Generation
2. Clustering with random & k-means++ initialization
3. Evaluation using Silhouette Score & ICSSD
4. Elbow Method visualization
5. Cluster scatter plots
6. Comparison across initialization and datasets

**Part 2: Gaussian Mixture Models**
1. Dataset Generation
2. GMM fitting for full & diagonal covariance
3. Evaluation using Silhouette, Log-Likelihood, BIC
4. Model selection using BIC
5. Cluster visualizations & contour plots
6. Comparison against K-Means

## METRICS USED

Primary evaluation metrics used in this project are:
- Silhouette Score
- ICSSD (Intra-Cluster Sum of Squared Distances)
- Log-Likelihood (per-sample)
- Bayesian Information Criterion (BIC)

## FUTURE IMPROVEMENTS

● Implement DBSCAN or Spectral Clustering for non-convex datasets
● Extend analysis to high-dimensional datasets
● Automate model selection with GridSearch for GMM parameters
● Add cluster uncertainty visualizations for GMM
