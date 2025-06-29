-------------------------------------------------------------------------------
Overview of Deep Learning
-------------------------------------------------------------------------------
wht is dl?
  layers of neural nets.
  MANY MANY layers of artificial neurons.
  feature extraction AND classification happen at the same time.


e.g.
  AtomNet for drug design, GNoME for matrl scnce, graphCast for weather

types of ML.
# Supervised
  Use Cleaned Data. Labeled
  Types of Labels: 
    - Discrete (cat vs dog) (classification)
    - Continuous (house prices) (regression)
# Unsupervised -
 Unlabed dataset, find patterns
  group similar sets (clustering)
  compressing features (dimensionality reduction)
# Reinforcement -
 reward & penalty when interacting w/ env. Trial/Error.
  Agent & Environment
  Reward and Punishment
  Mapping States -> best actions; Policy

# Data
  
# Why Now?
  because we have more data available.
  we have much better hardware to make it happen.
  ## GPU's
    Tensor Cores


-------------------------------------------------------------------------------
Feature Extraction and Data Conditioning
-------------------------------------------------------------------------------
feature - any measurable attribute of data.
  - choosing features is important
  - choosing data is important. Garbage in, garbage out.

# Data Conditioning
  clean it up a little bit before your traing.
  
# Missing Data
  many rows are missing data
  solns.
  - NOT time dependent? Remove
  - median or mean values.
  - else, interpolate
     - linear, cubic, polynomial

# Outliers
  remove them, usually
  probably badly measured data point. 

# Augmentation
  create new training samples by applying xfrms to existing samples.
  Rich dataset -> Need This
  - increase variability in data: address variations model may encounter
  - balanced classes: gen. more samples for low-ample classes
    - unbalanced data (not enough samples for edge cases) makes bad models.

  ## Augmentation Techniques
    Geo
      rotation, scale, translate, flip
    photometric
    ...
    etc.

  ## Synthetic but Realistic Data
    VERY helpful with sparse data

  ## Normalization
    scaling features to a common range
    learning by distance measure -> if two features on different scales, one will dominate the other feature. Not good.

    - Min-max normalization

    - z-score standardization

# Dimensionality Reduction
  too many features? reduce.
  more features != better model
  - too many features
    - clutter and redundancy
    - slows down training
    - hard to find data points with all that data (you have to measure more)

  ## Principle Component Analysis (PCA)
    Eigenvectors of Covarience Matrix.
      - tip: Use the features w/ most variation.
    ~ looking for flow dir.    

  ## Linear Discriminant Analysis (LDA)
    aka, fischer discriminant

    Maximize class separability
      ~ kind of finding clumps of data and drawing lines to separate them.
    ~ looking for clumps
    
  # Good Book
      Machine Learning with Python ~ amin zollanvari  
   ?? still don't know how to calculate for hi-dim eigenvalues. Maybe not imprt

  
-------------------------------------------------------------------------------
Probability and Bayesian Learning
-------------------------------------------------------------------------------
  Probability is what we use for learning.
  
  Conditional Probability - how often evenat A occurs given that event B has occurred.

  Bayes' Rules indicates how to update the probability based on the new observation.

  e.g. If we have to buckets, one with apples and one with pears....if what I picked up is an apple, then it came from the bucket with apples.
  but, generalized with probabilities.

# Bayesian ML
  density functions. 

# How Figure out F(x)

  some curve fitting algo's in prob.

  # Chi-Square Test
  See how well a distro. fits a data set.

  split into bins for each.
  check datapoints in each bin
  
  ## Two Density Estimations
    - Parametric (Maximum Likelihood Estimation (MLE))
      - aka Training.

    - Non-Parametric (Parzen Window, K-Nearest Neighbor) 
   
  slide 73, the pi symbol???

# Parzen
    Histogram
    (# samples in a particular bin) / (total # samples) = P(x)
    
    How does this work in higher dimensions??


    Key takeaway: more data is much better. Otherwise, algo will make artificial spikes and valleys.


# K-Nearest Neighbor
  

In Practice Tips
  use parametric w/ not many samples
  use non-parametric w/ LOTS of samples


