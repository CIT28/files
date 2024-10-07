# CS50 Problem Set 2 Part 3 - Finish Happy to Connect and start Union Square Donuts

## Finish Happy to Connect 
- In the ps2/connect folder, update your schema with any feedback you got from me regarding your submitted schema.
    - **COMMIT MESSAGE - "updates done"** 
- Resubmit your commit history for the connect folder into the Problem Set 2 - Part 2 - Connect from last Thursday. 
    - My solution video will be available after you submit this assignment

## Setup for Union Square Donuts
- Create a new folder inside of the ps2 at the same level as atl, then create another folder named donuts and then inside that folder create a file named schema.sql and README.md, then commit with message:
    - **COMMIT MESSAGE - "donuts ready"**

## Problem to Solve
- Review the Problem to Solve - https://cs50.harvard.edu/sql/2024/psets/2/donuts
- This work will be completed over 2 canvas assignment, for this item you need to complete the following:

- Step 1 - Donuts
    - Based on your understanding of the requirements create your query for donuts, you can create more than table if you feel it is needed.  
    - In your README.md file create a sub heading for donuts and using the requirements, identify what in the requirements you used to create this part of the schema. 
    - This does not need to be long and will be modified as we move into the other area.
    - For example: column name > what text in the requirements does this meet
        - **COMMIT MESSAGE - "first draft of donuts"**
- Step 2 - Orders
    - Based on your understanding of the requirements create your query for orders, you can create more than table if you feel it is needed.  
    - In your README.md file create a sub heading for orders and using the requirements, identify what in the requirements you used to create this part of the schema.  - This does not need to be long and will be modified as we move into the other areas. If you feel it is important to add additional tables make note on your README.md file.
    - For example: column name > what text in the requirements does this meet
        - **COMMIT MESSAGE - "first draft of orders"**

- Step 3 - Customers
    - Based on your understanding of the requirements create your query for customers, you can create more than table if you feel it is neded.  
    - In your README.md file create a sub heading for customers and using the requirements, identify what in the requirements you used to create this part of the schema.  
    - This does not need to be long and will be modified as we move into the other areas. If you feel it is important to add additional tables make note on your README.md file. 
    - For example: column name > what text in the requirements does this meet
        - **COMMIT MESSAGE - "first draft of customers"**

- Step 4 - Sample Data
   - Review the sample data and make sure your schema is designed to implement the sample data. 
    - In your README.md file create a sub heading for sample sata and using the requirements, identify what in the requirements you used to create this part of the schema.  
    - This does not need to be long and will be modified as we move into the other areas. If you feel it is important to add additional tables make note on your README.md file. 
      - For example: column name > what text in the requirements does this meet 
        - **COMMIT MESSAGE - "first draft of sample data"**

- Step 5 - Check your schema.sql
    - Review the Sample Data and make any adjustment you feel are needed. 
    - Create a new database file ```sqlite3 donuts.db``` and then run ```.read schema.sql``` and fix any errors you encounter.  Then on different terminal session run ```sqlite3 donuts.db``` and then ```.output pow3.txt``` and ```.schema```. Commit with message:
        - **COMMIT MESSAGE - "first run of schema"**

- Step 7 - Create a ERD image
    - Once you have your database schema finished, then from the output of .schema copy the schema into chatGPT
    - Have it create the DBML markup and the copy that into https://dbdiagram.io/
    - Arrange the tables so they are easy to view the relationships
    - Take a printscreen, name the file erd.png (or whatever file extension you want)
    - Upload (like I showed in the attendance you can just drag the file into the ps2/connect folder)
    - In your README.md, place this at the bottom of your file ![image info](erd.png) Yes this does show as a broken link when you are viewing the markdown file here, make sure you does show up. 
    - Update the filename as needed and commit with message:
        - **COMMIT MESSAGE - "ERD image file created"**     

## Grading
-This is how I will grade your work:
1. Did you provide the correct commit history URL for the connect folder 
    - 5 points
2. Did you do all the commits required for this work 
    - 20 points
3. Did you have all the queries in the schema.sql file
    - make sure you don't include notes in your sql file
    - does the schema you created meet the requirements
    - 25 points
4. Did you create the powp3.txt include all the required output
    - 15 points
5. Did you include all the required content in the README.md file
    - 25 points
6. Correctly created and upload the ERD image file into your README.md file
    - 10 points
- No solution video for this work, but I will record one for the Thursday night submission. Once you submit I will give you feedback and you can update your schema before Thursday and get any points you missed on that submission. 
- Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 