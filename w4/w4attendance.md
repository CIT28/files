# 💻 Week 4 Attendance

# Setup
## 1. New folder(s)
* In your pri repo create a new folder named `ps0` and then make that the current folder and create another folder named `cyberchase`. 
* Make sure you have the `cyberchase` as the current folder and then copy the following command and paste into the terminal:
- ```curl -o cyberchase.db https://raw.githubusercontent.com/CIT28/files/main/w4/cyberchase.db```

## 2. Create your SQL File
* Create a new file named `w4-q.sql` inside your `ps0/cyberchase` folder.
* **Do not** manually copy the old file. Instead, copy the code block below and paste it into your new `w4-q.sql` file.

```sql
-- starting the pow workflow
.mode box
.output '| cat >> pow-ds.txt'

-- ⬇️ WRITE YOUR QUERIES BELOW THIS LINE ⬇️
-- (Remember to .print 'description' before each query)


-- ⬆️ END OF QUERIES ⬆️

-- changes back to stdout
.output stdout

-- bash command (for reference): sqlite3 cyberchase.db < w4-q.sql
```
## 2. Open Your Terminals

### Terminal 1 (SQlite3 to write queries)
- Navigate to the `ps0/cyberchase` folder and then run the following command:

- `sqlite3 cyberchase.db`
- `.mode box`

Use this terminal to test your queries interactively **before** saving them to your SQL file. This process captures your problem-solving history, which serves as your **Proof of Effort (POE)**.

### Terminal 2 (Bash to complete GIT and POW Workflows)
- Navigate to the `ps0/cyberchase` folder
- Use this terminal for **Git** and **POW** commands

---

## 3. Initial Commit

In the `ps0/cyberchase` create a new file named `README.md`, add the following **Heading 1**:

```md
# Week 4 Attendance Proof of Work
```

Then complete your Git workflow in **Terminal 2**.

📌 **Commit message to use:**  
`new folder, files and db`

---

# New DataSet 

## 1. Update the w4-q.sql
In the w4-q.sql add this commmand:
`.schema`
Then on a new line add this query:
`SELECT * FROM "episodes`;

## 2. ✅ Proof of Work
- In terminal 2 run the POW:
  - `sqlite3 cyberchase.db < w4-q.sql`

## 🚀 Git Commit
- Commit your work **immediately after generating the POW**
- Use the following commit message format:

```text
cyberchase ds 
```
## What is in the cyberchase database
* https://cs50.harvard.edu/sql/psets/0/cyberchase/#schema

* Before going to the code challenge change this line in the w4-q.sql file:
    - from `.output '| cat >> pow-ds.txt'`
    - to `.output '| cat >> pow-w4.txt'`
---

# Code Challenge 

## 1. List episodes (Follow along with me)

**Task:**  
On the terminal write a SQL query to list the titles of all episodes in Cyberchase’s original season, Season 1.

**Validation:**
- **Columns:** 1 (`title`)
- **Rows:** 26

## 2. Find Production Code (Your Turn)

**Task:**  
Find the title and production code for the episode “Hackerized!”.

**Validation:**
- **Columns:** 1 (`title`)
- **Rows:** 21

# ⚙️ The Workflow (Repeat for **EACH** Problem)


## ❌ Fail / Verify

## If it gives an **Error**  
Example: `Parse error: no such column...`

1. **STOP.** Do not clear the screen.  
2. Select the text in the terminal (**your failed query + the error message**).  
3. Paste it into `README.md` **inside a code block** 
    - To display a block of code, wrap the content with three backticks (```` ``` ````) on the lines immediately before and after the code.

## 🔧 Refine
Try again until you get the correct result matching the **Validation** criteria.

### 🏁 Finalize
Once correct:
- Copy **only** the working SQL query into `w4-q.sql` for the official solution.

## If it gives **Wrong Data**
1. Select the query + the **first few rows** of the wrong result.  
2. Paste it into `README.md`.


## ✅ Proof of Work
- In terminal 2 run the POW:
  - `sqlite3 cyberchase.db < w1-q.sql`

---

## 🚀 Git Commit
- Commit your work **immediately after generating the POW**
- Use the following commit messages:
    * 1. ```Following along with Rio```
    * 2. ```Trying it on my own```

```text
Commit Message from above
```
---

### 🛑 STOP & CLEAN UP
Before moving to the next section:
- Comment out the queries you just wrote in `w4-q.sql`
- Add `--` before each line



