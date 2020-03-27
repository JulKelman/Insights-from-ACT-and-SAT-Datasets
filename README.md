# Where Should the ACT Spend Money? 
## Insights from 2017/2018 ACT and SAT Datasets 
---
#### Julia Kelman: [GitHub](https://github.com/JulKelman)  
  
  
## Problem Statement
---
The goal of the ACT team is to constantly improve the participation rates in order to have the most accurate representation of the U.S high school graduate population, which in term increases the value of our standardized test.
As part of the ACT data team, we need to identify states where money would be needed this year to improve ACT participation rates.

## Executive Summary 
---
Our goal is to identify states where investment would be needed to improve ACT participation rates. In order to do so, four datasets were used: the [2017 SAT Scores](https://git.generalassemb.ly/julia-kelman/project_1/blob/master/data/sat_2017.csv), the [2017 ACT Scores](https://git.generalassemb.ly/julia-kelman/project_1/blob/master/data/act_2017.csv), the [2018 SAT Scores](https://git.generalassemb.ly/julia-kelman/project_1/blob/master/data/sat_2018.csv), and the [2018 ACT Scores](https://git.generalassemb.ly/julia-kelman/project_1/blob/master/data/act_2018.csv). The SAT datasets list the 50 U.S state and the federal district District of Columbia. For each of those, the participation percentage, the scores for the evidence based reading and writting and math portions of the test, as well as the total scores are provided. The ACT datasets list the 50 U.S state and the federal district District of Columbia. They provides the participation percentage and composite scores for each state. In addition, the 2017 ACT dataset provides the english, math, reading and science scores for each state and the national averages. The four dataframes were cleaned and merged into one [final dataframe](https://git.generalassemb.ly/julia-kelman/project_1/blob/master/final.csv). The final dataset contained every feature from the original datasets for each of the 50 U.S states and the federal District of Columbia.  
Exploratory analysis including summary statistics was performed to identify trends in the data. Data visualization tools were then used to visualize those trends and outside research was done to put those trends into context. Trends for three specific states emerged as particularly interesting and recommendations were made to allocate part of this year's budget to Colorado, Florida, and Georgia. 

## Contents:
---
- 2017 Data Import and Cleaning
- 2018 Data Import and Cleaning
- Exploratory Data Analysis
- Data Visualization
- Outside Research
- Conclusions and Recommendations

## Project Files 
---
- [2017 SAT Scores](https://git.generalassemb.ly/julia-kelman/project_1/blob/master/data/sat_2017.csv)  
- [2017 ACT Scores](https://git.generalassemb.ly/julia-kelman/project_1/blob/master/data/act_2017.csv)
- [2018 SAT Scores](https://git.generalassemb.ly/julia-kelman/project_1/blob/master/data/sat_2018.csv)
- [2018 ACT Scores](https://git.generalassemb.ly/julia-kelman/project_1/blob/master/data/act_2018.csv)
- [final dataframe](https://git.generalassemb.ly/julia-kelman/project_1/blob/master/final.csv)

## Data Dictionary 
---
|Feature|Type|Dataset|Description|
|:---|:---:|:---:|:---|
|state|object|ACT & SAT|State name.| 
|sat_2017_participation_percentage|float|SAT|Percentage of graduates in the class of 2017 who took the SAT during high-school.|
|sat_2017_evidence_based_reading_and_writing|int|SAT|Average score obtained by the 2017 high school graduates on the evidence-based reading and writing section of the SAT. Students must have taken the SAT during high school. If a student took the SAT more than once, the most recent score was used.|
|sat_2017_math|int|SAT|Average score obtained by the 2017 high school graduates on the math section of the SAT. Students must have taken the SAT during high school. If a student took the SAT more than once, the most recent score was used.| 
|sat_2017_total|int|SAT|Average total SAT score obtained by the 2017 high school graduates who took the SAT during high school. If a student took the SAT more than once, the most recent score was used.|
|act_2017_participation_percentage|float|ACT|Percentage of graduating seniors from the class of 2017 who took the ACT.|
|act_2017_english|float|ACT|Average score obtained by the 2017 graduates on the english section of the ACT.|
|act_2017_math|float|ACT|Average score obtained by the 2017 graduates on the math section of the ACT.|
|act_2017_reading|float|ACT|Average score obtained by the 2017 graduates on the reading section of the ACT.|
|act_2017_science|float|ACT|Average score obtained by the 2017 graduates on the science section of the ACT.|
|act_2017_composite|float|ACT|Average composite score obtained by the 2017 graduates on the ACT.|
|sat_2018_participation_percentage|float|SAT|Percentage of graduates in the class of 2018 who took the SAT during high-school.|
|sat_2018_evidence_based_reading_and_writing|int|SAT|Average score obtained by the 2018 high school graduates on the evidence-based reading and writing section of the SAT. Students must have taken the SAT during high school. If a student took the SAT more than once, the most recent score was used.|
|sat_2018_math|int|SAT|Average score obtained by the 2018 high school graduates on the math section of the SAT. Students must have taken the SAT during high school. If a student took the SAT more than once, the most recent score was used.| 
|sat_2018_total|int|SAT|Average total SAT score obtained by the 2018 high school graduates who took the SAT during high school. If a student took the SAT more than once, the most recent score was used.|
|act_2018_participation_percentage|float|ACT|Percentage of graduating seniors from the class of 2018 who took the ACT.|
|act_2018_composite|float|ACT|Average composite score obtained by the 2018 graduates on the ACT.|

## Main Observations in Context
--- 
**Colorado**: The extreme changes in participation rates for the ACT and SAT between 2017 and 2018 are indicators of a major event. Indeed, our outside research reveiled that the state requirements have changed. Colorado used to require its high school graduates to take the ACT. However, effective in 2018, it now requires its students to take the SAT. This explains the large decrease in ACT participation rates from 100% to 30%, and the increase in SAT participation rates from 11% to 100%. [Source](https://www.testive.com/colorado-sat-change-2017/)

**Florida**: From 2017 to 2018 there is a sharp decrease in SAT participation rates (from 83% to 56%) and a small decrease in ACT participation rates (from 73% to 66%). As the ACT and SAT participation rates are negativelly correlated, a decrease in both states is interesting. Our outside research reveiled that the state of Florida requires high school students to take either the SAT, ACT, or the Florida Standards Assessments (FSA) in order to graduate. This third state specific test is a confounding variable that could have affected the trends in SAT and ACT participation rates. [Source](https://www.edweek.org/ew/section/multimedia/states-require-students-take-sat-or-act.html)
    
**Georgia**: From 2017 to 2018 the Georgia SAT participation rates increased from 61% to 70% while the ACT participation rates decreased from 55% to 53%. According to our outside research, Georgia has no state requirements concerning standardized testing for graduates. Given this information, this trend in participation rates is interesting because it suggests that more students are taking standardized tests, however they are opting for the SAT rather than the ACT. [Source](https://www.edweek.org/ew/section/multimedia/states-require-students-take-sat-or-act.html)

## Conclusions/Recommendations 
--- 
**Recommendation 1:** Invest in Colorado in order to counteract the effects of the state requirements change. While we used to have a near perfect representation of the high school graduate student population in Colorado, the change in state requirements significantly impacts the accuracy of our representation going forward. As a result, we recommend to allocate a portion of this year's budget to fighting this change. 

**Recommendation 2:** The sharp decrease in Florida's SAT participation rates between 2017 and 2018 accompanied by a lack of increase in the ACT participation rates during that time frame suggest a potential oppotunity for improvement. As a result, we recommend to invest in Florida to proactivelly try to convert those students who are no longer taking the SAT into ACT test takers. In addition, the lack of strict state requirements in Florida eliminates many hurdles and leave the doors open for an increase in ACT participation rates. 

**Recommendation 3:** The increase in SAT participation rates and decrease in ACT participation rates seen in Georgia are indicators of a potential issue. Indeed, this suggests that more students may be taking standardized tests in general in this state, but they seem to select the SAT as their test of choice. This is worrisome for two reasons:  
1. We are missing out on potential new test takers   
2. As the SAT participation rates and ACT participation rates are negatively correlated, if the SAT participation rate keeps increasing we are likely to see a further decrease in the ACT participation rates.  

For those reasons, we recommend to allocate a portion of this year's budget to fight those trends in Georgia. 


