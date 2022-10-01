# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis


### Overview

The SAT and ACT are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university.

The SAT has two sections of the test: Evidence-Based Reading and Writing and Math ([*source*](https://www.princetonreview.com/college/sat-sections)). The ACT has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section ([*source*](https://www.act.org/content/act/en/products-and-services/the-act/scores/understanding-your-scores.html)). They have different score ranges, which you can read more about on their websites or additional outside sources (a quick Google search will help you understand the scores for each test):
* [SAT](https://collegereadiness.collegeboard.org/sat)
* [ACT](https://www.act.org/content/act/en.html)

Standardized tests have long been a controversial topic for students, administrators, and legislators. Since the 1940's, an increasing number of colleges have been using scores from sudents' performances on tests like the SAT and the ACT as a measure for college readiness and aptitude ([*source*](https://www.minotdailynews.com/news/local-news/2017/04/a-brief-history-of-the-sat-and-act/)). Supporters of these tests argue that these scores can be used as an objective measure to determine college admittance. Opponents of these tests claim that these tests are not accurate measures of students potential or ability and serve as an inequitable barrier to entry.

### Problem statement

As part of the ad-hoc review of the education system, we (USA Ministry of Education) would like to find out if the current education system in the USA is fair and if not, what can we do to improve the education system. We hypothesize that students from higher household income have better performances on the SAT and ACT, compared to students from lower household income. 

This project seeks to identify if a relationship exists between student annual household income and SAT/ACT scores; and if these tests are a accurate measure of a students' abillity or if there exist a biasness due to socioeconomic differences.

### Data dictionary 

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|2017 - 2019 ACT and SAT|The various states of United State of America.| 
|participation_rate|float|2017 - 2019 ACT and SAT|The participation rate of the tests (SAT/ACT) of that particular state (units percent to two decimal places 98.10 means 98.1%.| 
|score|float|2017 - 2019 ACT and SAT|The total SAT score for SAT (EBRW and Math, range: 400 - 1,600) and the composite score for ACT [average of the four test scores (English, mathematics, reading, science), range: 1 - 36].| 
|year|object|2017 - 2019 ACT and SAT|Year ranging from 2017 to 2019.| 
|test|object|2017 - 2019 ACT and SAT|Which test (SAT or ACT).| 
|income|integer|Median Annual Household Income|The median annual household income for the various USA States from 2017 to 2019.| 

### Data source

The following 7 datasets will be used to complete the analysis:

> 1. [`act_2017.csv`](./data/act_2017.csv): 2017 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
> 2. [`act_2018.csv`](./data/act_2018.csv): 2018 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
> 3. [`act_2019.csv`](./data/act_2019.csv): 2019 ACT Scores by State ([source](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows))
> 4. [`sat_2017.csv`](./data/sat_2017.csv): 2017 SAT Scores by State ([source](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/))
> 5. [`sat_2018.csv`](./data/sat_2018.csv): 2018 SAT Scores by State ([source](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/))
> 6. [`sat_2019.csv`](./data/sat_2019.csv): 2019 SAT Scores by State ([source](https://blog.prepscholar.com/average-sat-scores-by-state-most-recent))
> 7. [`household income.csv`](../data/household_income.csv): Median annual household income by State from year 2017 to 2019 ([*source*](https://nces.ed.gov/programs/digest/d20/tables/dt20_102.30.asp))

### Brief summary of analysis 

- There exist a moderate positive correlation between ACT scores and annual household income.
- There exist little to no correlation between SAT scores and annual household income.

### Conclusions/Recommendations

**Conclusion:** 

- There exist a slight relationship between the annual household income and their ACT scores. As students with higher annual household income achieves a higher ACT score, there exist a biasness due to socioeconomic differences. 

- As for the SAT score, we observed minimal correlation between the annual household income and SAT score. Thus, we conclude there is little to no relationship between the annual household income and their SAT scores.

**Recommendations:**

- The ACT system should be abolished and students should take SAT as part of the college entrance examinations. This will allow students from a less wealthy family gets to go to the school of their choice if they have the academic ability (scored via SAT). 

- Financial support could also be given to students from less wealthy families who are taking the ACT to support them and help them in their ACT scores.
