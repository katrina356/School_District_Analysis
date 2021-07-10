# School_District_Analysis

## Overview
The primary purpose of this analysis is to analyze the impact of academic dishonesty on a given data set.  During this module we performed an initial analysis on 15 schools to compare their performance and understand what may contribute to a school being a "high" performer.  Additional information came to light that indicated their may be a case of academic dishonesty in one of the schools.  As such we performed a secondary analysis removing the data that was in question (the math and reading scores of 9th graders in Thomas high school).  The below summarizes the impact on the results by removing this data

## Results

### The Original Data Set:
Overall medium size schools were the top performers regardless of the spending ranges per students.  There is one large school in the top 5 performers, Wilson High School.  The top performing schools all had over 90% of the students with passing grades in both math and reading while the bottom performing schools dropped drastically to on 50% with passing both reading and math.  The biggest variance in the % of passing is due to Math.  In the top performing schools the percentage of students passing math was in the 90% range while the bottom performing schools were significantly different at 66% (over 20% variance

There appears to be a negative correlation between the spending ranges per student and the average % of students passing for reading, math and both, with a more pronounced impact on math

Overall charter schools performed better than district schools.

### The Modified Data Set:
The impact of removing the 9th grader results for Thomas High school on the overall results were insignificant.  Thomas High school still remained in the top 5 performing schools and in fact remained ranked as #2 in the district based on overall passing percentages.


District Summary Impact - With the removal of the Thomas High School 9th grades from the data set the results dropped slightly from the original results.  Overall passing percentage dropped from 65.2% to 64.9%

School Summary Impact - There is no impact on the rankings of the schools.  Thomas Highschool despite the changes remained as the 2nd ranked overall best performing school.  All other schools remained in the same ranking position

How does replacing the ninth-grade scores affect the following:
Math and reading scores by grade - There is no impact except to the 9th grade codes which will not produce a calculation since they were replaced with Nan
Scores by school spending - no impact
Scores by school size no impact
Scores by school type no impact

Four changes in the updated school district:
 - average math scores dropped from 79.0 to 78.9
 - average reading scores remained the same at 81.9
 - % passing math changed from 75.0% to 74.8%
 - % passing reading changed from 85.8% to 85.7%
 - % overall passing both reading and math changed from 65.2% to 64.9%
