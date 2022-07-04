# School_District_Analysis
Using Python with Pandas and Jupyter Notebook to analyze school data.

## Overview of the project
In this project a school board has been notified that the 9th grade testing data for Thomas High School has evidence of academic dishonesty. Since we had already completed an analysis of the data, we were tasked with replacing all of the math and reading grades with [NaN](https://pandas.pydata.org/docs/user_guide/missing_data.html) (461 students in total). After replacing the the data we were asked to performing another analysis and comparing the overall changes.

## Results

### How is the school district summary affected?

#### Original District Summary
![Old district summary](/Resources/old_district_summary.PNG)

#### Updated District Summary
![Updated District Summary](/Resources/new_district_summary.PNG)

After updating the grades to NaN, we can see the summary was marginally effected. The greatest change was .3% difference from our original summary.
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

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

#### Original Top 5 Schools
![Old Top 5 Schools](/Resources/old_top_5.PNG)

#### Updated Top 5 Schools
![Updated Top 5 Schools](/Resources/new_top_5.PNG)

Thomas High school was originally the second highest school when we sort the schools by "% Overall Passing". After updating the ninth grade math and reading scores to NaN, and getting Thomas High Schools grades by dividing by the updated student count we are able to compare the changes.