# CS50 Problem Set 3 Part 3 - Step 1 Clean the Data

## Setup
-   In the ps3 folder and at the same level as dont-panic create a new folder named meteorities.
-   In that folder create a new query file named import.sql and README.md
-   Read the problem - https://cs50.harvard.edu/sql/2024/psets/3/meteorites/
-   ```curl -o meteorites.csv https://raw.githubusercontent.com/CIT28/files/main/w13/meteorites.csv```
        - **COMMIT MESSAGE - "setup done"**    


## Recreate my cleaning audit report 
- Commit after each step (ex S1 total records imported)
- Write your queries in the import.sql
    - For queries that needed to ouptut a message I used .print 'message' in the import.sql file, 
    but for most just use the alias. 
- Here was my workflow, from the meteorites folder you can run:
    - ``` rm meteorites.db```
    - ``` cat import.sql | meteorites.db```

# Audit report
<pre>
temp table created 
┌───────────────────────────┐
│ S1 total records imported │
├───────────────────────────┤
│ 45716                     │
└───────────────────────────┘
┌──────────────────────────────────────┐
│ S2 total records for mass 2B updated │
├──────────────────────────────────────┤
│ 19                                   │
└──────────────────────────────────────┘
┌─────────────────┐
│ AF mass updated │
├─────────────────┤
│ 0               │
└─────────────────┘
┌─────────────────────────────────────┐
│ S3 total records for lat 2B updated │
├─────────────────────────────────────┤
│ 6438                                │
└─────────────────────────────────────┘
┌────────────────┐
│ AF lat updated │
├────────────────┤
│ 0              │
└────────────────┘
┌──────────────────────────────────────┐
│ S4 total records for long 2B updated │
├──────────────────────────────────────┤
│ 6214                                 │
└──────────────────────────────────────┘
┌────────────────┐
│ AF log updated │
├────────────────┤
│ 0              │
└────────────────┘
┌──────────────────────────────────────┐
│ S5 total records for year 2B updated │
├──────────────────────────────────────┤
│ 291                                  │
└──────────────────────────────────────┘
┌─────────────────┐
│ AF year updated │
├─────────────────┤
│ 0               │
└─────────────────┘
┌────────────────────────────────────────────────┐
│ S6 total records for > 2 decimal mass lat long │
├────────────────────────────────────────────────┤
│ 34231                                          │
└────────────────────────────────────────────────┘
┌──────────────────────────────┐
│ AF > 2 decimal mass lat long │
├──────────────────────────────┤
│ 0                            │
└──────────────────────────────┘

┌─────────────────────────────┐
│ S7 total records for delete │
├─────────────────────────────┤
│ 75                          │
└─────────────────────────────┘
┌───────────┐
│ AF delete │
├───────────┤
│ 0         │
└───────────┘
┌──────────────────────────────┐
│ S8 total records AF cleaning │
├──────────────────────────────┤
│ 45716                        │
└──────────────────────────────┘
cleaning finished
</pre>

- Once you have this done, the output it to pow1.txt

## Grading
-This is how I will grade your work:
1. Did you provide the correct commit history URL for the meteorites  (all lowercase) folder = 5 points
2. Did you do all the commits required for this work = 20 points
3. Did you have all the queries in the import.sql file = 40 points
4. Did you create the powp1.txt and include all the required output = 15 points
5. 6. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 

