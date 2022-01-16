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
