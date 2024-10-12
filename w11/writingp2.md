# CS50 Writing Part 2
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 1 - Writing](https://www.youtube.com/watch?v=BD08USRd2M8)


### Timemark 1:02 to ?
- Continue working in the writing folder, in the README.md add a heading for 'Writing Part 2'.
- Rename the write.sql to write-1.sql and create a new file write-2.sql and delete all the code in the schema.sql file.  
- Delete the mfa.db and rec-create it with [schema](writingp1.md#MFA2)
-
    - **COMMIT MESSAGE - "setup done"**
- 
- Create another new file named write.sql and in that file write the first INSERT INTO query, comment it out and then write the second one.  No need to include the query to view the data in the table. 
- Now write the thrid INSERT INTO and in your notes explain what happens when you leave off the id and also include the concepts covered by the questions. 
    - **COMMIT MESSAGE - "INSERT INTO and notes"**
- Continue at 13:46 to code along just try to run the write.sql again to see the error and note your README.md the error and note how the table constrain work in this case. 
- Continue and write the next INSERT INTO to test the NULL constrain, then continue and code the next INSERT INTO and make sure all the data was created correctly.
- Listen to the question.
- Second a second terminal output to pow1.txt and run a query to output all the data. 
    - **COMMIT MESSAGE - "INSERT INTO w contrains & > 1 row"**

- You will need the following files:
    -```curl -o mfa.csv https://raw.githubusercontent.com/CIT28/files/main/w11/mfa.csv```
- In the README.md, add a subheading for Importing and a note about what is a CSV file. 
- DROP the tables in the mfa.db file or delete it and re-create as Carter does. You are doing this to remove the data from the database. 
- Write the .import in your write.sql, note in your README.md what each parameter (ex --csv) in the .import command does. 
- Now run the .import and the SELECT * to make sure the csv was successfully imported and output that to the pow1.txt. 
- Remove the id from the csv file and then run the .import again with the new temp parameter and in the README.md explain why this will no longer
be imported correctly. 
- HEADS UP - Be careful not to run the .import more than once as it will cause issues with the INSERT INTO.
- Now code the INSERT INTO to populate the collections table with the temp table data, delete the temp table (DROP). 
- Listen to the questions and note what happens on error for INSERT TO from temp file and fields without values.
- Then commit with message,
    - **COMMIT MESSAGE - ".import & temp tables"**

- Then start back at 37:08 and add a subheading for Deleting add the concepts cover by Carter about this topic.
- Code along in your write.sql, makes sure to comment out previous query and before you code along write the INSERT INTO 
query for the new items in the collections table. After you run the query, update your pow1.txt file, then comment out the query.
- Now code the DELETE and run it and make sure the query worked and note the id's in the table now. 
- Now code the query to DELETE based on NULL, did it work? Mine did not and I'm guessing yours did not. Anything idea why? 
Note your thoughts or what you did to figure it out in your README.md, then watch this video from me - https://youtu.be/xztU0Wpuw1c
- Update your pow file and then commit with message:
    - **COMMIT MESSAGE - "DELETE and why NULL did not work"**

- Continue at 41:22 and then before hear the answer to what conditional would we need, write your thoughts in the README.md file and then listen to the answers and update based on what Carter suggested. 
- Code the DELETE, run the query, make sure it worked and update your pow file and commit with message:
    - **COMMIT MESSAGE - "conditional DELETE"**

- Continue at 45:36, adding a subheading Foreign Key Constraints and take a few notes on content covered. 
- Before coding, delete the mfa.db, copy the [schema](#MFA1) code here into a file named schema.sql and run that to create the db and data.  
- Now code the DELETE in your write.sql, yes it will throw an error, then commet it out. 
- In your write.sql, now write the DELETE with the subquery, yes the correct one and make sure it runs successfully, commet it out and uncomment the DELETE above and run it again. 
- In the README.md, write your understanding of why we needed to do the subquery to delete.
- At 55:07, update your pow file and commit with message:
    - **COMMIT MESSAGE - "foreign key constraints & DELETE"**

- Now add ON DELETE into the README.md and add the what this SQL commands does and the associated options (params) and how they work. 
- Delete the mfa.db and copy the [schema](#MFA2) into the schema.sql file, no need to save the previous schema code and run this query to create the db and data.
- Comment out previous query and code along with in the write.sql. 
- Review the .schema to see make sure the ON DELETE CASCADE is there.
- Make sure your DELETE work on both artists and the created table??????
    - Mine did not and I'm guessing yours did not!  Like before see if you can determine why and in your README.md file add a subheading for ON DELETE did not work and tell me what you searched or what prompts you used, then commit with message:
    - **COMMIT MESSAGE - "what I tried"**
    - Now watch how I fixed it - https://youtu.be/wLv4vRcIJMQ
    ```PRAGMA foreign_keys = ON```
    - Then try the query again to make sure it worked!  
    - **COMMIT MESSAGE - "works now"**
- Listen to the question!

## Grading
-This is how I will grade your work:
1. Did you provide the correct commit history URL for the writing (all lowercase) folder = 5 points
2. Did you do all the commits required for this work = 20 points
3. Did you have all the queries in the write.sql file = 25 points
    - make sure you not include notes in your sql file. 
    - You can include, but don't need to include the SELECT * FROM queries that Carter does on the terminal
    - I counted 16 queries in my write.sql
4. Did you create the powp1.txt include all the required output = 15 points
5. Did you include all the required content in the README.md file = 35 points
6. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 

## MFA1 
```
CREATE TABLE "collections" (
    "id" INTEGER,
    "title" TEXT NOT NULL,
    "accession_number" TEXT NOT NULL UNIQUE,
    "acquired" NUMERIC,
    PRIMARY KEY("id")
);

INSERT INTO "collections" ("title", "accession_number", "acquired")
VALUES 
('Farmers working at dawn', '11.6152', '1911-08-03'),
('Imaginative landscape', '56.496', NULL),
('Profusion of flowers', '56.257', '1956-04-12'),
('Spring outing', '14.76', '1914-01-08');

CREATE TABLE "artists" (
    "id" INTEGER,
    "name" TEXT NOT NULL,
    PRIMARY KEY("id")
);

INSERT INTO "artists" ("name") 
VALUES 
('Li Yin'),
('Qian Weicheng'),
('Unidentified artist'),
('Zhou Chen');

CREATE TABLE "created" (
    "artist_id" INTEGER,
    "collection_id" INTEGER,
    PRIMARY KEY("artist_id", "collection_id"),
    FOREIGN KEY("artist_id") REFERENCES "artists"("id"),
    FOREIGN KEY("collection_id") REFERENCES "collections"("id")
);

INSERT INTO "created" ("artist_id", "collection_id")
VALUES 
((SELECT "id" FROM "artists" WHERE "name" = 'Li Yin'), (SELECT "id" FROM "collections" WHERE "title" = 'Imaginative landscape')),
((SELECT "id" FROM "artists" WHERE "name" = 'Qian Weicheng'), (SELECT "id" FROM "collections" WHERE "title" = 'Profusion of flowers')),
((SELECT "id" FROM "artists" WHERE "name" = 'Unidentified artist'), (SELECT "id" FROM "collections" WHERE "title" = 'Farmers working at dawn')),
((SELECT "id" FROM "artists" WHERE "name" = 'Zhou Chen'), (SELECT "id" FROM "collections" WHERE "title" = 'Spring outing'));
```


## MFA2
```
-- Add ON DELETE CASCADE

CREATE TABLE "collections" (
    "id" INTEGER,
    "title" TEXT NOT NULL,
    "accession_number" TEXT NOT NULL UNIQUE,
    "acquired" NUMERIC,
    PRIMARY KEY("id")
);

INSERT INTO "collections" ("title", "accession_number", "acquired")
VALUES 
('Farmers working at dawn', '11.6152', '1911-08-03'),
('Imaginative landscape', '56.496', NULL),
('Profusion of flowers', '56.257', '1956-04-12'),
('Spring outing', '14.76', '1914-01-08');

CREATE TABLE "artists" (
    "id" INTEGER,
    "name" TEXT NOT NULL,
    PRIMARY KEY("id")
);

INSERT INTO "artists" ("name") 
VALUES 
('Li Yin'),
('Qian Weicheng'),
('Unidentified artist'),
('Zhou Chen');

CREATE TABLE "created" (
    "artist_id" INTEGER,
    "collection_id" INTEGER,
    PRIMARY KEY("artist_id", "collection_id"),
    FOREIGN KEY("artist_id") REFERENCES "artists"("id") ON DELETE CASCADE,
    FOREIGN KEY("collection_id") REFERENCES "collections"("id") ON DELETE CASCADE
);

INSERT INTO "created" ("artist_id", "collection_id")
VALUES 
((SELECT "id" FROM "artists" WHERE "name" = 'Li Yin'), (SELECT "id" FROM "collections" WHERE "title" = 'Imaginative landscape')),
((SELECT "id" FROM "artists" WHERE "name" = 'Qian Weicheng'), (SELECT "id" FROM "collections" WHERE "title" = 'Profusion of flowers')),
((SELECT "id" FROM "artists" WHERE "name" = 'Unidentified artist'), (SELECT "id" FROM "collections" WHERE "title" = 'Farmers working at dawn')),
((SELECT "id" FROM "artists" WHERE "name" = 'Zhou Chen'), (SELECT "id" FROM "collections" WHERE "title" = 'Spring outing'));
```