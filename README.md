# School_District_Analysis
Using Python with Pandas and Jupyter Notebook to analyze school data.

## Overview of the project
In this project a school board has been notified that the 9th grade testing data for Thomas High School has evidence of academic dishonesty. Since we had already completed an analysis of the data, we were tasked with replacing all of the math and reading grades with [NaN](https://pandas.pydata.org/docs/user_guide/missing_data.html) (461 students in total). After replacing the the data we were asked to performing another analysis and comparing the overall changes.

## Results

- ### How is the school district summary affected?

#### Original District Summary
![Old district summary](/Resources/old_district_summary.PNG)

#### Updated District Summary
![Updated District Summary](/Resources/new_district_summary.PNG)

After updating the grades to NaN, we can see the summary was marginally affected. 
- The Average Math Score decreased 1.1%.
- The Average Reading Score stayed the same.
- The % Passing Math decreaesed .2%
- The % Passing Reading decreased .3%
- The % Overall Passing decreased .1%