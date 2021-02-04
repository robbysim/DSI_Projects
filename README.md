## Completed Projects Under General Assembly Singapore's Data Science Immersive

### Contents

#### Project 1: 
[Analyzing trends in SAT & ACT scores for 2017 & 2018 - 9 Nov 2020](https://github.com/robbysim/DSI_Projects/tree/main/Project_1)

A dataset consisting of 2017 and 2018 SAT and ACT scores/participation rates across all US states was analyzed using visualization techniques like bar charts, histograms, scatterplots, and correlation heat maps. Additionally, through outside readings and research, I created plotly choroplelth heatmaps showing the changes in SAT and ACT participation rates across the 2 years. 

#### Project 2:
[Ames House Price Analysis - 23 Nov 2020](https://github.com/robbysim/DSI_Projects/tree/main/Project_2)

A dataset consisting of 2,051 housing transactions in Ames, Iowa spread across 2006-2010 was analyzed. Each transaction is unique and there were no repeated transactions for the same house in our dataset. Additionally, each transactional sale price is accompanied by 80 other columns detailing the features of the house. Through visualization techniques, including histograms, boxplots, scatterplots, correlation heatmaps, I identified key features that was selected for the linear regression model. This model was subsequently regulated using Ridge, Lasso and ElasticNet Regularization models. The Lasso model was selected based on the lowest root mean squared error achieved on the validation set. 

#### Project 3:
[Reddit Classification Analysis](https://github.com/robbysim/DSI_Projects/tree/main/Project_3)

2,000 reddit posts each from r/excel and r/vba was scraped from which an eventual combined dataset of about 1,500 was obtained after cleaning duplicated posts. A number of visualization and analysis were done to identified the keywords as well as prepare the dataset for our model by cleaning the posts with regex. The cleaned text is subsequently vectorized into word and trained using a variety of models including Logistic Regression, Multinomial Bayes, Random Forest and Extra Trees while the best model is selected based on our problem statement which was to reduce the number of posts that were actual vba postings but are labelled as excel. Based on a hypothetical annual cost of $500,000 on time wasted to re-classify and match the wrong posts, the final model based on the Multinomial classifier achieves a precision score of 0.89 based on the excel class and thus is able to achieve cost savings of almost $450,000.

#### Project 4:
[West Nile Virus Prediction in the City of Chicago](https://github.com/robbysim/DSI_Projects/tree/main/Project_4)

Group project looking at predicting West Nile Virus (WNV) in mosquitoes caught in traps located in the city of Chicago. Geo-Spatial visualization techniques, using Folium and Geopandas, were done to analyse traps that were most frequently sampled, as well as having high rates of WNV infection. Standard exploratory data analysis was also done to examine mosquito species as well as how weather features impacted the wnv rates and mosquito numbers. Weather features were aggregated into the main training and testing set and final production model was an ensemble of 3 advance tree-based models. Our final model features could be forecast a-priori, leading to a highly effective proactive vector management solution. We also included an analysis of the cost-benefit of spraying based on contracted pricing and benefits derived from studies made into economic losses due to WNV infections. 


#### Capstone:
[Alternative Features in credit lending to better served the unbanked and under-banked population](https://github.com/robbysim/DSI_Projects/tree/main/Capstone)

Final Capstone project examining the impact of alternative features on model scores for credit default predictions. Currently, the underbanked and unbanked population represents a large opportunity for credit lenders to tap into while alternative features have been actively explored as an intellectual property to improve the prediction on default rates for these 2 groups.  The original dataset is split into 4 main customer segments based on whether they are repeat or new customers and whether they have or do not have credit bureau reports. Detailed exploratory data analysis was conducted to observe any trends in the profile of borrowers as well as their corresponding credit default rates. 6 other datasets containing information on loan repayment, credit bureau information as well as credit card usage were aggregated into the main training set compile a complete picture for each borrower based on his/her past borrowing and repayment habits. A number of features were generated and a set of alternative features based on social media, habits and mobile data were identified and analysed based upon their impact on model scoring. 