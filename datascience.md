By **Victor**

# Useful resources

## R
- [RStudio](http://www.rstudio.com/): popular IDE for R
- [CRAN](http://cran.r-project.org/): repository of R packages
- [caret](https://topepo.github.io/caret/index.html): library with supporting functions for machine learning
- [ggplot2](http://ggplot2.org/): visualization library based on the grammar of graphics
- [dplyr](http://goo.gl/87ZM57): library for manipulating data frames
- [tidyr](http://goo.gl/87ZM57): library for tidying up messy data

## Python
- [Scikit](http://scikit-learn.org/stable/index.html): popular machine learning library with great documentation
- [Numpy](www.numpy.org/), [Scipy](www.scipy.org), and [Matplotlib](http://matplotlib.org/): popular packages for scientific computing and visualization
- [Pandas](http://pandas.pydata.org/) for data frames
- [IPython] (http://ipython.org/): Python interpreter with lots of nifty features, including [IPython Notebook](http://goo.gl/dY3RQ) 
- [Spyder](https://github.com/spyder-ide/spyder): IDE for scientific computing in Python
- [Pycharm](https://www.jetbrains.com/pycharm/): General purpose Python IDE
- [Sublime Text](https://www.sublimetext.com/): General purpose text editor, commonly used for programming and development

## Java
- [Weka](http://www.cs.waikato.ac.nz/ml/weka/)
- [ABAGAIL](https://github.com/pushkar/ABAGAIL)

## Reading
- [Booz Allen Hamilton Field Guide to Data Science](http://goo.gl/G5vggo)
- [Hands-on Data Science with Togaware](http://onepager.togaware.com/)
- [Coursera machine learning course by Andrew Ng](https://www.coursera.org/course/ml)
- [“Machine learning” by Tom Mitchell](https://www.cs.cmu.edu/~tom/mlbook.html)
- ["The elements of statistical learning" by Hastie, Tibshirani, and Friedman](http://statweb.stanford.edu/~tibs/ElemStatLearn/)

# Pre-processing
## Data munging
Put data in a usable format, e.g. table or data frame

## Data cleaning
- Normalize variable names
- Select candidate features
- Correct data formats, i.e. numeric, categorical
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

# Descriptive analytics
## Clustering

### Two questions
1. What clustering helps us distinguish between real and fake hotels?
2. What clustering helps us distinguish between different activities, in general?
3. How to deal with missing or categorical data?

### Set-up
- Choose distance metric, e.g. Euclidean or Manhattan (or more generally L-norm), Mahalanobis, Minkowski
- Scale, standardize, or normalize as necessary
- Establish a base case (1 cluster)
-

### Methods
- Selection of K (# of clusters)
    - Scree plot
    - Calinski Harabasz criteria
    - Average silhouette width
    - *clusterCrit package has 40 clustering criteria*
- K-means with random restarts
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

## Association analysis
## Anomaly detection

# Predictive analytics
## Anomaly detection
## SVM
## Logistic regression
## Naive Bayes
## Neural network
## Decision trees
## Random forest
## Ensemble methods
