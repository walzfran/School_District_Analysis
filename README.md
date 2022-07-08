# School_District_Analysis
Module 4 School District Analysis

## Overview of the school district analysis

### This challenge was to assist Maria in understanding all of the collected data from diferent school districts on thier standardized test results. We are specifically looking at the math and reading results and making sure that the data has been cleaned and will not skew the results. This information will help the board understand where funding needs to go. In the first part of the challenge we needed to make sure that the data was clean and was free of any discrepencies and data to alter the results. We found that there was an issue with Thomas High School having non-student results included. When it was realized that Thomas High School had skewed data, we removed the input data for the 9th grade section of results as this was the area where there were discrepancies. After this data was removed from the data set we were able to adjust our code to reflect the new student count which was then used to run analysis on the school districts. 

## Results

### How is the district summary affected?
#### When looking at the district summary, there does not seem to be an overwhelming change in the cleaned data set. 
* Total Schools : 15 
  - This number remains the same
* Total Students : 39,170
  - This number remains the same 
* Total Budget : $24,649,428.00
  - This number remains the same
* Average Math Score
  - In the first analysis we got an average math score of 79.0
  - In the second analysis with cleaned data we got an average math score of 78.9 
    * This is a negative difference of .1
* Average Reading Score : 81.9
  - This number remains the same
* Percentage Passing Math 
  - In the first analysis we got 75% passing math
  - In the second analysis we got 74.8% passing math 
    * This is a difference of .2%
* Percentage Passing Reading
  - In the first analysis we got 86% passing reading
  - In the second analysis we got 85.7% passing reading
    * This is a difference of .3%
* Percentage Overall Passing
  - In the first analysis we got 65% overall passing
  - In the second analysis we got 64.9% overall passing
    * This is a difference of .1%

#### The biggest difference that I notice is how we formatted, in the first analysis we formatted the percentages to .0 which would round to the nearest whole percentage with no following numbers. If you were to format the second analysis the same way we would receive the same percentages. This means that the only real difference in the data sets is the small change of .1 in the average math score, as the reading score remained the same with both. 
#### The image below is the District Summary from the first analysis 

![District_Summary_PySchool](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/District_Summary_PyCitySchools.png)

#### This image is the District Summary from the second analysis 

![District_Summary_Challenge](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/District_Summary_Challenge.png)


### How is the school summary affected?

#### Looking at the school summary, we really only need to look at the numbers for Thomas High School as that was the only data set we altered. I will now go over the data and show what has changed or stayed the same for Thomas High School. 
* School Type : Charter
  - This remains the same
* Total Students : 1,635
  - This number remains the same 
* Total Budget : $1,043,130.00
  - This number remains the same
* Per Student Budget : $638.00
  - This number remains the same
* Average Math Score
  - In the first analysis we got an average math score of 83.418
  - In the second analysis with cleaned data we got an average math score of 83.350
    * This is a negative difference of .68
* Average Reading Score
  - In the first analysis we got an average reading score of 83.848
  - In the second analysis with cleaned data we got an average reading score of 83.896
    * This is a positive difference of .48
#### As we saw when looking at the district summary, there really is not much of a change in the data other than the small changes in average reading and math scores, with the change not even relfecting a whole percentage there was not much that cleaning the data did other than give us an accurate read versus a skewed one with false inforamtion in it. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
#### The average math and reading scores were not too impacted by the change in removing the 9th graders scores. Below are two images, the first depicts the top performing schools with all of the data and the second depicts the same set with the 9th graders scores removed. 

![Top_Performing_PyCity](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/Top_Performing_PYCity.png)

![Top_Performing_Challenge](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/Top_Performing_Challenge.png)

#### As you can see Thomas High School is still ranked second amongst the schools we analyzed in the district. The change was that the average math score went down by .068% and the average reading score went up by .048%. These are again small changes but it is good to know that our data is truly clean from false information. 


### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade
##### The math and reading scores by grade were not affected in any other way than havong the 9th grade score averages set to NaN, this is because we cleaned the data and set all of these scores to be NaN as there were false scores reported by Thomas High School. The remaining grades in the data set stayed the same as they were not altered. 
##### Below are the images for the math scores - the first is the unaltered data and the second is the data with the 9th grade scores set to NaN

![Math_Scores_PY](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/Math_Scores_PY.png)

![Math_Scores_Challenge](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/Math_Scores_Challenge.png)

##### Below are the images for the reading scores - the first is the unaltered data and the second is the data with the 9th grade scores set to NaN

![Reading_scores_Py](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/Reading_Scores_PY.png)

![Reading_scores_challenge](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/Reading_Scores_Challenge.png)

#### Scores by school spending
##### This data set was not altered by removing the 9th grade scores for math and reading as the amount this data changed was so minor that it would not be reflected in the percentages or averages for school spending. 

#### Scores by school size
##### Because we did not remove the students from the 9th grade and only the scores, the school size remained the same which did not pull Thomas High School out of the original school size it was in. Below are the images from both data sets, the first being the data that has the skewed 9th grader results and the second is cleaned. They are identical images as there was not much of a change that would be noticed with the formatting we did. 

![School_Size_PY](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/School_Size_ScoolPY.png)

![School_Size_Challenge](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/School_Size_Challenge.png)


#### Scores by school type
##### Below are the two iages of the school types, the first depicting the results that included Thomas High School 9th graders and the second reflects the data without the 9th graders from Thomas High School. 

![School_Type_PYCity](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/School_Type_PYCity.png)

![School_Type_Challenge](https://github.com/walzfran/School_District_Analysis/blob/main/Resources/School_Type_Challenge.png)

#### As you can see they are identical images which meas there was not a significat change with altering the 9th grade scores out of Thomas High School

## Summary
### Above we went over all of the sections of data we analyzed for both the data reflecting the 9th grade scores and the data that had the 9th grade scores for Thomas High School set to NaN. There were a few minor changes in the data, mainly in the math and reading score averages. Because the changes in the averages were so low the percentages were not altered very much and with formatting it was difficult to see any changes in this data. When we altered the sata to reflect NaN in the 9th grade results of Thomas High School it did not alter the total student count which made it easy to compare against the other schools in the district. I would say that the biggest thing I learned from the challenge was that it is important to have correct data even if it does not alter the final outcome in huge ways. 
