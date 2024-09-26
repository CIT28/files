## CS50 Problem Set 2 - ATL

## Setup
- Create a folder ps2 at the same level as ps1 and ps0, then inside ps2 folder create another folder named atl and then inside that folder create a file named schema.sql and README.md, then commit with message:
    - **COMMIT MESSAGE - "ATL"**

## Problem to Solve
- Review the Problem to Solve - https://cs50.harvard.edu/sql/2024/psets/2/atl/

- My schema for this work created 6 tables. 

- Step 1 - Passengers
    - Based on your understanding of the requirements create your query for passenger.  
    - In your README.md file create a sub heading for passenger and using the requirements, identify what in the requirements you used to create this part of the schema.  This does not need to be long and will be modified as we move into the other areas. 
    - For example: column name > what text in the requirements does this meet
        - **COMMIT MESSAGE - "first draft of passenager"**
- Step 2 - Check-Ins
    - Based on your understanding of the requirements create your query for Check-Ins.  
    - In your README.md file create a sub heading for Check-Ins and using the requirements, identify what in the requirements you used to create this part of the schema.  This does not need to be long and will be modified as we move into the other areas. If you feel it is important to add additional tables make note on your REAMD.md file.
    - For example: column name > what text in the requirements does this meet
        - **COMMIT MESSAGE - "first draft of checkins"**
- Step 3 - Airlines
    - Based on your understanding of the requirements create your query for Airlines.  
    - In your README.md file create a sub heading for Airlines and using the requirements, identify what in the requirements you used to create this part of the schema.  This does not need to be long and will be modified as we move into the other areas. If you feel it is important to add additional tables make note on your REAMD.md file. 
    - For example: column name > what text in the requirements does this meet
        - **COMMIT MESSAGE - "first draft of airlines"**
- Step 4 - Flights
    - Based on your understanding of the requirements create your query for Flights.  
    - In your README.md file create a sub heading for Flights and using the requirements, identify what in the requirements you used to create this part of the schema.  This does not need to be long and will be modified as we move into the other areas. If you feel it is important to add additional tables make note on your REAMD.md file.
    - For example: column name > what text in the requirements does this meet
        - **COMMIT MESSAGE - "first draft of atl schema"**
- Step 5 - Check your schema.sql
    - Create a new database file ```sqlite3 atl.db``` and then run ```.read schema.sql``` and fix any errors you encounter.  Then on different terminal session run ```sqlite3 atl.db``` and then ```.output pow2.txt``` and ```.schema```. Commit with message:
        - **COMMIT MESSAGE - "first run of schema"**
- Step 6 - Sample Data
    - Review the Sample Data and update any schema area you feel is needed and update the README.md with your reasoning, once you feel your code meets the needs. 
    - Repeat Step 5
        - **COMMIT MESSAGE - "sample data updates"**

## Grading
-This is how I will grade your work:
1. Did you provide the correct commit history URL for the atl folder = 5 points
2. Did you do all the commits required for this work = 20 points
3. Did you have all the queries in the schema.sql file = 25 points
    - make sure you don't include notes in your sql file. 
4. Did you create the powp1.txt include all the required output = 10 points
5. Did you include all the required content in the README.md file = 15 points
6. After submitting your work, watch the solution video and then make any changes needed and update your README.md with a new sub heading My Grade and then based on the work you completed and how it compared to mine give you self a grade. If you feel you solution was better or how your approach was different you can discuss that in this part of your work. 
FYI the more justifiy your grade the more likely I would agree. = 15 points
    - **COMMIT MESSAGE - "my grade"**
- Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 