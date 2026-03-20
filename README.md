 Wine Quality Signal Decomposition — PCA & ICA

Dimensionality reduction analysis applied to the UCI Wine Quality 
dataset using Principal Component Analysis (PCA) and Independent 
Component Analysis (ICA) in R.

## Dataset
UCI Wine Quality Dataset — Red Wine
1,599 observations, 12 chemical variables including fixed acidity, 
volatile acidity, citric acid, residual sugar, chlorides, 
free sulfur dioxide, total sulfur dioxide, density, pH, 
sulphates, alcohol, and quality score.

## Key Findings
- PC1 explains 94.61% of total variance, dominated by 
  Total Sulfur Dioxide
- PC2 adds 4.835%, bringing cumulative variance to 99.44%
- PC3 through PC12 each contribute less than 1%
- FastICA successfully isolated independent chemical signal 
  sources using logcosh approximation over 26 iterations

## Methods
- Principal Component Analysis (prcomp)
- Independent Component Analysis (fastICA, symmetric method)
- Signal visualization: original, mixed, and ICA source estimates

## Tools
R, fastICA, ggplot2, tidyverse

## Requirements
install.packages(c("fastICA", "tidyverse", "here"))
