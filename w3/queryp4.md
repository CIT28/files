# CS50 Query Part 4
Right-click and select "Open in new tab" to watch [CS50 SQL - Lecture 0 - Querying](https://youtu.be/vHYeChEf2lA?si=hKFR9GDxKMU2JEYo)

## 1. Create your SQL File
* Create a new file named `p4-q.sql` inside your `querying` folder.
* **Do not** manually copy the old file. Instead, copy the code block below and paste it into your new `p4-q.sql` file.

```sql
-- starting the pow workflow
.mode box
.output '| cat >> pow4.txt'

-- ⬇️ WRITE YOUR QUERIES BELOW THIS LINE ⬇️
-- (Remember to .print 'description' before each query)


-- ⬆️ END OF QUERIES ⬆️

-- changes back to stdout
.output stdout

-- bash command (for reference): sqlite3 longlist.db < p4-q.sql
```
## 2. Open Your Terminals

### Terminal 1 (SQlite3 to write queries)
- Navigate to the `querying` folder and then run the following command:

- `sqlite3 longlist.db`

Use this terminal to test queries interactively **before** saving them to your SQL file.

### Terminal 2 (Bash to complete GIT and POW Workflows)
- Navigate to the `querying` folder
- Use this terminal for **Git** and **POW** commands

---

## 3. Initial Commit

In your `README.md`, add the following **Heading 1**:

```md
# Week 3 Querying Part 4
```

Then complete your Git workflow in **Terminal 2**.

📌 **Commit message to use:**  
`query file and README.md ready`

---

## 📺 Part 2: Operators (46:01 – 53:10)

### 1. Notes (`README.md`)
- Start the video at **46:01**
- Add a **Heading 2** to your README:

```md
## Operators
```

- Take notes on the **logical operators** discussed

---

### 2. Code (`p4-q.sql`)
- Follow along with Carter and write each query on **Terminal 1** 
- Once the query has the correct results, copy it into `p4-q.sql` inside the **WRITE QUERIES** section
- Repeat for each query that Carter writes for a total of 6 queries

**Requirement:**  
Use a `.print 'description of query'` line **before each QUERY **

---

### 3. ✅ Checkpoint
- Run the POW:
  - `sqlite3 longlist.db < p4-q.sql`
- Commit your work

📌 **Commit message to use:**  
`Operators and range queries`

---

### 🛑 STOP & CLEAN UP
Before moving to the next section:
- Comment out the queries you just wrote in `p4-q.sql`
- Add `--` before each line

This prevents **duplicate output** in your text file.

---

## 📺 Part 2: ORDER BY (53:10 – 1:02:00)

### 1. Notes (`README.md`)
- Add a **Heading 2**:

```md
## ORDER BY
```

- Take specific notes on **ASC vs DESC**

---

### 2. Code (`p4-q.sql`)
- Write and test the **5 queries** covered in this section

**Requirement:**  
Include `.print` descriptions for each query

---

### 3. ✅ Checkpoint
- Run the POW:
  - `sqlite3 longlist.db < p4-q.sql`
- Commit your work

📌 **Commit message to use:**  
`ORDER BY and notes`

---

### 🛑 STOP & CLEAN UP
- Comment out the **ORDER BY** queries in `p4-q.sql` before continuing

---

## ☕ The “Thursday Break” Option

Feeling the burn? If you have completed everything above, you may pause here.

### To take the break:
- Submit the **URL to your commit history**
- Make sure the previous commit is visible
- Add a submission comment saying:

> Taking the break, will finish by Thursday!

*(If you are not taking the break, continue below.)*

---

## 📺 Part 3: Aggregates (1:02:06 – End)

### 1. Notes (`README.md`)
- Start the video at **1:02:06**
- Add a **Heading 2**:

```md
## Aggregates
```

- Take notes on your understanding of the following:
  - `SUM`
  - `AVG`
  - `MIN`
  - `MAX`

⚠️ **Note:** Pay attention to how `MAX` and `MIN` behave with **string data** and include this in your notes.

---

### 2. Code (`p4-q.sql`)
- Test and write the **14 queries** covered

**Requirement:**  
Include `.print` descriptions for each query

---

### 3. Conclusion (`README.md`)
- At **1:17:21**, listen to the conclusion
- Add a **Heading 2**:

```md
## My Thoughts
```

- Write a solid paragraph reflecting on what you learned during this code-along

---

### 4. ✅ Final Checkpoint
- Run the POW:
  - `sqlite3 longlist.db < p4-q.sql`
- Commit your work

📌 **Commit message to use:**  
`aggregate queries and notes`


## 📤 Submission Instructions
**How to get the correct URL:**
1.  Go to `github.com/CIT28` and navigate to your private repo.
2.  Click on the `querying` folder.
3.  Click on the **History** (clock icon) located at the top right of the file list.
4.  Copy the URL from the address bar.
    * *It should look like this:* `https://github.com/CIT28/yourrepo-pri/commits/main/querying`
5.  Paste this URL into the Canvas assignment submission.

---

## 🔍 How I Grade Your Work
**Transparency Note:** I verify the **content inside your commits**.
When I view your history, I click on specific commits (e.g., *"Operators and range queries"*) to ensure the work was actually completed at that step.

**For every commit checkpoint, I check for 3 things:**
1.  **📝 Notes:** Are the notes for that specific video segment present in `README.md`?
2.  **💻 SQL:** Are the specific queries for that segment present in `p4-q.sql`?
3.  **✅ POW Output:** Does `pow4.txt` show the output results for those specific queries?

*If a commit is empty or missing the associated Notes, SQL, or POW output for that section, points will be deducted.*

---

## 💯 Grading Rubric (100 Points)

**1. Submission URL (10 Points)**
* Did you submit the correct URL to the **folder history** (as shown above)?

**2. Commit History (20 Points)**
* Are all required commits present, and do they contain the required **Notes + SQL + POW** for that section?
* *Required Commits:*
    * "query file and README.md ready"
    * "Operators and range queries"
    * "ORDER BY and notes"
    * "aggregate queries and notes"

**3. SQL Source Code (25 Points)**
* Does your final `p4-q.sql` contain the valid SQL syntax for all queries?

**4. Proof of Work Output (25 Points)**
* Does your final `pow4.txt` contain the results **AND** the descriptions?
  - (Mine had 758 lines)
* *Check:* Did you remember to use `.print` before every query so the output is readable?

**5. Learning Notes (20 Points)**
* Does your final `README.md` contain all required headers and detailed notes?
* *Required Sections:* Operators, Order By, Aggregates, and My Thoughts.

---

### 🕒 Late Policy
* **Penalty:** Work submitted after the due date receives a **25-point deduction**.
* *Example:* A perfect assignment submitted late will receive **75/100**.