# CS50 Viewing Part 1
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 1 - Viewing](https://www.youtube.com/watch?v=jZwGVuA8PMI)

## Attendance
### Time mark 00:00 to 21:12
- Create a new folder at the same level as writing and name it viewing, then inside that folder add the README.md, now add a heading for 'Viewing Part 1'. 
- In your README.md file add a sub heading for Relating Review and take notes on content covered. 
- Then at 4:44 add a sub heading for View and include your understanding of what a view is and list each of the ways in which we might use them.
- In the viewing folder  ```curl -o longlist.db https://raw.githubusercontent.com/CIT28/files/main/w14/longlist.db```
- Create view.sql and code along with Carter to get a good refresher on relating, sub queries and joins. 
- Then at 15:01 add a subheading for CREATE VIEW and give how this works and how it get added into the database and make sure to include what makes it "virtual". 
- Then continue to code along to CREATE the view and then write the query using the view.
- SO MUCH CLEANER!!
- Then code along with the question to learn about how to implement ORDER BY and the better practice you could use (yes take a few notes on this concept to have the VIEW order created)
     - **COMMIT MESSAGE - "refresh and CREATE VIEW**

## Part 1 - Viewing

- Add a sub heading Viewing Part 1 and then add another sub heading for View Aggregating
- Continue at 21:12 listen about aggregates and in your notes discuss the reason for individual results vs the statists.
- Then code along with the book rating query and then code the CREATE view in your view.sql file, run it and comment out and run the simpler SQL and output that and the .schmea to the pow1.txt. 
- In your notes consider this statement Carter makes: "That the underlying data from the view still does not take up any more disk space" and tell me if you understand why this is true, use heading "disk space and view"

    - **COMMIT MESSAGE - "view with aggregating"**

- Pick it back up at 33:06 and add a sub heading for CREATE TEMPORARY VIEW and give difference between this and what we just learned and at what point do you lose the VIEW. 
- Now code along and create a temporary view and once you are done, output the .schema and the query to pow1.txt. 
- Carter gives a really good overview of the difference between the 2 methods here.  So review your content in the first point and update it if needed to help you clarify the different use cases.

    - **COMMIT MESSAGE - "TEMPORARY VIEWs"**

- Pick it back pat 39:09 and add a sub heading for "CTE - Common Table Expression" and write your understanding of this concept. 
- Now code along with Carter DROP the VIEW we created on the previous step and code the CTE.  Once you have the correct output, update your pow1.txt and commit:

- **COMMIT MESSAGE - "Creating view with CTE"**

- Start back at 44:38 and add a sub heading for "Partitioning" and write your understanding of this concept. 
- Then code along and in your notes tell me why is it might be important to have naming standards?
- Once you have both the partitioned 2022 and 2021 output them to the pow1.txt. 
- Listen to the questions and code along see why you can't update the view and then output the message to the pow1.txt. Update your understanding of the concept from the start item if you feel you understanding has improved. 
    - **COMMIT MESSAGE - "Partitioning VIEW"**

## Grading
-This is how I will grade your work:
1. Did you provide the correct commit history URL for the writing (all lowercase) folder = 5 points
2. Did you do all the commits required for this work = 15 points
3. Did you have all the queries in the view.sql file = 30 points
    - make sure you not include notes in your sql file. 
    - I counted 14 queries in my write.sql
4. Did you create the powp1.txt include all the required output = 20 points
5. Did you include all the required content in the README.md file = 30 points
6. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 


