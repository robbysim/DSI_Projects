# General Assembly DSI-18 Project 3

## Sub-Reddits Classification Analysis

### Problem Statement

Training a classification model on r/excel and r/vba to better match queries for Excel & VBA Support Company and eventually achieve an annual savings of 500,000 dollars based on man-hour costs for the company. 

### Executive Summary

**Background**<br>
Excel & VBA Support Company is a company that provides specialized support for Microsoft Excel & VBA users. Users post their problem in a query box and a specific (Excel or VBA) specialists are assigned to attend the query and reply (in real-time). <br>

**Issue**<br>
However, the current setup requires manual labelling of the query by users (with manual random checks) on whether it is an Excel or VBA issue and time is wasted if it is mis-classified. Mis-classification is an issue as VBA requires a more specialized product knowledge and product specialists supporting Excel are not necessarily able to support VBA queries. However, the inverse is not true, as VBA product specialists are more likely able to support Excel queries. <br>

Assuming the company receives 1000 Excel queries per day but out of these, 20% are actually VBA queries. Further assuming that redirecting these wrongly classified queries will waste an additional 10 mins (or 1/6th man-hour) for searching and matching to the correct product specialist, there is wastage of 2000 mins (~ 30 man-hours) daily just because the query was mis-classified. Assuming a hypothetical man-hour cost of 50 dollars per man-hour, there is a wastage of 0.5 million dollars per year just due to the mis-classification. <br>

Our model trains on the r/excel and r/vba sub-reddits so that it is able to differentiate among the 2 classes and classify the queries accordingly. We imported the sub-reddits and combined the title and text of each post to form the training and validation sets. Our models consisted of a variety of classification models including, Logistic Regression, Naive Bayes, Random Forests and Support Vectors to see which gives us the lowest false negatives (predicted to be excel query but was in fact a vba query).

### Overview of the Analysis

Our initial dataset scrape using reddit API consists of 1964 and 1993 rows in excel and vba respectively. Both had 105 columns of which we were mainly interested in the title, selftext (actual posts) and created utc (time of post in utc format). We found a number of duplicates which we cleaned out and retrieved only the unique posts. Even in reddit, our problem was evident as we found roughly 7% of the postings to be about vba instead. Once removed, we were left with 752 unique posts and 946 unique posts for excel and vba respectively. 

We analyzed basic trends for the 2 reddits based on timing of posts, title length and text length. Addtionally, we looked at frequent words for each sub-reddits where, unsurprisingly, we found a number of common words shared across both excel and vba. We then proceed to conduct an iterative process to clean the text to be free from symbols, formulas, hyperlinks, and pointer references. 

The cleaned text is then vectorized into individual words and a number of classification models (logistic regression, naive bayes, random forest, support vector machine) were used to determine the best model for our problem. 

### Conclusions

We found our best model to be the Naive Bayes Classifer. Even though its accuracy on the validation set was only 0.836 compared to the highest accuracy of 0.866 scored by the Extra Trees Classifier, our Naive Bayes Classifier achieved the lower False Negative (Actual VBA but Predicted Excel) of 35, and the next best model for False Negative was Logistic Regression with 44 False Negatives and an accuracy of 0.842. 

We further improved our best model by retaining the vba keyword so that our model is able to better recognize and classify vba posts which further reduced our False Negative number down to 23 from the original 35, achieving a reduction of 34%. 



### Sources, Data Source & Documentation

[Excel Sub-reddit](https://www.reddit.com/r/excel/) <br>
[VBA Sub-reddit](https://www.reddit.com/r/vba/) <br>


