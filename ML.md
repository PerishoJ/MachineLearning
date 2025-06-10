######################################
## Machine Learning
######################################

# 4 Pillars of Machine Learning
- Regression - 
    vector calc. , linear alg.
- Dimensional Reduction 
    prob. and Anlytc geo
- Density Estm. - 
    prob. and Anlytc geo
- Classification - 
    optimization matrx decomposition

# Types of Learning Methods
- Supervised (labeled data)
  - Classification
    - KNN
    - Logistic Regression
    - SVM
    - CART
  - Regression
    - CART
    - Linear Regression
    - Ridge Regression
    - Lasso
- Unsupervised (unlabeled data)
  - Clustering (Classification)
    - K-means
    - Hierarchical
  - Dimensionality Reduction
    - PCA
#Data
  __Data__ 
  collection of examples and their features
  Types:
    -Categorical
    - Numerical
  Goal:
  Convert Categorical into numerical: a point in a __Feature Space__

  __Feature Space__ 
  like xfrm actual things into numbers. Like apples = 1, bananas = 2, ripe = 1 , green = 0 , so a fruit could be {fruit, ripeness} -> [1,1] for a ripe banana.

  __bag__
  Database of words. { hello goodbye blue red stop go good bad ... } 

  __text similarity__
    count of each word.

  __Deterministic__
  when the current values can be used to predict a future values.

# Statistics
  ## Measure of Location
    mean
    mode
    median
    quantile
  ## Measure of spread
    rng
    std dev
    IQR (interquartile Range) 

# What we do w/ statistics
  __Histogram__
  an estimate of the probability density func
  create bins - rng of values divided by num of intervals

In ML , we want to know the prob. dens. func. (PDF) of the data
  __parametric density estimation__ 
  We guess which parametric density function it is.
  e.g. gaussian, exponential, poisson, or linear.

  __non-parametric density estimation__
  TBD

# Measures of RND
## Histograms - again
  idea about the statistical behavior of problm
  ~ an approx. of PDF
  these funcs are non-negative and may be defined over 
  - The volume under this function is probability
  - for a vector, we have a dimensional function 


__Covariance Mtrx__
  variables on each axis, the cross is a number 0.0 - 1.0 describing relationship. 1 being 100% correlated. 0 meaning not related at all.

## Entrpy
  
  positive value > 0
  0 is no entropy, perfectly predictable
  
# Cleaning
  NMOD - mnemonic 'not my other dad'
  noise , missing values , outliers , duplicates

# Linear Algbra
  
__Eigen value Decomposition (EVD)__
  xfrm a matrix to another w/ uncorrelated elements
  ¿ Finding a list of things that just don't affect each other...maybe they are useless??? Lol

    __Hermition matrix__
    ¿ What ?     
  
__Singular Value Decomposition (SVD)__
  what if matrix is singular, not square  ( what is a singular matrix? Sqr mtrx? )
  Unitary Matix ?

__Principle Component Analysis (PCA)__
    - reduce dimensionality
    - data visualzn
    - data preprocessing ( use in ml algos)
    - correlation ID

# Data models & Lrng
  feature map leads to a "Kernal" in deep learning ( What is a kernal?)

  Learning = finding parameters

  # 3 phases Lrng
    1) prediction or inference
    2) Traing or Param Est.
    3) Hyper param . Tuning Or Model Selection

  Deterministic or probabistic model??? importatnt to know

  ## Empirical Risk Minimization (ERM)
    Loss function for Training
    bld a predictor to min. rsk in mk decisn.

  ## Cross Validation -> assess general perf.


# Parametric Estimation

## MLE
  asymptotically efficient ... ?? not realistic in some problems
  suffers overfitting problms
  if Noise isn't Gaussian, MLE is bad
  Assumes param isn't rnd
  If param IS rnd, us __Maximum A-posteriori estimate (MAP)__

## Maximum A Posteriori Estimate
  

## Parametric Density Estimation


# Model FItting - over fitting and underfitting

## Probabistic Models
__Bayesian inference__
  make a full posteriori distribution
    -> this distro. is used for decision making

## Linear Regrssn
  ... Stopped here. Wtf am I learning???



################################################
## Questions
################################################

- Data Cleaning
  - Are we going to learn some practical stuff here? What should we know?

 
################################################
## Left Off 
################################################
Eigenvalue Decomposition (EVD) pg 24


################################################
## META
################################################
- Integral Symbol ∫
  Ctrl-K In 
  ∫
- Upside-down Question Mark
  Ctrl-k ?I
  ¿
