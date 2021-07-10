# School_District_Analysis

## Overview
The primary purpose of this analysis is to analyze the impact of removing data from a data set.  This analysis is performed by reviewing data points of the original data set, removing a set of data and then running the same analysis again.  During this module we performed an initial analysis on 15 schools to compare their performance and understand what may contribute to a school being a "high" performer.  Additional information came to light that indicated their may be a case of academic dishonesty in one of the schools.  As such we performed a secondary analysis removing the data that was in question (the math and reading scores of 9th graders in Thomas high school).  

  - The code was modified by replacing the Thomas High School 9th grade scores with Nan, 
  - recalculating the students: `student_count_T9 = sum((school_data_complete_df["school_name"] == "Thomas High School") & (school_data_complete_df["grade"] == "9th"))`
  - calculating a new student count `new_student_count = student_count - student_count_T9`
  - Replacing the results for Thomas High School `per_school_summary_df = per_school_summary_df.replace({per_school_summary_df.loc["Thomas High School", "% Passing Math"]: passing_math_percent_THS})`


## Results of Removing Thomas High School 9th Grade Results

### District Summary Impact:
The impact of replacing the 9th Grade scores with Nan and recalculating the number of students was not significant to the results.  Four changes occurred in the district summary as a result of this change:
 - average math scores dropped from 79.0 to 78.9
 - % passing math changed from 75.0% to 74.8%
 - % passing reading changed from 85.8% to 85.7%
 - % overall passing both reading and math changed from 65.2% to 64.9%

Original District Summary
![Original_District_Summary](/Resources/District_Summary_Original.png)

New District Summary
![District Summary](/Resources/District Summary.png)

### Impact to Thomas High School Data Points
When you replace the grades for the 9th graders and re-calculate the total students for Thomas High School the impact on the measurements is insignificant
 - average math scores dropped from 83.42 to 83.35
 - average reading scores dropped from 83.85 to 83.89
 - % passing math changed from 93.27% to 93.19%
 - % passing reading changed from 97.31% to 97.02%
 - % overall passing both reading and math changed from 90.95% to 90.639%

### School Summary Impact:
There is no impact on the rankings of the schools.  Thomas Highschool, despite the changes, remained as the 2nd ranked overall best performing school.  All other schools remained in the same ranking position

Thomas High School results after modification and ranking:
![Top 5 Schools](/Resources/Top5_Schools.png)

### Impact to Other Measurements:
In the original and post analysis the following data points were analyzed.  Changes in the below measurements were not significant between the two data sets.
  - Math and Reading scores by grade
  - Scores by school spending
  - Scores by school size
  - Scores by school types

### Noteworthy data points:
- Medium size schools were the top performers regardless of the spending ranges per students
  - There appears to be a negative correlation between the spending ranges per student and the average % of students passing for reading, math and both, with a more pronounced impact on math

## Summary
The impact of removing the 9th grader results for Thomas High school on the overall results were insignificant.  As identified above there were four main changes within the District Summary results: 1) averge math scores dropped, 2)% passing math dropped, 3)% passing reading dropped and 4)the overall % of passing both reading and math dropped




