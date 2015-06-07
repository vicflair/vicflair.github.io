**Guide to Data Science**
By **Victor Ma**

![Data science](https://upload.wikimedia.org/wikipedia/commons/0/02/Giraffe_Ithala_KZN_South_Africa_Luca_Galuzzi_2004.JPG)

A practical reference guide to applied data science with my own commentary and summaries.

The structure this guide attempts to follow for each major topic:

- Summary
- Instructions
- Commentary
- Examples
- Tools and resources, e.g. packages, modules
- FAQ
- References and learning resources

# Table of Contents
<!-- MarkdownTOC depth=2 -->

- [Programming](#programming)
    - [R](#r)
    - [Python](#python)
    - [Java](#java)
- [Learning Resources](#learning-resources)
- [Pre-processing](#pre-processing)
    - [Data collection and ingestion](#data-collection-and-ingestion)
    - [Data munging, cleaning, preparing](#data-munging-cleaning-preparing)
    - [Feature and data transformation](#feature-and-data-transformation)
    - [Feature selection and engineering](#feature-selection-and-engineering)
    - [Imbalanced data](#imbalanced-data)
- [Exploratory analysis](#exploratory-analysis)
    - [High-level](#high-level)
    - [Manual inspection](#manual-inspection)
- [Unsupervised learning](#unsupervised-learning)
    - [Clustering](#clustering)
    - [Association rules mining](#association-rules-mining)
    - [Anomaly detection](#anomaly-detection)
- [Supervised learning: classification and regression](#supervised-learning-classification-and-regression)
- [Reinforcement learning](#reinforcement-learning)
- [Meta methods and algorithms](#meta-methods-and-algorithms)
- [Time series analysis](#time-series-analysis)
- [Text mining and NLP](#text-mining-and-nlp)
- [Network analysis](#network-analysis)
- [Visualization](#visualization)
- [Optimization](#optimization)
- [Statistics](#statistics)
- [Big Data](#big-data)
- [Learning theory](#learning-theory)
- [Mathematics fundamentals](#mathematics-fundamentals)
- [Computer science fundamentals](#computer-science-fundamentals)
- [Simulation](#simulation)

<!-- /MarkdownTOC -->

# Programming

## R
- [RStudio](http://www.rstudio.com/): popular IDE for R
- [CRAN](http://cran.r-project.org/): repository of R packages
- [caret](https://topepo.github.io/caret/index.html): library with supporting functions for machine learning
- [ggplot2](http://ggplot2.org/): visualization library based on the grammar of graphics
- [dplyr](http://goo.gl/87ZM57): library for manipulating data frames
- [tidyr](http://goo.gl/87ZM57): library for cleaning up messy data
- [Hands-on Data Science with R](http://onepager.togaware.com/): An excellent, fairly comprehensive set of tutorials for doing data science using R. 

## Python
- [Scikit](http://scikit-learn.org/stable/index.html): popular machine learning library with great documentation
- [Numpy](www.numpy.org/), [Scipy](www.scipy.org), and [Matplotlib](http://matplotlib.org/): popular packages for scientific computing and visualization
- [NLTK](www.nltk.org): Natural langue processing and text mining platform.
- [Pandas](http://pandas.pydata.org/) for data frames
- [IPython] (http://ipython.org/): Python interpreter with lots of nifty features, including [IPython Notebook](http://goo.gl/dY3RQ) 
- [Spyder](https://github.com/spyder-ide/spyder): IDE for scientific computing in Python
- [Pycharm](https://www.jetbrains.com/pycharm/): General purpose Python IDE
- [Sublime Text](https://www.sublimetext.com/): General purpose text editor, commonly used for programming and development

## Java
- [Weka](http://www.cs.waikato.ac.nz/ml/weka/)
- [ABAGAIL](https://github.com/pushkar/ABAGAIL)

# Learning Resources
- [Booz Allen Hamilton Field Guide to Data Science](http://goo.gl/G5vggo)
- [Hands-on Data Science with Togaware](http://onepager.togaware.com/)
- [Coursera machine learning course by Andrew Ng](https://www.coursera.org/course/ml)
- [“Machine learning” by Tom Mitchell](https://www.cs.cmu.edu/~tom/mlbook.html)
- ["The elements of statistical learning" by Hastie, Tibshirani, and Friedman](http://statweb.stanford.edu/~tibs/ElemStatLearn/)
- [Becoming a Data Scientist - Curriculum via Metromap](http://nirvacana.com/thoughts/becoming-a-data-scientist/)
- [Data Science Central](http://www.datasciencecentral.com/)
- [Natural Language Processing with Python](www.nltk.org/book/)
- [Data science IPython Notebooks](https://github.com/donnemartin/data-science-ipython-notebooks)
- Coursera, Udacity, EdX (specific courses??)

# Pre-processing

## Data collection and ingestion

## Data munging, cleaning, preparing
- Normalize variable names
- Select candidate features
- Data formats: i.e. numeric, categorical
- Ignore IDs, outputs
- Ignore features which are constant, all missing, or mostly missing
- Ignore observations which are all or mostly missing
- Ignore low variance features?
- Ignore or bin features with too many levels
- Ignore, impute, or mask missing values
- Identify highly correlated or linearly dependent features

## Feature and data transformation
- (for R only) Factors
    - Drop unused levels
    - Reorder levels
- Dummy code categorical data
- Scale or standardize (z-score) data
- Normalize data, that is, make it more normal
- Dimensionality reduction
- Clustering
- Expansions, e.g. x*y, x/y, xˆ2, ax+by, etc.
- Tidy or reshape data so that we have one measurement per observation
- Sampling
- Stratified sampling

## Feature selection and engineering
Parse and transform raw data into features that better capture the structure of the problem so that it's more suitable for machine learning models. That is,
we have improved predictive power.

http://machinelearningmastery.com/discover-feature-engineering-how-to-engineer-features-and-how-to-get-good-at-it/

## Imbalanced data

# Exploratory analysis

## High-level
- Summarize over entire dataset
- Summarize by groups
- Add group summary statistics to original observations

## Manual inspection
- Compare between pre and post opening
- Compare between real and fake
- Look at invidual features, e.g. density or histogram plots
    - [ggplot2 example of density and histogram plots](http://goo.gl/GqvKAV)
- Look at pairs of features, e.g. 2d scatter plots
    - [ggplot2 example of scatterplot matrices](http://goo.gl/GqvKAV)
    - [ggpairs example of a plot matrix](http://goo.gl/vPWpzG)

# Unsupervised learning

## Clustering

### Set-up
- Choose distance metric, e.g. Euclidean or Manhattan (or more generally L-norm), Mahalanobis, Minkowski
- Scale, standardize, or normalize as necessary
- Establish a base case (e.g., 1 cluster)

### Methods
- Selection of K (# of clusters)
    - Scree plot
    - Calinski Harabasz criteria
    - Average silhouette width
    - *clusterCrit package has 40 clustering criteria*
- K-means
    + With random restarts
    - Entropy weighted k-means?? *ewkm() in wskm package for R*
    - Subspace clustering??
    - Bicluster analysis??
- Expectation-Maximization (EM) with random restarts
- General clustering with randomized optimization
- Hierarchical clustering
    - Single link
    - Average link
    - Complete link
    - *amap package for R*
    - By missing-ness, using binary indicator values (*mona() in R*)
- Partitioning around mediods (PAM)
- Self organising maps (*kohonen package in R*)

### Evaluation
- Visualizations
    - Silhouette plot
    - Radial plot
- Assess cluster stability
- Cluster quality metrics
    - Label independent
        - Sum of square error
        - Silhouette coefficient
    - Label dependent
        - Adjusted mutual information
        - Adjusted Rand index
        - Homogeneity
        - Completeness
    - Learner performance (regression, classification, etc.)
    - *clusterCrit pacakge has 40 clustering criteria*

## Association rules mining

## Anomaly detection

# Supervised learning: classification and regression
- Anomaly detection
- SVM
- Generalized linear models (logistic regression)
- Naive Bayes
- Perceptron
- Neural network
- Decision trees
- Random forest
- Gradient boosting machine
- General linear models (linear regression)
- Ranking
- Collaborative filtering

# Reinforcement learning
- Markov decision processes
- Value iteration
- Policy iteration
- Q-learning
- SARSA
- TD learning
- Game theory

# Meta methods and algorithms
- Bagging (bootstrap aggregating)
- Boosting
- Blending (stacking, stacked aggregation)
- Ensemble learning

# Time series analysis
- Forecasting
- Breakout, change analysis
- Anomaly detection

# Text mining and NLP
- Viterbi algorithm
- TF-IDF
- Latent dirichlet allocation (LDA)
- Latent semantic indexing/analysis (LSI/A)
- Viterbi algorithm
- Baum-Welch algorithm
- Named entity recognition
- WordNet
- Term-document matrix (thesis on matrix based methods)
- Sentiment analysis
- Vowpal Wabbit
- NLTK

# Network analysis

# Visualization
- Univariate, bivariate, multivariate
- Data exploration
- Scatter plots
- Spatial charts
- 3D charts
- interactive visualization
- d3.js, plot.ly, Shiny, ggplot, matplotlib

# Optimization
- Randomized hill climbing
- Simulated annealing
- Genetic algorithms
- Gradient descent
- Newton-Raphson method
- Broyden-Fletcher-Goldfarb-Shanno (BFGS) algorithm
- Simplex algorithm
- Linear programming
- Nonlinear programming
- Dynamic programming
- Convex and nonconvex optimization

# Statistics
- Basic descriptive statistics
- ANOVA
- Bayes Theorem
- Histograms
- Skewness
- Moments
- Continuous distributions
- Discrete distributions
- Probability theory
- Central limit theorem
- Statistical significance, p-value, chi square
- MLE and MAP estimates
- Hypothesis testing
- Monte carlo method
- Kernel density estimation
- Correlation: Pearson, etc.
- Causation
- Causal analysis

# Big Data
- Map Reduce
- Hadoop and HDFS
- Hive
- Apache Spark
- Memory efficient approaches

# Learning theory
- Bias-variance trade-off
- Overfitting
- Lift
- VC dimensions
- PAC learning

# Mathematics fundamentals
- Linear algebra
- Calculus

# Computer science fundamentals
- Hash functions
- Complexity
- Algorithms

# Simulation
