# Project 1: SAT & ACT Analysis


## Problem Statement

SAT and ACT are used for US college application. They attempt to measure an individual college readiness and predict future academic success. As we are administering the SAT test, our direct competitior will be the ACT, Inc whom is administering the ACT test. Therefore, in this project, we will be looking at how to improve the particiation of SAT test across the 51 states in USA and, how we can put our funds to better use.

## Executive Summary
We will be using the datas of ACT and SAT in both 2017 and 2018 for the project. Data such as participation rates and tests mean scores are used for comparison and analysis. In this analysis, we will be looking for the trends and relationships between the features in both years and in different states. Some sources from outside research will be taken, to better understand the policies and requirements for education in different states. With these information, we will be making recommendation for which state to start improving on.


## Contents:

1. [Datasets Used](#1-Datasets-Used)
2. [Data Dictionary](#2.-Data-Dictionary)
3. [Exploratory Data Analysis](#3.-Exploratory-Data-Analysis)
4. [Data Visualization](#4.-Data-Visualization)
5. [Descriptive and Inferential Statistics](#5.-Descriptive-and-Inferential-Statistics)
6. [Outside Research](#6.-Outside-Research)
7. [Conclusions and Recommendations](#7.-Conclusions-and-Recommendations)
8. [References](#8-References)
9. [Python Library Used](#9.-Python-Library_used)

### 1. Datasets Used :

The following datasets were used for this projects:
- ACT 2017
- SAT 2017
- ACT 2018
- SAT 2018

The following datasets were created and used during the projects:
- Combined 2017 (Combination of ACT and SAT 2017 data)
- Combined 2018 (Combination of ACT and SAT 2018 data)
- Final (Combination of all data)

### 2. Data Dictionary:

The below is a data dictionary containing all the data features, type and its description:

|Feature|Type|Dataset|Description|
|:---:|:---:|:---:|:---:|
|state|object|ACT/SAT|State
|act2017_participation|float64|ACT|ACT 2017 Participation Rate
|act2017_english|float64|ACT|ACT 2017 English Mean Score
|act2017_math|float64|ACT|ACT 2017 Math Mean Score
|act2017_reading|float64|ACT|ACT 2017 Reading Mean Score
|act2017_science|float64|ACT|ACT 2017 Science Mean Score
|act2017_composite|float64|ACT|ACT 2017 Composite Mean Score
|sat2017_participation|float64|SAT|SAT 2017 Participation Rate
|sat2017_ebrw|float64|SAT|SAT 2017 Evidence-Based Reading and Writing Mean Score
|sat2017_math|float64|SAT|SAT 2017 Math Mean Score
|sat2017_total|float64|SAT|SAT 2017 Total Mean Score
|act2018_participation|float64|ACT|ACT 2018 Participation Rate
|act2018_english|float64|ACT|ACT 2018 English Mean Score
|act2018_math|float64|ACT|ACT 2018 Math Mean Score
|act2018_reading|float64|ACT|ACT 2018 Reading Mean Score
|act2018_science|float64|ACT|ACT 2018 Science Mean Score
|act2018_composite|float64|ACT|ACT 2018 Composite Mean Score
|sat2018_participation|float64|SAT|SAT 2018 Participation Rate
|sat2018_ebrw|float64|SAT|SAT 2018 Evidence-Based Reading and Writing Mean Score
|sat2018_math|float64|SAT|SAT 2018 Math Mean Score
|sat2018_total|float64|SAT|SAT 2018 Total Mean Score

### 3. Exploratory Data Analysis

In this section, we came up with a function to calculate standard deviation manually, not using pandas or numpy library. Then,we will investigate the trends in the data. The following are the different data we worked on:

- States with highest and lowest participation rates for both tests in both years
- States with the highest and lowest composite/total scores for the both tests in both years
- States with full participation rates on both tests that have a rate change year-to-year
- States that have more than 50% participation on both test in both years
- States with ACT 100% participation rate, to find out the participation rate for SAT tests
- States with SAT 100% participation rate, to find out the participation rate for ACT tests
- District of Columbia's comparison on SAT participation rate and SAT total score.
- Nevada's comparison on ACT participation rate and ACT composite score.
- Minnesota's comparison on both tests participation rates and total/composite score.

### 4. Data Visualization

In this section, plotting of different type of diagrams were used to study and visual the trend data more. Functions were built for different methods of plotting.The following are the different methods used:

##### Heatmap
 - The correlation of SAT and ACT mean data for both years

##### Sub-plotting of Histograms
 - SAT's and ACT's participation rates for 2017 and 2018
 - Math scores for SAT and ACT for 2017 and 2018
 - Reading and verbal scores for SAT and ACT for 2017 and 2018

###### Scatter plotting
- SAT vs ACT math scores for 2017
- SAT vs ACT verbal/reading scores for 2017
- SAT vs ACT total/composite scores for 2017
- Total scores for SAT 2017 vs 2018
- Composite scores for ACT 2017 vs 2018
- SAT participation rate & total score in 2017
- SAT vs ACT participation rate for 2017

##### Box plotting
- SAT VS ACT participation rate for 2017 and 2018
- SAT evidence-based reading and writing scores for 2017 and 2018
- SAT math scores for 2017 and 2018
- SAT total scores for 2017 and 2018
- ACT english scores for 2017 and 2018
- ACT reading scores for 2017 and 2018
- ACT math scores for 2017 and 2018
- ACT science scores for 2017 and 2018
- ACT composite scores for 2017 and 2018

### 5. Descriptive and Inferential Statistics

In this section, a summary of the distributions were done up. The central tendency, spread and skewness are being summarized and compared between each data. Then, Central Limit Theorem was tested on the following data:

- ACT and SAT math scores for 2017 and 2018
- ACT reading scores for 2017 and 2018
- SAT evidence-based reading and writing for 2017 and 2018
- ACT and SAT participation rates for 2017 and 2018

The tests are to prove on the assumption assumption on application of Central Limit Theorem, which will return a population with normal distribution.

We are seeking to understand the relationship between SAT and ACT participation rates in 2017. Reasoning on whether to conduct statistical inference on the two data.

Math scores between SAT and ACT were also being reasoned whether it is being fair to be compared on the terms of students with higher SAT math score is better than those with lower ACT math score or vice versa.


### 6. Outside Research

Additional outside research is done on three states; Nevada, District of Columbia and Minnesota. Research is also done on states which candidates are able to take SAT or ACT for free or subsidized rates. For the three states mentioned, ACT or SAT is optional for entry to university or high school.

### 7. Conclusions and Recommendations

After the analysis and visualization of data, some trends were found.

1) There seemed to have a negative correlation of ACT participation rate and SAT participation rate. It seemed that if a candidate were to take SAT, he/she will not take ACT in the same year, vice versa.

2) Participation rates for both tests have a negative correlation with their respective composite/total scores. When the participation rate increases, the scores will decrease.

3) Positive correlations were found in both tests' composite/total scores with their sub-tests scores.

To improve our SAT participation, I will recommend to concentrate on states that do not have a high ACT participation but a very low SAT participation.

An example will be Iowa. The table above shows both tests participation in both year. The ACT 2018 participation rates increased by 1 from 2017. The SAT 2018 partcipation rates increases by 1 as well. The ACT 2018 composite score decreased by 0.1 as compared to 2017. The SAT 2018 total score decreased by 10 as compared to 2017. These two decreases in both tests composite and total score proved the negative correlation with the participation rate of the tests.

From outside research, it is not free to take either test in the state. To enter the university of Iowa, the applicant will require a ACT composite score of 26 or SAT total of 1230.

A recommendation will be to work with the Iowa's education board for subsidized SAT tests. As Iowa's median household income is lower than the national's median household, it might be able to help some students. The schools can also implement SAT to be taken on school days, students might treat it as part of the curriculum.

It might help in encouraging more students to enter college after high school. Based on sources from United States Census Bureau, the education attainment for high school or higher in Iowa is 92.6%, however 31% is only from high school. Therefore, more SAT participation will encourage them to enter college as SAT is one of the requirements.


### 8. References

###### College Raptor is used to find out on the states which subsidize ACT or SAT:
https://www.collegeraptor.com/getting-in/articles/act-sat/states-act-sat-given-free/

###### University of Nevada, Reno's entry requirements:
https://www.unr.edu/admissions/undergraduate/freshman/requirements#:~:text=Standardized%20test%20scores%20are%20not%20required%20for%20admission%20to%20the,placement%20in%20first%20year%20courses

###### University of District of Columbia's entry requirements:
https://www.udc.edu/admissions/information-for-college-advisors/#:~:text=Admissions%20Process,There%20are%20slight&text=In%20general%2C%20UDC%20requires%20students%20to%3A&text=Submit%20official%20SAT%20or%20ACT,other%20colleges%20or%20universities%20attended

###### University of Minnesota's entry requirements:
https://admissions.tc.umn.edu/freshman/test_requirements.html

###### University of Iowa's entry requirements:
https://admissions.uiowa.edu/academics/first-year-admission

###### Iowa's median household income from United States Census Bureau:
https://www.census.gov/quickfacts/fact/table/US,IA/INC110218

###### Iowa's educational attainment. Source from United States Census Bureau:
https://data.census.gov/cedsci/profile?g=0400000US19


### 9. Python Library Used

- Numpy
- Pandas
- Matplotlib
- Seaborn
- SciPy
