# School District Analysis
## Overview of School District Analysis
I've been given two datasets: schools in the district and students who study at these schools. 
The dataset of schools consists of name, school type, budget, number of students.
The table of student includes student ID, name, gender, grade, school, reading and math score.
The goal is to make an overview of key metrics for each school, find average math and reading scores for each grade and analyze school performance based on budget, type and school size.
I've used jupyter notebook and library pandas to conduct the analysis.

## Results
After inspecting the data, I found that, while school data is clean, the student data has undesired prefixes and suffixes in the names. I've removed all suffixes and prefixes and merged two datasets to analyze them.
During the analysis I've got the information that reading and math grades for Thomas High School (THS) ninth graders appear to have been altered. So, I have to eliminate data for the 9th grade of THS. Thus, at first, I've completed the school district analysis with all available data. Then I replaced all scores for the 9th grade of THS with NaN values and performed the analysis one more time, so now it's clear how the academic dishonesty influenced the results:

- In the district summary average math score has reduced by 0.1 points. Other values have not been changed.

![District summary](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/District%20summary.png)

![District summary, excluding the 9th grade of THS](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/District%20summary%20(excl_9th%20THS).png)

- School summary has minor changes at the THS performance: average math and reading score reduced by 0.06 and 0.05 points.

![School summary](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/School_summary.png)

![School summary, excluding the 9th grade of THS](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/School_summary_(excl_9th_THS).png)

- The Thomas High School performance compare to other schools left the same. The school still is in second place of top 5 district schools.

![Top 5 schools](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/Top_5_schools.png)

![Top 5 schools, excluding the 9th grade of THS](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/Top_5_schools_(excl_9th_THS).png)

- As I excluded data for the 9th grade of THS, nan values have appeared in the table. Other values have not been changed.

![Top 5 schools](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/Math_scores_by_grade_(excl_9th_THS).png)

- Scores by school spending have not been changed.

![Scores by school spending](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/Scores_by_school_spending.png)

![Scores by school spending, excluding the 9th grade of THS](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/Scores_by_school_spending_(excl_9th_THS).png)

- Scores by school size have not been changed too.
![](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/Scores_by_school_size.png)
![](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/Scores_by_school_size_(excl_9th_THS).png)

- Scores by school type have not been changed as well.

![](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/Scores_by_school_type.png)
![](https://github.com/angkohtenko/School_District_Analysis/blob/main/Resources/Scores_by_school_type_(excl_9th_THS).png)

## Summary
After replacing reading and math scores for the 9th grade at Thomas High School with NaNs and updating the school district analysis, I discovered few minor changes:

- Average math and reading score at the THS performance reduced by 0.06 and 0.05 points.
- That leads to reducing average math score in district summary by 0.1 points. Average reading score remained unchanged.
- Percent of passing math and reading at the THS was decreased by 0.09 and 0.29 points
- Percent of overall passing at the THS dropped by 0.31 points.

As the grade averages were rounded to one decimal place and percentages were formatted to the nearest whole number percent, the only difference that can be seen in the final tables is reducing average math score in district summary by 0.1 points.
