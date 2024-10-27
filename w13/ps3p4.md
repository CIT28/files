# CS50 Problem Set 3 Part 2 - Step 2 Order and Insert

## Create your plan
-   Read the problem - https://cs50.harvard.edu/sql/2024/psets/3/meteorites/
-   Specifically read 4. and 5. in the "To consider the data" section 
-   In your README.md file add a heading 'My Plan' and after you have feel you understand what is needed write how you will approach solving the ordering and inserting. If you are using outside resources, which is fine, then be specific on prompts or resources you used/find. Provide links. 
    - **COMMIT MESSAGE - "My Plan"**  

## Finish Recreating my cleaning audit report 

- Commit after each step (ex S8 meteorites table created)
- Write you queries in the import.sql
- Here was my workflow:
    - ``` rm meteorites.db```
    - ``` cat import.sql | meteorites.db```

# Audit report finished
- Here is the content that needs to be added to your report

S8 meteorites table created 
S9 order and insert complete 
output first 10 records of meteorites table 
┌─────────────────────┬────┬───────────────┬──────────┬───────────┬──────┬────────┬─────────┐
│        name         │ id │     class     │   mass   │ discovery │ year │  lat   │  long   │
├─────────────────────┼────┼───────────────┼──────────┼───────────┼──────┼────────┼─────────┤
│ Apache Junction     │ 1  │ Iron, IIIAB   │ 25000.0  │ Found     │      │ 33.45  │ -111.52 │
│ Asarco Mexicana     │ 2  │ Iron, IIIAB   │ 0.0      │ Found     │      │ 0.0    │ 0.0     │
│ Aus                 │ 3  │ L             │ 30.2     │ Found     │      │ -26.67 │ 16.25   │
│ Benares (b)         │ 4  │ Iron          │ 0.0      │ Found     │      │ 25.33  │ 83.0    │
│ Cacilandia          │ 5  │ H6            │ 0.0      │ Found     │      │ 0.0    │ 0.0     │
│ California          │ 6  │ Iron, IAB-sLL │ 0.0      │ Found     │      │ 0.0    │ 0.0     │
│ Camp Wood           │ 7  │ Iron, IIIAB   │ 148000.0 │ Found     │      │ 29.77  │ -99.88  │
│ Cochabamba          │ 8  │ CM2           │ 85.0     │ Found     │      │ 0.0    │ 0.0     │
│ Cook                │ 9  │ Unknown       │ 0.0      │ Found     │      │ 0.0    │ 0.0     │
│ Czestochowa Rakow I │ 10 │ Iron          │ 0.0      │ Found     │      │ 50.8   │ 19.12   │
└─────────────────────┴────┴───────────────┴──────────┴───────────┴──────┴────────┴─────────┘
finished

- Once you done, the delete and create pow1.txt with the entire audit report. 

## Grading
-This is how I will grade your work:
1. Did you provide the correct commit history URL for the meteorites  (all lowercase) folder = 5 points
2. Did you do all the commits required for this work = 10 points
3. Did you have all the queries in the import.sql file = 40 points
4. Did you create the powp1.txt and include all the required output = 25 points
5. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 

## Complete audio report ex

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
┌──────────────────────────────┐
│ S7 total records AF cleaning │
├──────────────────────────────┤
│ 45716                        │
└──────────────────────────────┘
cleaning finished
S8 meteorites table created
S9 order and insert complete
output first 10 records of meteorites table
┌─────────────────────┬────┬───────────────┬──────────┬───────────┬──────┬────────┬─────────┐
│        name         │ id │     class     │   mass   │ discovery │ year │  lat   │  long   │
├─────────────────────┼────┼───────────────┼──────────┼───────────┼──────┼────────┼─────────┤
│ Apache Junction     │ 1  │ Iron, IIIAB   │ 25000.0  │ Found     │      │ 33.45  │ -111.52 │
│ Asarco Mexicana     │ 2  │ Iron, IIIAB   │ 0.0      │ Found     │      │ 0.0    │ 0.0     │
│ Aus                 │ 3  │ L             │ 30.2     │ Found     │      │ -26.67 │ 16.25   │
│ Benares (b)         │ 4  │ Iron          │ 0.0      │ Found     │      │ 25.33  │ 83.0    │
│ Cacilandia          │ 5  │ H6            │ 0.0      │ Found     │      │ 0.0    │ 0.0     │
│ California          │ 6  │ Iron, IAB-sLL │ 0.0      │ Found     │      │ 0.0    │ 0.0     │
│ Camp Wood           │ 7  │ Iron, IIIAB   │ 148000.0 │ Found     │      │ 29.77  │ -99.88  │
│ Cochabamba          │ 8  │ CM2           │ 85.0     │ Found     │      │ 0.0    │ 0.0     │
│ Cook                │ 9  │ Unknown       │ 0.0      │ Found     │      │ 0.0    │ 0.0     │
│ Czestochowa Rakow I │ 10 │ Iron          │ 0.0      │ Found     │      │ 50.8   │ 19.12   │
└─────────────────────┴────┴───────────────┴──────────┴───────────┴──────┴────────┴─────────┘
FINISHED