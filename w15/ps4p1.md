# CS50 Problem Set 4 Part 1 - Census Taker

## Setup
-   Create a new folder name  ps4 at the same level as ps3 and then create a new folder named census.
-   In that folder create a new query file named report.sql
-   Read the problem - https://cs50.harvard.edu/sql/2024/psets/4/census/
-   Get the census database
    -   ```curl -o census.db https://raw.githubusercontent.com/CIT28/files/main/w15/census.db```
- **COMMIT MESSAGE - "setup done"**   

## Create Views
- For this problem set your will create 4 views: rural, total, by_district, most_populated
        -  In the link you will fine How to Test
        -  For each view:
            - Code the view and then associated test
            - Once you have correct output for each test
            - Commit for each view and test, ex of commit message
                - **COMMIT MESSAGE - "rural view and test done"**

## Create Census Report
- Now create the Nepal Census Report, see my example below
- You will notice in my output below I have commas, this is a good time to introduce printf
    - ```SELECT printf('%,d', your_column) AS formatted_number FROM your_table;```
- At the end of the report include .schema, I don't include this in my example below.
- Once you have the correct output created
    - **COMMIT MESSAGE - "report complete"**
## Example
- Here the output you need to create in report.txt
<pre>
----------------->> Nepal Census Report <<-------------------
Number of rural districts
=============================================================
┌───────────────────┐
│ # Rural Districts │
├───────────────────┤
│ 461               │
└───────────────────┘
Number of rural families
=============================================================
┌──────────────────┐
│ # Rural families │
├──────────────────┤
│ 2,229,834        │
└──────────────────┘
Total HouseHolds
=============================================================
┌─────────────────┐
│ Total HouseHold │
├─────────────────┤
│ 5,642,674       │
└─────────────────┘
District with second lowest number of families?
=============================================================
┌──────────┬──────────────┐
│ district │ Num Families │
├──────────┼──────────────┤
│ Manang   │ 1,545        │
│ Mustang  │ 3,751        │
└──────────┴──────────────┘
Most populated by HouseHold
=============================================================
┌───────────┬───────────────────────────┐
│ district  │ Most Populated HouseHolds │
├───────────┼───────────────────────────┤
│ Kathmandu │ 275,806                   │
└───────────┴───────────────────────────┘
Census Schema MY EXAMPLE DOES NOT INCLUDE THIS BUT YOURS SHOULD
=============================================================

</pre>

## Grading
-This is how I will grade your work:
1. Did you provide the correct commit history URL for the census (all lowercase) folder = 5 points
2. Did you do all the commits required for this work = 10 points
3. Did you have all the queries in the report.sql = 40 points
4. Did you create the report.txt and include all the required output = 25 points
5. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 