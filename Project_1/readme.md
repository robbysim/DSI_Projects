# Reclaiming The Lead
### Back to Relevance for the SAT

The SAT was once the most widely used college admission exam in the US. Designed as an aptitude test to measure intelligence, it was held as a standard on how well a high school student will succeed in college. Since the 2000s and up to 2012, the SAT was losing sight of its relevance at the same time, the ACT, was gaining ground. In 2012, the nationwide participation rates for ACT overtook the SAT for the first time. The College Board sought to implement major design changes to the SAT which was subsequently launched in 2016. With a full year after implementation, we analyze the results and success using the SAT and ACT participation and scoring data by states in 2017 and 2018, and make further recommendations from any insights gained to improve take-up rate. 

### Overview of the Analysis

Our dataset consists of 2017 and 2018 SAT and ACT data for 51 states (plus D.C) in the US. These data points are the aggregated state level data for both years. We combined the datasets into a single dataframe and used simple visualization techniques, including histograms, boxplots, scatterplots, correlation heatmaps and choropleth maps to identify trends and insights. 

Lastly, with the insights gained, including further research on the context, we make recommendations to the College Board to revitalize the SAT. 

### Recommendations

With the insights gained, we identified Arizona as the state where the ACT is not yet entrenched while the SAT is not predominant and introduced strategies that the SAT could gain entry and get entrenched in and subsequently exert dominance. We are hopeful that these strategies, if successful, can be replicated to other states where the SAT is not yet dominant.

### 2017 / 2018 SAT & ACT Data Dictionary

|Feature|Type|Dataset|Description|
|:-|:-|:-|:-|
|**state**|*object*|ACT / SAT|Full name of 51 US states, including District of Columbia (DC).| 
|**sat_xxxx_part**|*float*|SAT|Participation rate of SAT exam for the state. Measured as number of students who took the SAT exam over the total number of eligible students in that state. (units percent, 58.0 means 58.0%). xxxx refers to the particular year of the data, i.e., sat_2017_participation refers to participation rate for year 2017.|
|**sat_xxxx_read_wri**|*intger*|SAT|Average score for the Evidence-based Reading and Writing section of the SAT exam for a particular state. Measured as an integer value from range of min=200 to max=800 inclusive. xxxx refers to the particular year of the data, i.e., sat_2017_reading_writing refers to the reading & writing section score for year 2017.|
|**sat_xxxx_math**|*integer*|SAT|Average score for the Mathematics section of the SAT exam for a particular state. Measured as an integer value from range of min=200 to max=800 inclusive. xxxx refers to the particular year of the data, i.e., sat_2017_math refers to the Mathematics section score for year 2017.|
|**sat_xxxx_tot**|*integer*|SAT|Overall average total score of the SAT exam for the particular state, combining the Mathematics and Evidence-based Reading and Writing section. Measured as an integer value from range of min=400 to max =1,600 inclusive. xxxx refers to the particular year of the data, i.e., sat_2017_total refers to the total score for year 2017. Note that due to rounding, Total can be different from the simple addition of Mathematics section plus Evidence-based Reading and Writing section.|
|**act_xxxx_part**|*float*|ACT|Participation rate of ACT exam for the state. Measured as number of students who took the ACT exam over the total number of eligible students in that state. (units percent, 58.0 means 58.0%). xxxx refers to the particular year of the data, i.e., act_2017_participation refers to participation rate for year 2017.|
|**act_xxxx_eng**|*float*|ACT|Average scaled score for the English section of the ACT exam for a particular state. The raw score for the section is converted to a scaled score from range of min=1 to max=36. Measured as a float value. xxxx refers to the particular year of the data, i.e., act_2017_english refers to the English section score for year 2017.|
|**act_xxxx_math**|*float*|ACT|Average scaled score for the Mathematics section of the ACT exam for a particular state. The raw score for the section is converted to a scaled score from range of min=1 to max=36. Measured as a float value. xxxx refers to the particular year of the data, i.e., act_2017_math refers to the Mathematics section score for year 2017.|
|**act_xxxx_read**|*float*|ACT|Average scaled score for the Reading section of the ACT exam for a particular state. The raw score for the section is converted to a scaled score from range of min=1 to max=36. Measured as a float value. xxxx refers to the particular year of the data, i.e., act_2017_reading refers to the Reading section score for year 2017.|
|**act_xxxx_sci**|*float*|ACT|Average scaled score for the Science section of the ACT exam for a particular state. The raw score for the section is converted to a scaled score from range of min=1 to max=36. Measured as a float value. xxxx refers to the particular year of the data, i.e., act_2017_science refers to the Science section score for year 2017.|
|**act_xxxx_comp**|*float*|ACT|Average score for the Composite section of the ACT exam for a particular state. The individual section scores are averaged to a composite score and scaled from range of min=1 to max=36. Measured as a float value. xxxx refers to the particular year of the data, i.e., act_2017_composite refers to the Composite section score for year 2017.|

### Sources

College Board:
https://about.collegeboard.org/overview
    
    
Background context of SAT & ACT and discussion of statewide contracts:

https://www.applerouth.com/blog/2016/01/13/how-the-sat-got-its-groove-back/

https://www.newamerica.org/education-policy/edcentral/how-college-boards-aggressive-campaign-to-save-the-sat-may-kill-it/

https://www.washingtonpost.com/news/grade-point/wp/2015/12/24/the-sat-now-the-no-2-college-test-pushes-to-reclaim-supremacy/

https://blog.collegevine.com/sat-vs-act-everything-you-need-to-know/

Investigative report on the SAT scandal:

https://www.forbes.com/sites/susanadams/2020/09/30/the-forbes-investigation-how-the-sat-failed-america/?sh=71a076b553b5


SAT School Day and related research:

https://reports.collegeboard.org/archive/sat-suite-program-results/2018/sat-school-day

Alaska's particiation rates:

https://www.adn.com/alaska-news/education/2016/06/30/students-no-longer-need-national-tests-to-graduate/

https://www.govtech.com/education/k-12/Alaska-Education-Department-Looks-for-New-Test-After-Online-Exam-Struggles.html

https://chariotlearning.com/which-states-use-the-sat-or-act-for-state-testing/

Arizonia data & information:
    
https://www.infoplease.com/us/states/state-population-by-rank

https://www.census.gov/quickfacts/AZ

https://azsbe.az.gov/assessments-and-menu-assessments

