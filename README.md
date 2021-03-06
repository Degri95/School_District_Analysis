# School_District_Analysis
Using Python with Pandas and Jupyter Notebook to analyze school data.

## Overview of the project
In this project a school board has been notified that the 9th grade testing data for Thomas High School has evidence of academic dishonesty. Since we had already completed an analysis of the data, we were tasked with replacing all of the math and reading scores of the affected students with [NaN](https://pandas.pydata.org/docs/user_guide/missing_data.html) (461 students in total). After replacing the the data we were asked to perform another analysis and compare the overall changes.

We were able change all the 9th Grade values to NaN by using a Numpy method with the following code.

![NaN Code](/Resources/nan_code.PNG)

## Results

### How is the school district summary affected?

#### Original District Summary
![Old district summary](/Resources/old_district_summary.PNG)

#### Updated District Summary
![Updated District Summary](/Resources/new_district_summary.PNG)

After updating the grades to NaN, we can see the summary was marginally affected. The greatest change was .3% difference from our original summary.
- The Average Math Score decreased .1%.
- The Average Reading Score stayed the same.
- The % Passing Math decreaesed .2%
- The % Passing Reading decreased .3%
- The % Overall Passing decreased .1%


### How is the school summary affected?

#### Original School Summary
![Old School Summary](/Resources/old_school_summary.PNG)

#### Updated School Summary
![Updated School Summary](/Resources/new_school_summary.PNG)

In the Thomas High School row we can see the changes in the data.

- The Average Math Score decreased .008%
- The Average Reading Score increased .05%
- The % Passing Math decreased .08%
- The % Passing Reading decreased .29%
- The % Overall Passing decreased .317%

We were able to update Thomas High Schools scores to the correct values by calculating the averages and percentages by using an updated student count for the school, without the 9th Grade student count skewing the metrics.

![THS student count without 9th Graders](/Resources/THS_count.PNG)

### How does replacing the ninth graders??? math and reading scores affect Thomas High School???s performance relative to the other schools?

#### Original Top 5 Schools
![Old Top 5 Schools](/Resources/old_top_5.PNG)

#### Updated Top 5 Schools
![Updated Top 5 Schools](/Resources/new_top_5.PNG)

Thomas High school was originally the second highest school when we sort the schools by "% Overall Passing". After updating our data and finding the adjusted values, we can analyze if our changes made an impact in perfomance relative to other schools.

- Thomas High Schools still holds the second highest passing percentage.
- The difference between Thomas High Schools (2nd) percentage and Griffin High School (3rd) has decreased to .3% from the original .35%
- The difference between Thomas High Schools (2nd) percentage and Cabera High Schools (1st) has increased to .7% from the original .39%

#### Original Bottom 5 Schools
![Old Bottom 5 Schools](/Resources/old_bottom_5.PNG)

#### Updated Bottom 5 Schools
![New Bottom 5 Schools](/Resources/new_bottom_5.PNG)

Looking at the Bottom 5 schools we can see no metrics were impacted. All values remain the same.

### Math and Reading Score by Grade

#### Original Math Score by Grade 
![Original Math Score by grade](/Resources/old_math_scores_by_grade.PNG)

#### Updated Math Score by Grade
![Updated Math Shore by Grade](/Resources/new_math_score_by_grade.PNG)

#### Original Reading Score by Grade
![Original Reading Score by Grade](/Resources/old_reading_scores_by_grade.PNG)

#### Updated Readin Score by Grade
![Updated Reading Score by Grade](/Resources/new_reading_score_by_grade.PNG)

The only change in these DataFrames were the 9th grade Thomas High School scores were replaced with NaN.

### Scores by Spending Size

#### Original Scores by Spending Size
![Original Scores by Spending Size](/Resources/old_spending_ranges.PNG)

#### Updated Scores by Spending Size
![Updated Scores by Spending Size](/Resources/new_spending_ranges.PNG)

Thomas High School falls in the $630-644 bin. Looking at the updated Scores by Spending size DataFrame, we can see that no values changed. This DataFrame was formatted to round decimals, so there may be a very small change we're not seeing.

### Scores by School Size

#### Original Scores by School Size
![Original Scores by School Size](/Resources/old_by_size.PNG)

#### Updated Scores by School Size
![Upated Scores by School Size](/Resources/new_by_size.PNG)

Thomas High School falls into the Medium bin. Updating the 9th Graders data in Thomas High School didn't cause any values to change in the updated DataFrame. This DataFrame was also formated to round decimals, so there may be a very small change we're not seeing.

### Scores by School Type

#### Original Schools by School Type
![Original Schools by School Type](/Resources/old_by_type.PNG)

#### Updated Schools by School Type
![Updated Schools by School Type](/Resources/new_by_type.PNG)

Thomas High School is a Charter school. So if data was changed, it would occur in the Charter row. Comparing the two DataFrames we can see that no data has changed. This DataFrame had formatting to round decimals as well. So there may be a small change we're not seeing.

## Summary 
- Any metrics that were affected by the replacement of Thomas High Schools 9th Grade scores were less than 1%
- The only metrics that were visibly altered were the School District Summary, School Summary, Top 5 Schools, and Math and Reading Scores by Grade DataFrame. (Math and Reading Scores only displayed updated value of NaN)
- Thomas High School almost dropped to third in the Top 5 Schools DataFrame. If the "% Overall Passing" column was .03% to .04% lower, Griffin Highschool would replace it as second.
- By updating Thomas High Schools scores and averages by using their student count without the 9th graders we were able to keep our data unskewed. the changes made in the data values were all marginal.
