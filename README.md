# School_District_Analysis

## Project Overview
In working with the the school board to perform a district analysis on math and reading scores, it was brought to our attention that part of our data may have been corrupted.  We will be using Pandas functions to remove the corrupted data revising the dataframe, and then analyze the passing success rates of individual schools as well as the district as a whole using the following steps:

1. Replace corrupted data with NaNs
2. Create a new district summary dataframe showing average math and reading scores with passing percentages
3. Create a new school summary dataframe showing average math and reading scores with passing percentages
4. Summarize top and bottom five performng schools
5. Summarize average scores by grade level
6. Create district summaries by average spent per student, school size, and school type

## Results
After factoring out the corrupted data, the follow discoveries were made:

- At the district level, the % Overall Passing dropped from 65.2% to 64.9% after removing the corrupted data.  There was a slighlty larger drop in % Passing Math (75.0% to 74.8%) then there was in % Passing Reading (85.8% to 85.7%) when comparing the district summary before an after the data was altered.
- As expected, the only change to the school summary was to Thomas High School, which had the altered data.  It's % Overall Passing dropped from 90.9% to 90.6%
- The Change to Thomas High School was not enough to effect it's overall performance relative to other schools.  It still had the second highest overall passing rate amongst all schools
- The math and reading scores by grade analysis was summarized at the individual school level.  Therefore, other than excluding the Thomas High School 9th Grade students from the review, there were no other changes to this metric
- The impact of rmoving the corrupted data was too immaterial to register an impact on the Scores By Spending, Scores By Size, and Scores by School type metrics

## Summary
After replacing the reading and math scores of the 9th grade students at Thomas High School with NaN, we saw the district wide average math scores drop from 79.0 to 78.9.  In turn, the percentage of students passing math dropped from 75.0% to 74.8%.  The percentage of students passing reading also experienced a drop from 85.8% to 85.7%.  Overall, based on the district analysis performed, the percentage of students passing both math and reading dropped from 90.9% to 90.6%.
