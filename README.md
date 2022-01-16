# School_District_Analysis_Challenge

## Challenge Overview
A district school board has requested we repeat our school district analysis project from earlier, but with modifications due to evidence of academic dishonesty focussing on Thomas High School ninth graders.

1. Replace the math and reading scores for Thomas High School(THS) ninth graders.
2. Calculate new passing percentages with the new data.
3. Calculate the new district and school summary.
4. Calculate the top 5 and bottom 5 schools based on overall passing rate.
5. Determine average math and reading for each grade level at each school.
6. Determine scores by school spending per student, by school size and type.

## Resources
- Data Sources: schools_complete.csv, students_complete.csv
- Software: Python 3.8.8, Jupyter Notebook 6.3.0, Pandas 1.3.3

## Results

### How is the district summary affected?
Original Analysis:
<img width="910" alt="Screen Shot 2022-01-16 at 6 49 08 AM" src="https://user-images.githubusercontent.com/91889241/149660647-e382587c-cf96-4fe3-9ab1-b4acec6b92b3.png">

The original analysis included the 9th graders from THS scores on reading and math.  We replaced their values with NaN, that allowed us to keep the student information, such as student count, but effectively gave them a 0 grade.

New Analysis:
<img width="925" alt="Screen Shot 2022-01-16 at 6 49 59 AM" src="https://user-images.githubusercontent.com/91889241/149660773-6ff0d25c-eebf-44d1-9231-c1dd6fc88ee6.png">

The new analysis shows the effects of dropping 461 THS 9th graders student scores out of 39,170 total students.  The 1.1% difference in the new total student count from the old, doesn't statistically alter the results from prior, with a less than 0.3% change.

### How is the school summary affected?
Original Analysis:

<img width="828" alt="Screen Shot 2022-01-16 at 7 09 43 AM" src="https://user-images.githubusercontent.com/91889241/149661301-f20bad7a-ae2a-46f2-8370-981c6e14a2d3.png">

The original analysis shows an passing scores of 93.3%, 97.3% and 90.9% for math, reading, and both, respectively.

New Analysis:

<img width="825" alt="Screen Shot 2022-01-16 at 7 09 49 AM" src="https://user-images.githubusercontent.com/91889241/149661311-792a5fe0-ac7b-4f7a-be68-2a6009f2d0b0.png">

The new analysis shows after adjusting for the suspected manipulation of the THS 9th graders, the math, reading and both drop to 66.9%, 69.7% and 65.1%, respectively.  A drop of over 25 points for each category and an indication of an outlier for the 9th grade.

### How does replacing the ninth graders' math and reading scores affect THS's performance relative to the other schools?

Original Analysis:

<img width="825" alt="Screen Shot 2022-01-16 at 7 23 13 AM" src="https://user-images.githubusercontent.com/91889241/149661772-08d96d8c-3f4d-40c0-96df-dc70cff04027.png">

In the original analysis, THS scores were showing THS as the second best performing school.

New Analysis:

<img width="824" alt="Screen Shot 2022-01-16 at 7 23 20 AM" src="https://user-images.githubusercontent.com/91889241/149661774-c81ce58b-77cc-4b06-a17d-597221f81fd4.png">

In the new analysis, THS is in the middle of all schools in overall passing percentage.

### How does replacing the 9th grade scores affect the following:

#### Math and reading scores by grade
Math and reading scores by grade are unaffected for every school other than THS, as the scores and percentage of passing are done on a school by school basis.  THS in the 9th grade shows NaN to represent a non-score.

Original Analysis for math:

<img width="424" alt="Screen Shot 2022-01-16 at 7 37 25 AM" src="https://user-images.githubusercontent.com/91889241/149662392-dca368c9-a578-4149-8c4f-7bc12cd92d39.png">

New Analysis for math:

<img width="295" alt="Screen Shot 2022-01-16 at 7 38 31 AM" src="https://user-images.githubusercontent.com/91889241/149662422-a7873aed-09ec-497c-bf8c-9cf6a8427e07.png">

#### Scores by school spending
Scores by school spending have little effect on the outcome; the total amount of students was not changed for the analysis, only the grade values for THS 9th graders.  THS is the $630 - $644 range.

Original Analysis:

<img width="825" alt="Screen Shot 2022-01-16 at 7 48 19 AM" src="https://user-images.githubusercontent.com/91889241/149662785-d9cb3f0d-bec5-49cb-b2fa-3e681fa784bf.png">

New Analysis:

<img width="831" alt="Screen Shot 2022-01-16 at 7 48 48 AM" src="https://user-images.githubusercontent.com/91889241/149662792-c5b2623a-6f0e-48c1-b269-93f08fd9efa0.png">

#### Scores by school size
THS is defined as a medium sized school with 1000-2000 students.  Due to THS dropped 9th grade scores, this only represents 1.1% of the total population of students and shows only a nominal drop in passing percentage overall catetgories; math, reading and overall.

Original Analysis:

<img width="824" alt="Screen Shot 2022-01-16 at 7 50 26 AM" src="https://user-images.githubusercontent.com/91889241/149662924-0187381d-087c-4240-a2ab-55114d520398.png">

New Analysis:

<img width="827" alt="Screen Shot 2022-01-16 at 7 50 32 AM" src="https://user-images.githubusercontent.com/91889241/149662932-efceb7d4-6b2b-49c6-986e-c5d34689ca57.png">

#### Scores by school type
THS is classified as a Charter school.  THS, as a whole, makes up 13% of the charter schools student population.  THS 9th grade class is 3.8% of the total.  Due to such a small factor, we see very little drop in the key metrics once the 9th grade class is removed for THS.

Original Analysis:

<img width="827" alt="Screen Shot 2022-01-16 at 7 50 32 AM" src="https://user-images.githubusercontent.com/91889241/149663155-efa1b313-3ac0-4e52-a6ab-a9e109b30e7b.png">


New Analysis:

<img width="829" alt="Screen Shot 2022-01-16 at 8 01 14 AM" src="https://user-images.githubusercontent.com/91889241/149663217-852f0f0c-bf90-4638-ad76-7ae6927c3553.png">

## Summary

The analysis of the election. show that:
- There were 369,711 votes cast in the election.
- The candidates were:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
  
- The candidate results were as follows:
  - Charles Casper Stockham received 23.0% of the vote and 85,213 number of votes.
  - Diana DeGette received 73.8% of the vote and 272,892 number of votes.
  - Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes.
  
- The winner of the election was:
  - Diana DeGette, who received 73.8% of the vote and 272,892 number of votes.

- Election audit summary:
  - The creation of this program file, can be used in other elections.  While currently, this is serving to perform this task given three variables; ballots,         candidates, and counties.  We can expand on this to other degrees.
  - If we would like to change from known counties to known voting districts, we can take the original code:
