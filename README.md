# Analysis of Wine Quality and Chemical Components

Wine quality is normally a very subjective measurement. There are many types of wines available and people have can have very different tastes. But is there a way to use objective measurements to predict a wine's quality? This analysis attempts to answer the following questions using wine chemical measurements and expert quality ratings.

1. Which chemical feature has the most negative effect on a wine's quality?
2. Which chemical feature has the most positive effect on a wine's quality?
3. What other information could be used or is important to consider when attempting to predict wine quality?
4. How can those in the wine industry use this information to their benefit?

## Files:

* 'WineQualityAnalysis.ipynb' - Notebook with analysis code and results.
* 'winequality-red.csv' - Data source for analysis.

## Data Collection:

The data for this project was collected through the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/wine+quality)

The data was collected by researchers at the University of Minho in Portugal. It contains chemical inputs of red variants of "Vinho Verde" wine, so named due to the region it hails from in Portugal. The dataset consists of 11 chemcial measurements, and 1 output variable, the quality rating as a score between 0 and 10. Full list of the variables is below:

Input variables (based on chemical tests):
- fixed acidity
- volatile acidity
- citric acid
- residual sugar
- chlorides
- free sulfur dioxide
- total sulfur dioxide
- density
- pH
- sulphates
- alcohol

Output variable (based on sensory data):
- quality (score between 0 and 10)

The dataset unfortunately does not include other information such as grape types, brand, or price due to data privacy concerns.

For more information on how the original dataset was created, reference the below paper:

[P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis.
Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009](http://dx.doi.org/10.1016/j.dss.2009.05.016)

## Python Libraries:

This analysis makes use of the following python libraries:

* `matplotlib`
* `mord`
* `numpy`
* `pandas`
* `seaborn`
* `sklearn`

## Analysis Summary:

This analysis approaches the problem by using an ordinal regression method to predict the resulting quality rating based on the chemical inputs. The model resulted in an accuracy of 58%, with the most impactful features being volatile acidity, chlorides, sulphates, and alcohol as determined by their coefficients. Additional information and results are described in the analysis notebook.