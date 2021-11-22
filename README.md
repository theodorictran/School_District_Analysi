# School_District_Analysis

## Overview

Initially, the purpose of this project was to create an overview of high school and district student performance and discover insights and trends based on the data given. I was given access to student's standarized test math and reading test scores as well as other information including high school attended, school budget, and grade level to name a few. Once the first run of analysis was completed, it was brought to my attention that grades for 9th graders attending Thomas High School were tampered with. As a result, I replaced the 9th graders grades with NaNs and re-conducted my analysis to create overview of student, district, and school performance.

# Results
## How is the district summary affected?
- First District Summary:<img width="925" alt="first_district_analyis" src="https://user-images.githubusercontent.com/91519293/142798900-3c41191f-bf3d-428a-99ee-1a57133b0c1c.png">

- Second District Summary:<img width="921" alt="second_district_analysis" src="https://user-images.githubusercontent.com/91519293/142798909-c7f6f7d2-a550-4222-801c-62d44c042bd8.png">

- In the images above, the top image shows the initial district analysis from my original "PyCitySchools.ipynb" file and the bottom images shows the second-run district analysis from my "PyCitySchools_Challenge.ipynb" file. The district summary was not significantly affected by replacing the 9th graders grades at Thomas High School. There were tenths of a decimal changes between "Average Math Score", "% Passing Math", "% Passing Reading", and "% Overall Passing", but nothing extreme to report.

## How is the school summary affected?
- First School Summary: <img width="987" alt="thomas_school_summary_before" src="https://user-images.githubusercontent.com/91519293/142798961-f9fa2c6d-c817-4ea0-9b45-2567c0daf455.png">

- Second School Summary:<img width="987" alt="thomas_school_summary_after" src="https://user-images.githubusercontent.com/91519293/142798976-59952b09-d841-45d4-a4b9-afd6dfab4e3c.png">

- As we saw that there were miniscule changes in the district summary, the school summary was affected the same manner. Because I only replaced 9th graders scores at Thomas High School and kept the original grades for the remaining the students at the remaining grade levels, it makes sense to only focus on the Thomas High School while looking at the two school summaries, as Thomas High School was the only school affected. Overall, average grade scores for both math and reading, and percentages across the board remained the same, but were only affected slightly having changes a couple of tenths of a decimal.

## How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
- Initial Top Performing Schools:<img width="988" alt="top_five_before" src="https://user-images.githubusercontent.com/91519293/142799017-c5b5b1ff-0298-493d-982a-ba957cf69f38.png">

- After Top Performing Schools: <img width="989" alt="top_five_after" src="https://user-images.githubusercontent.com/91519293/142799035-7fcf45d6-0511-46ad-95b2-1e4fc0631421.png">

- Replacing the ninth graders' math and reading scores did not affect Thomas High School's performance in comparison to the other schools. Prior to replacing the ninth graders' scores, Thomas High School was the second best performing school. After replacing the ninth graders' scores, Thomas High School's standing did not change, as they are still ranked the second best performing school.

## How does replacing the ninth-grade scores affect the following:
 - Math and reading scores by grade
    - By replacing the ninth-grade scores with NaNs, when looking at student scores at different grade levels, we see NaNs for the 9th grade column. All other columns remain intact.
    - Thomas High School Math Scores by Grade after grade replacements:
    - <img width="295" alt="math_nans" src="https://user-images.githubusercontent.com/91519293/142799142-cd4f4b2b-5d20-4dce-acb4-72e2461a54d2.png">
    - Thomas High School Reading Scores by Grade afer grade replacements:
    - <img width="290" alt="reading_nans" src="https://user-images.githubusercontent.com/91519293/142799154-6e48f88a-4dc9-411c-b643-0507f17720e7.png">

 - Scores by school spending
    - Scores by School Spending before grade replacements:
    - <img width="809" alt="spending_before" src="https://user-images.githubusercontent.com/91519293/142799243-2983770e-37a2-41a3-9ad2-829337a99fcd.png">

    - Scores by School Spending after grade replacements:
    - <img width="818" alt="spending_after" src="https://user-images.githubusercontent.com/91519293/142799254-7b06c056-8cf9-45ec-998a-ffbcb32a07e7.png">

    - It must first be mentioned that Thomas High School falls under the spending range of $630-644 per student. Looking at the $630-644 row between the before and after images, there was not a significant difference between all columns. All columns decreased by less than 0.5% or 0.5 grade score, respectively.
 - Scores by school size
    - Scores by School Size before grade replacements: 
    - <img width="746" alt="size_before" src="https://user-images.githubusercontent.com/91519293/142799348-de4ac024-5e70-4713-8c16-d6073d8252fd.png">

    - Scores by School Size after grade replacements:
    - <img width="752" alt="size_after" src="https://user-images.githubusercontent.com/91519293/142799355-7e16d27d-c975-4e8b-8c7d-c46ffdbb1e6d.png">

    - Looking at the school size charts before and after grade replacements, there were no differences observed. Possibly, there was a miniscule difference if columns formatted to allow more decimal places.
 
 - Scores by school type
    - Scores by School Type before grade replacements:
    - <img width="706" alt="school_type_before" src="https://user-images.githubusercontent.com/91519293/142799417-568924fa-1cbc-4e9c-bd8b-386100604f57.png">

    - Scores by School Type after grade replacements:
    - <img width="701" alt="school_type_after" src="https://user-images.githubusercontent.com/91519293/142799425-eb612bae-50ac-4dc8-91d6-3997816120dc.png">

    - Similar to looking at the differences in scores by school size, replacing the scores of ninth grade students at Thomas High School did not yield any significant difference. It is worth mentioning that there might be a insignificant difference that can be seen if columns were formatted to allow more decimal places.


# Summary
After replacing the math and reading scores of ninth grade students at Thomas High School with NaNs, there was no significant differences exhibited between math and reading scores by grade level, scores by school spending, scores by school size, and scores by school type dataframes. To clarify, there was differences of less than 0.5% and 0.5 grade scores, but these differences did not yield any new information. Before the grade replacements, Thomas High School was the second best performing school. After the grade replacements, Thomas High School was still the second best performing school.
