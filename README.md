# Saudi Traffic Analysis README

### Authors
Murtadha

### Date

16th Mar 2019

### Website
[Analysis of the Saudi Traffic](https://pages.git.generalassemb.ly/Murtadha/project_1/)

---


### Problem Statement

New traffic rules and fines were [implemented in October 2016](http://live.saudigazette.com.sa/article/164574/New-traffic-laws-in-15-days). We are at the General Department of Traffic under the Ministry of Interior, try to track traffic accidents and give policy recommendations that are best to help reduce injuries and casualties on the road. In this project we use data provided by The General Authority for Statistics. Two datasets are in use: a) the number of driving licenses issued between 1993-2016 and b) the accidents and causalities records of the years 2016 and 2017. We try to exploit this data statistically to give practical insights into the subject.

---


### Executive Summary
We start this project by importing the data in its raw format and then do the necessary cleaning to its values and structure. We next ship these cleaned tables to a Python friendly data type. From this point we are ready to do our stats. First, we explore the data using Pandas builtin methods of central tendency mean, median, and mode. Secondly, we investigate trends in the data using the proper plotting libraries. We identify the relationship between different variables of the data and we give the correspondent graphical representations of them. Finally we investigate the distribution of the data and we run hypothesis tests to compare variables of interest in our dataset. At the end we discuss some observations and give stats-based recommendations.

---

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**ta**|DataFrame|--|The dataset for the Traffic Accidents file|
|**dl**|DataFrame|--|The dataset for the Driving Licenses file|
|**mm**|DataFrame|--|The merged DataFrame of *ta* and *dl*|
|year|int Series|dl/ta|The year at which that event happens|
|region|object Series|dl/ta|The region in which that event takes place|
|licenses_count|int Series|dl|The number of deiving licenses (event) issued in that year|
|aciident_info|object Series|ta|The describtion of the event for this row|
|accident_count|int Series|ta|The count for the event given in the indicator col|
|x|object Series|dl/da|The x location coordinate for the region in this row|
|y|object Series|dl/da|The y location coordinate for the region in this row|
---

### Conclusions/Recommendations

**Observations:**

1. Highest populated regions are the highest in the scaled number of accidents. It's expected from these regions to have more strict law enforcement and more traffic eduation, however, it seems that traffic is not effected by both.

2. The incrasing tendency in the number of licenses issued starting from 2005 till 2015 is interesting to study. Further invistigation is needed to see how it's correlated to the placement of the late King Abdullah in this exact period.

3. Driving in SA is very dengerous. Casualities in SA is more likely to be a death case than injury. It would be insightful to compare casualities cases in similar populated countries as SA, and see what's its tendency.


**Additional Data:**

1. It would be more helpful if the data of the SA population is provided, as to find correlations between population and traficc.

2. Any prior data to major traficc law enforcement, like Saher, would beneficial to study its worthy.

3. Data of the distrubution of youth population of SA would give us insight where to start traficc awareness capaign. Also, to correlate accidents with age distribution.
