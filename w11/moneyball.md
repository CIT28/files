# CS50 Problem Set 1: Moneyball ⚾
## The Quest for Value in the Major Leagues

## Week 11 Attendance 

### Setup
- Inside your `ps1` folder, create a new folder named `moneyball`.
- Let's review the schema for this dataset:
    * https://cs50.harvard.edu/sql/psets/1/moneyball/#schema
- Change your current folder to `moneyball`, then use the following command to download the database:
    - ```curl -o moneyball.db https://raw.githubusercontent.com/CIT28/files/main/w11/moneyball.db```
- Create a new query file (`mball-q.sql`) from previous query file remove any queries written and create a new `README.md`.
- Create `README.md` and heading 1 `# Week 11 Moneyball `
- Update the `mball-q.sql` POW to be `pow-ds.txt`
- Perform the standard dataset inspection:
    1. `.table`
    2. `.schema`
    3. Code a query to list the first 10 records of each table in the moneyball.db: `performances`, `players`, `salaries`, and `teams`
- **COMMIT MESSAGE - "new dataset"**
- Comment out the queries and commands above.
- Update the `mball-q.sql` POW to be `pow-w11.txt`
- Create `README.md` with Heading 2 `## Attendance Problem`
- Review the Task and the Workflow Loop
- **COMMIT MESSAGE - "week 11 attendance problem"**

---

## Week 11 Attendance: The "2001 Oakland Audit"

**The Context:**
The year is **2001**. You’ve been hired by the Oakland Athletics. Your first task is to audit the roster during this iconic season to see how the "A's" were spending their limited budget.

**Task:**
Find the `first_name`, `last_name`, and `salary` of every player who played for the **'Oakland Athletics'** in the year **2001**.

* **Architectural Constraint:** You must use a **Triple Join** to connect the player names to a human-readable team name from the `teams` table.
* Use table aliasing for all tables (e.g., `players AS p`, `salaries AS s`, `teams AS t`).
* Order the results by `salary` from highest to lowest.


**Validation:**
- **Columns:** 3 (`first_name`, `last_name`, `salary`)
- **Rows:** 27



## Week 11 Problem Set - MoneyBall
- Update the mball-q.sql pow to be pow-mball.txt
    
## ⚙️ The Workflow (Repeat for **EACH** Problem)

For **every problem** listed below (**1 through 6**), you must perform this exact cycle:

---
## 1. Add problem heading to README.md

In your `README.md`, add the following **Heading 2**:

```md
## Problem # 
```

## 🔁 The Loop 

---

### ✅ Attempt
Type your best-guess query in the terminal.

---

### ❌ Fail / Verify

### If it gives an **Error**  
Example: `Parse error: no such column...`

1. **STOP.** Do not clear the screen.  
2. Select the text in the terminal (**your failed query + the error message**).  
3. Paste it into `README.md` **inside a code block** 

### If it gives **Wrong Data**
1. Select the query + the **first few rows** of the wrong result.  
2. Paste it into `README.md`.

---

### 🔧 Refine
Try again until you get the correct result matching the **Validation** criteria.

---

### 🏁 Finalize
Once correct:
- Copy **only** the working SQL query into `mball-q.sql` for the official solution.

---

## 3. ✅ Proof of Work

## 🚀 Git Commit
- Commit your work **immediately after generating the POW**
- Use the following commit message format:

```text
Problem #
```
---

### 🛑 STOP & CLEAN UP
Before moving to the next section:
- Comment out the queries you just wrote in `mball-q.sql`
- Add `--` before each line

## REPEAT FOR EACH PROBLEM
---

## ⚙️ The Workflow (Repeat for **EACH** Problem)
Follow the **Attempt -> Fail/Verify -> Refine -> Finalize** loop.

---

## Problem 1: The "Home Run Heroes" (JOIN Version)

**The Context:**
While the A's were looking for value, the rest of the league was chasing power. Let's find the heavy hitters from that same year.

**Task:**
Identify the `first_name`, `last_name`, and number of home runs (`HR`) for all players who hit **40 or more home runs** in the year **2001**.

* **Architectural Constraint:** Use an **Inner Join** to connect names in the `players` table to their hitting statistics in the `performances` table.
* Order the results by `HR` from highest to lowest.

**Validation:**
- **Columns:** 3 (`first_name`, `last_name`, `HR`)
- **Rows:** 12

---

## Problem 2: The "Home Run Heroes" (Subquery Version)

**Task:**
Identify the `first_name` and `last_name` of all players who hit **40 or more home runs** in the year **2001**. 

* **Architectural Constraint:** You are **forbidden** from using a JOIN for this specific query. You must use a **Nested Subquery** (using the `IN` operator) to filter the player list.



**Validation:**
- **Columns:** 2 (`first_name`, `last_name`)
- **Rows:** 12

---

## Problem 3: The "Payroll Gap" (Aggregates)

**The Context:**
In 2001, the New York Yankees spent over $112M while the A's spent only $33M. Let's visualize that gap across the whole league.

**Task:**
Identify the **total payroll** for every Major League team in the year **2001**.

* **Architectural Constraint:** Use the `SUM()` aggregate function on the `salary` column and a **Group By** clause on the team name.
* Alias the sum as `total_payroll`.
* Order the results by `total_payroll` from highest to lowest.



**Validation:**
- **Columns:** 2 (`name`, `total_payroll`)
- **Rows:** 30

---
## BREAK OPTIONAL  
- If you have completed 1, 2 and 3 problems than you can take a break and complete the rest of this work by the Thursday night deadline.
- To "GET" this break you will submit your commit history for the packages folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 
---

## Problem 4: The "Cheap Speed" (Value Discovery)

**Task:**
Find the `first_name`, `last_name`, and `salary` of all players who had **more than 30 stolen bases (`SB`)** in **2001**, but earned a salary of **less than $1,000,000**.

* **Architectural Constraint:** This requires a **Triple Join** between `players`, `salaries`, and `performances`. Ensure your `WHERE` clause filters for the year **2001** across the tables to ensure data alignment.
* Order by `salary` from lowest to highest.

**Validation:**
- **Columns:** 3 (`first_name`, `last_name`, `salary`)
- **Rows:** 5

---

## Problem 5: The "One-Club Men" (Negative Logic)

**The Context:**
In the era of "Moneyball," players were traded constantly. Let's find the "Loyalists"—players on the 2001 Oakland roster who have **no records** of ever playing for any other team in this database.

**Task:**
Identify the `first_name` and `last_name` of all players who played for the **'Oakland Athletics'** in **2001**, but have **never** played for any other team.

* **Architectural Constraint:** This query requires **Negative Logic**. You must use a subquery with the `NOT IN` operator to exclude any player who has a performance record with a `team_id` other than Oakland's.



**Validation:**
- **Columns:** 2 (`first_name`, `last_name`)
- **Rows:** 15

---

## Problem 6: The "Finale" (The All-Star Value Report)

**Task:**
Find the `first_name`, `last_name`, and `salary` of players who played for the **'Oakland Athletics'** in **2001** and recorded **at least 150 hits (`H`)**.

* **Architectural Constraint:** This is a **Quad-Join**. You must successfully bridge `players`, `salaries`, `performances`, and `teams` into a single result set using shared ID columns.
* Order by `salary` (lowest to highest) to highlight the best value first.



**Validation:**
- **Columns:** 3 (`first_name`, `last_name`, `salary`)
- **Rows:** 5


## 💯 Grading Rubric (100 Points)

**1. Submission URL (10 Points)**
* Did you submit the correct URL to the **folder history** `ps1/moneyball` 

**2. Commit History (10 Points)**
* Are all required commits present, and do they contain the required **POE + SQL + POW** for that section?
* *Required Commits:*
    * "Problem 1"
    * ...
    * ...
    * "Problem 6"

**3. SQL Source Code (25 Points)**
* Does your final `mball-q.sql` contain the valid SQL syntax for all queries?

**4. Proof of Work Output (15 Points)**
* Does your final `pow-mball.txt` contain the results **AND** the descriptions?
* *Check:* Did you remember to use `.print` before every query so the output is readable?

**5. Proof of Effort (40 Points)**
* Does your final `README.md` contain all required headers and authenicate attempts?
* *Required Sections:* Problem 1....thru Problem 6.

**6. Scope of Work.**
* Limit your code to the specific SQL concepts covered in this course so far. The goal is to demonstrate your understanding of the current material. Note: Using SQL functions or syntax we haven't covered yet will be flagged as AI-generated code and points will be deducted.  
---