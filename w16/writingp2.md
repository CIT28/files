## CS50 Writing Part 2

📺 **Watch Lecture**  
Right-click and select **“Open in new tab”** to view [CS50 SQL - Lecture 2 - Writing](https://www.youtube.com/watch?v=BD08USRd2M8)

---

### Markdown Legend

Use these Markdown syntaxes in your `README.md` file:

- **Headings**
  - `#` for H1
  - `##` for H2
- **Outline**
  - `*` or `-` for bullet points

---

## Setup

1. Continue working in the `writing` folder 
2. Create a new file `p2-q.sql` by copying a previous query file.
   - Remove any old queries.
   - Update to have `pow-p2.txt` output file.
3. Add an H1 heading to your `README.md`:  
   ```markdown
   # Writing Part 2
   ```
---

### Setup the new mfa.db
- Before you start working do the following
    - delete the mfa.db, create it `sqlite3 mfa.db` 
    - deleting content in the `schema.sql` copying the contents here [schema](#MFA). `.read schema.sql`
    - In your p2-q.sql file write our "normal" queries for each table in the newly created `mfa.db`. 
    - In the sqlite3 terminal also run this `PRAGMA foreign_keys = 1;`
**Commit Message:** `"new mfa.db ready"`

📍 Timestart: 55:00 

#### Exploring ON DELETE Behaviors

- Take notes in your `README.md` ## `DELETE Behaviors:
  - What ON DELETE options exist: RESTRICT, NO ACTION, SET NULL, CASCADE.
  - CASCADE deletes related rows automatically.
  - Default behavior when deleting rows without AUTOINCREMENT.
  - AUTOINCREMENT ensures unused IDs can be filled.

- Code along to:
  - Confirm that ON DELETE CASCADE is applied on the `created` table.
  - Delete the artist "Unidentified artist" and observe the automatic deletion from `created`.
  - Verify results
- Include `.print` commands in your SQL to describe what ON DELETE CASCADE did.
- Output final table data using the queries we wrote for the setup`pow-p2.txt`.

**Commit Message:** `"explored ON DELETE options and cascade behavior"`

📍 Timestart: 01:02:19

#### Update Artist Association

- Code Along to reassign "Farmers Working at Dawn" to the correct artist (Li Yin) in the `created` table
- Confirm update 
- Include a `.print` explaining that you reassigned artist correctly.
- Comment out the UPDATE query
- Output `created` table data using the queries we wrote for the setup update the `pow-p2.txt`.

💾 **Commit Message:** `"updated artist association for Farmers working at dawn"`


#### Import and Setup Votes Data
- You will need the following file in your `writing` folder:
    -  ```curl -o votes.csv https://raw.githubusercontent.com/CIT28/files/main/w16/votes.csv```
- Create a new database `votes.db`.
- Import `votes.csv` into a table called `votes`:
- Verify by data in `votes` table.
- Comment out the import query
- Output `votes` table data and update the  `pow-p2.txt`.

💾 **Commit Message:** `"imported votes.csv into votes table"`


#### Trim Whitespace and Uppercase Titles
- Code the `TRIM` and `UPPER` to clean titles:
- Verify by data in `votes` table.
- Comment out the UPDATE query
- Output `votes` table data and update the `pow-p2.txt`.
  
💾 **Commit Message:** `"trimmed and uppercased titles for consistency"`


#### Fix Typos with UPDATE and LIKE
- Correct typos manually and using `LIKE` patterns
- Use `.print` to explain why `LIKE` was used carefully.
- Comment out the UPDATE query
- Output `votes` table data and update the `pow-p2.txt`.

💾 **Commit Message:** `"fixed title typos using UPDATE and LIKE"`

#### ✅ Final Grouping and Review
- Group the cleaned data
- Confirm there are four correct groups.
- Take a final note in `README.md` about using UPDATE for data cleaning.
- Output final results to `pow-p1.txt`.

💾 **Commit Message:** `"finalized cleaned vote data"`


## BREAK OPTIONAL  
- If you got this far you can take a break and complete the rest of this work by the Thursday night deadline.  
- To "GET" this break you will submit your commit history for the writing folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 

📍 Timestart: 01:24:00
### Triggers and Soft Deletion

####  Create Transactions Table and Basic Trigger
- Take notes in your `README.md` ## `CREATE TRIGGER` include the `BEFORE`, `FOR EACH ROW`, `BEGIN` and `END` concepts
- Write SQL to create `transactions` table
- Write SQL to create trigger to log sold items
- Test by writing SQL to deleting a row from `collections` and checking `transactions`.
- Verify the trigger worked by output the tables updated and the schema to the pow2-p.txt. 

💾 **Commit Message:** `"created transactions table and sell trigger"`


#### Create Trigger for Buying
- Write SQL to create trigger to log bought items
- Add  `.print` and describe how each line functions in this SQL
- Verify using `.schema`.
- Test by writing SQL to insert into `collections` and checking `transactions`.
- Verify the trigger worked by output the tables updated and the schema to the pow2-p.txt. 


💾 **Commit Message:** `"created buy trigger for purchases"`

#### Add Soft Delete Functionality
- Take notes in your `README.md` ## `Soft Delete` 
- Write SQL to add the  `deleted` column to `collections`
- Verify column addition using `.schema`.
- Write SQL to Mark an item as deleted
- Verify the trigger worked by output the tables updated and the schema to the pow2-p.txt. 
  
💾 **Commit Message:** `"added soft delete feature with deleted column"`


#### ✅ Query Non-Deleted Items
- Write query to show only non-deleted items:
- Reflect in `README.md`:
- Benefits and concerns with soft deletion (e.g., GDPR and ethical issues).
- Importance of true deletion vs soft deletion depending on data type.

💾 **Commit Message:** `"queried non-deleted items and noted soft deletion best practices"`

## Grading Rubric

| Criteria                                                                | Points |
|-------------------------------------------------------------------------|--------|
| ✅ Correct commit history URL for `writing` folder                      | 10     |
| ✅ All required commits are included                                    | 20     |
| ✅ All queries are present in `p2-q.sql`                                | 25     |
| ✅ Correctly created `pow-p2.txt` with required output                  | 20     |
| ✅ Complete and accurate `README.md` content                            | 25     |
| ❗ Late submissions will be penalized 25 points                         |        |
|-------------------------------------------------------------------------|--------|
**Example:** If submitted late but otherwise complete, you will receive 75/100.




## MFA
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