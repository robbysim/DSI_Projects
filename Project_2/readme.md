# General Assembly DSI-18 Project 2

## Ames House Price Analysis

### Problem Statement

The Executive Committe of the Iowa Real Estate Investment Fund (IREIF) identified Ames as a high potential target to invest in. As part of the investment team in IREIF, we seek to understand why real estate in Ames is attracting attention as well as develop a model to predict the intrinsic value of houses in Ames so that the fund is able to make targeted investments and generate returns for our investors.

### Executive Summary

Ames City is voted as the 9th best suburban city to live in and housing prices have shown a good resistence to the US Subprime Crisis. We explore approximately 2,500 housing transactions from the 2006-2010 period and identify features that were subsequently used in our regression models to assist in predicting the intrinsic value of the house. Our final model has good predictive accuracy up till the $300,000 valuation, thereafter, the predictions tend to under-predict actual house prices. Nonetheless, we believe the model is still useful in that it provides a margin of safety in predictions and will be a good tool to generate investment returns.


### Overview of the Analysis

Our dataset consists of 2051 housing transactions in Ames, Iowa spread across 2006-2010. Each transaction is unique and there were no repeated transactions for the same house in our dataset. Additionally, each transactional sale price is accompanied by 80 other columns detailing the features of the house. Through visualization techniques, including histograms, boxplots, scatterplots, correlation heatmaps, we seek to identify key features that will help us better predict sale prices.

With the selected features, we conducted a validation of our multiple linear regression model and further used Ridge, Lasso and ElasticNet Regularization Models to regularize our linear regression model to prevent overfitting. Our final Lasso model regulated 6 features out from our initial selection, and shown good predictive ability up till the $300,000 price range. 


### Conclusions

We believe our Lasso model is able to achieve high predictive powers below the 300,000 valuation, evidenced by how close the actual sale prices are to the prediction line. Also, we have avoided overfitting our model by not including many of the correlated features as well as polynomial and interactive terms that may make the model unwieldly and difficult to interpret.

Any predictions that are above the 300,000 valuation mark should be treated with caution as our model tends to under-predict the actual values. However, it might not be a huge problem if we were to seek real estate investments, as we will then obtain a margin of safety from the supposedly true value of the house. Additionally, one important factor that our model's prediction power is decreased is due to the lower number of observations above this price range. 

To improve our model, an immediate and direct method would be to collect more data, especially in the 300,000 and above valuation range. This will allow our model to better learn and generate predictions. Additionally, this will also allow us to see if other features can be included that will further explain house prices for this price range.


### Sources, Data Source & Documentation

[Kaggle Data Source](https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/submissions?sortBy=date&group=all&page=1&pageSize=100) <br>
[Data Documentation](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt) <br>
[Research paper by Author (Dean De Cock)](http://jse.amstat.org/v19n3/decock.pdf) <br>
[Ames voted as the 9th best small cities](https://money.cnn.com/magazines/moneymag/bplive/2010/snapshots/PL1901855.html) <br>
[US Census Bureau for demographics on Ames](https://www.census.gov/)  <br>
[Information on Ames](https://www.cityofames.org)   <br>
[Information on Properties](https://beacon.schneidercorp.com/) <br>

