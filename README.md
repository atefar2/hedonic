# Hedonic Regression
Quick example of using linear regression for real estate valuation for homes in
the Boston suburbs.

## tl;dr
R's [`lm`](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/lm.html) function for linear model fitting was used for a Hedonic regression to predict with fair accuracy the median value of owner-occupied homes. While there was some doubt as to the effect of independent variables `CRIM,` `INDUS`, `AGE` and `B`, a model including all the independent variables available seemed to work best at prediction.

## Data

* Data was obtained on 2016年 9月 22日 木曜日 00:32:22
* URL: https://archive.ics.uci.edu/ml/datasets/Housing
* Number of Instances: 506
* Number of Attributes: 13 continuous attributes (including "class" attribute "MEDV"), 1 binary-valued attribute
* Attribute Information:
  1. `CRIM` ... per capita crime rate by town
  1. `ZN` ... proportion of residential land zoned for lots over 25,000 sq.ft.
  1. `INDUS` ... proportion of non-retail business acres per town 
  1. `CHAS` ... Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
  1. `NOX` ... nitric oxides concentration (parts per 10 million) 
  1. `RM` ... average number of rooms per dwelling
  1. `AGE` ... proportion of owner-occupied units built prior to 1940
  1. `DIS` ... weighted distances to five Boston employment centres 
  1. `RAD` ... index of accessibility to radial highways
  1. `TAX` ... full-value property-tax rate per $10,000 
  1. `PTRATIO` ... pupil-teacher ratio by town 
  1. `B` ... 1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town
  1. `LSTAT` ... % lower status of the population 
  1. `MEDV` ... Median value of owner-occupied homes in $1000's 
* No missing attributes in the data were found 

  

## References
The following references were used in this study, and are also stored under
`doc`.
* [Valuation Using Hedonic Pricing Models](http://scholarship.sha.cornell.edu/cgi/viewcontent.cgi?article=1058&context=crer), Monson, 2009
* [Hedonic Housing Prices and the Demand for Clean Air](http://www.colorado.edu/ibs/crs/workshops/R_1-11-2012/root/Harrison_1978.pdf), Harrison & Rubinfeld, 1978
