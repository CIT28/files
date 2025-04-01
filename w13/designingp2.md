## CS50 Designing Part 2

📺 **Watch Lecture**  
Right-click and select **“Open in new tab”** to view [CS50 SQL - Lecture 1 - Designing](https://www.youtube.com/watch?v=QzRW6bfv3Fo)

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

1. Continue working in the `designing` folder.
2. Create a new file `p2-q.sql` by copying a previous query file.
   - Remove any old queries.
   - Update to have `pow-p2.txt` output file.
3. Add an H1 heading to your `README.md`:  
   ```markdown
   # Designing Part 2
   ```

---

## Lecture Notes (Start at 53:35)

### Column Constraints

📍 **Timestart:** 53:35  
1. Add a new H2 heading in `README.md`:
   ```markdown
   ## Column Constraints
   ```
2. Take notes on each constraint using bullet point format.
3. Before coding:
   - Run the `DROP TABLE` statements (copy them from `p2-d.sql` or run them manually).
   - Copy the final queries from `p1-d.sql` into your `p2-q.sql` to restore the initial schema.

### Primary Key & Foreign Key

4. Add a new H2 heading:
   ```markdown
   ## Constraints: Primary Key and Foreign Key
   ```
5. Take notes on this topic, including the example queries.
6. Make sure to listen carefully to the student questions in the video.
7. At **1:00:19**:
   - Run your SQL.
   - Fix any errors.
   - Output the schema and a note to `pow-p2.txt`:
     ```
     .schema
     .print 'column constraints example'
     ```
   - 💾 **Commit Message:** `"column constraints"`

---

## Altering the Schema

📍 **Next topic: ALTER and CharlieCard schema**  
Carter uses an earlier version of the schema. Make sure yours matches before continuing.

### Set Up the Schema for Alteration

1. Drop all existing tables.
2. Copy the following into your `p2-q.sql`:

    ```sql
    CREATE TABLE "riders" (
        "id" INTEGER,
        "name" TEXT
    );

    CREATE TABLE "stations" (
        "id" INTEGER,
        "name" TEXT,
        "line" TEXT
    );

    CREATE TABLE "visits" (
        "rider_id" INTEGER,
        "station_id" INTEGER
    );
    ```

3. Run the queries to create the schema.
4. **Important:** Comment out these lines after running them.
5. Start writing `ALTER` commands below in `p2-q.sql`, commenting out each one after it’s run.

### Altering Tables

📍 **Timestamp:** 1:03:54  
1. Follow along with Carter's `DROP TABLE` command.  
   ➕ Do this **in your `p2-q.sql` file**, not the terminal, so you have a reference.
2. Add a new H2 heading:
   ```markdown
   ## Altering Tables
   ```
3. Document at least **5 different alteration techniques**, including:
   - Mistakes made
   - Related SQL examples
4. Output `.schema` to `pow-p2.txt`.
5. Write the SQL to `DROP` all tables, run it, and then uncomment the previous setup code.
6. 💾 **Commit Message:** `"ALTER tables"`

---

## Final Steps

1. Rebuild the schema one last time to match Carter’s.
2. Code along and listen for questions and responses—take notes.
3. Carter reviews all the techniques covered.  
   Add a new H1 heading and a summary in `README.md`:
   ```markdown
   # Summary
   ```
   - You may use a paragraph or bullet points.
   - Summarize how each SQL technique was applied.

4. Run your SQL to ensure no syntax errors.
5. Output `.schema` to `pow-p2.txt`.

💾 **Final Commit Message:** `"updating schema"`

---

## Grading Rubric

| Criteria                                                                | Points |
|-------------------------------------------------------------------------|--------|
| ✅ Correct commit history URL for `designing` folder                    | 10     |
| ✅ All required commits are included                                    | 20     |
| ✅ All queries are present in `p2-q.sql`                                | 25     |
| ✅ Correctly created `pow-p2.txt` with required output                  | 20     |
| ✅ Complete and accurate `README.md` content                            | 25     |
| ❗ Late submissions will be penalized 25 points                         |        |
|-------------------------------------------------------------------------|--------|
**Example:** If submitted late but otherwise complete, you will receive 75/100.