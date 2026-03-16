# CS50 Problem Set 1 DESE 
## Department of Elementary and Secondary Education

## Week 10 Attendance 

### Setup
- Inside the folder ps1 folder, make sure it is at the same level as packages create another folder named dese.
- Let's review a key statement on the CS50 page for this problem set:
    * https://cs50.harvard.edu/sql/psets/1/dese/#schema
- Change the current folder to dese, then use the following command to copy the database file:
    - ```curl -o dese.db https://raw.githubusercontent.com/CIT28/files/main/w10/dese.db```
    - Create a new query file (dese-q.sql) by copying a previous sql file we have used. Remove any queries in the file and update bash command and pow reference to be pow-ds.txt.
    - Create README.md and heading 1 `# Week 10 DESE `
    - Do the normal new dataset queries:
        1. .table
        2. .schema
        3. Code a query for listing the first 10 records of each table
        - **COMMIT MESSAGE - "new dataset"**

- Update the dese-q.sql pow to be pow-w10.txt

- Create heading 2 `## Attendance Problem`
- Review the Task and the Workflow Loop below
- Commit Message - `week 10 attendance problem`

## Week 10 Attendance: The "Dropout" Diagnostic

**Task:**
Find the **average dropout rate** of all schools located in districts categorized as a **"Charter District"**. 

**Validation:**
- **Columns:** 1 (`average_dropout_rate`)
- **Rows:** 1

---

## Week 10 Problem Set - DESE
- Update the dese-q.sql pow to be pow-dese.txt
    
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
- Copy **only** the working SQL query into `dese-q.sql` for the official solution.

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
- Comment out the queries you just wrote in `dese-q.sql`
- Add `--` before each line

## REPEAT FOR EACH PROBLEM


### Problem 1: The "Perfect Finish" (Architectural Challenge I)

**Task:**
Identify the names of all **Public School Districts** that contain at least one school with a **100% graduation rate**. Your solution must use **JOINs** to connect the necessary data. Ensure the final list contains no duplicate district names.

**Validation:**
- **Columns:** 1 (`name`)
- **Rows:** 9

---

## Problem 2: The "Perfect Finish" (Architectural Challenge II)

**Task:**
Identify the names of all **Public School Districts** that contain at least one school with a **100% graduation rate**. Your solution must use **nested subqueries** rather than JOINs to achieve the result. 

**Validation:**
- **Columns:** 1 (`name`)
- **Rows:** 9

## Problem 3: The "Bang for Your Buck" Analysis

**Task:**
Identify the **city** in Massachusetts that has the **highest average per-pupil expenditure**, but only consider cities that contain **at least 10 public schools**. 

**Validation:**
- **Columns:** 1 (`city`)
- **Rows:** 1

## BREAK OPTIONAL  
- If you have completed 1, 2 and 3 problems than you can take a break and complete the rest of this work by the Thursday night deadline.
- To "GET" this break you will submit your commit history for the packages folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 


## Problem 4: The "Charter Challenge"

**Task:**
Identify the `name` of every school that belongs to a **Charter District** with a per-pupil expenditure of **less than $15,000**.

**Validation:**
- **Columns:** 1 (`name`)
- **Rows:** 4

## Problem 5: The "Purely Public" Districts

**Task:**
Identify the `name` of every **Public School District** that contains **zero** Charter Schools. 
* Use a **subquery** with the `NOT IN` operator to filter the results.
* Ensure your results are limited only to districts of the "Public School District" type.

**Validation:**
- **Columns:** 1 (`name`)
- **Rows:** 520

## Problem 6: The "Investment" Report

**Task:**
Identify the `name` and the **average graduation rate** of every district that spends **more than $20,000** per pupil. 
* Use **JOINs** to connect the districts, their expenditures, and their schools' graduation rates.
* Alias the average graduation rate column as `average_graduation_rate`.
* Group the results by district name and order them from the highest average graduation rate to the lowest.

**Validation:**
- **Columns:** 2 (`name`, `average_graduation_rate`)
- **Rows:** 99

## 💯 Grading Rubric (100 Points)

**1. Submission URL (10 Points)**
* Did you submit the correct URL to the **folder history** `ps1/dese` 

**2. Commit History (10 Points)**
* Are all required commits present, and do they contain the required **POE + SQL + POW** for that section?
* *Required Commits:*
    * "Problem 1"
    * ...
    * ...
    * "Problem 6"

**3. SQL Source Code (25 Points)**
* Does your final `dese-q.sql` contain the valid SQL syntax for all queries?

**4. Proof of Work Output (15 Points)**
* Does your final `pow-dese.txt` contain the results **AND** the descriptions?
* *Check:* Did you remember to use `.print` before every query so the output is readable?

**5. Proof of Effort (40 Points)**
* Does your final `README.md` contain all required headers and authenicate attempts?
* *Required Sections:* Problem 1....thru Problem 6.

**6. Scope of Work.**
* Limit your code to the specific SQL concepts covered in this course so far. The goal is to demonstrate your understanding of the current material. Note: Using SQL functions or syntax we haven't covered yet will be flagged as AI-generated code and points will be deducted.  
---

### 🕒 Late Policy
* **Penalty:** Work submitted after the due date receives a **25-point deduction**.
* *Example:* A perfect assignment submitted late will receive **75/100**.

### 💡 Hints for Success

#### 1. The "Middle-Man" Table
In almost every problem this week, you will need to connect **Districts** (where the money and names are) to **Graduation Rates** (where the performance data lives). 
* Notice that `graduation_rates` has a `school_id`, but it does **not** have a `district_id`.
* You must use the `schools` table as a **bridge** because it contains both a `school_id` and a `district_id`.

#### 2. Aliasing for Clarity
When joining three or four tables, typing full table names like `graduation_rates.graduated` becomes difficult to manage. Use short aliases to keep your code readable and to save time:
* `FROM districts AS d`
* `JOIN schools AS s ON d.id = s.district_id`

#### 3. Inclusion vs. Exclusion Logic
* **Problem 2:** Think "Inside-Out." Start with the graduation rates, find the associated schools, and finally pull the district names that own those schools.
* **Problem 5:** To find districts with **zero** charter schools, searching for "Public" schools isn't enough (a district could have both). You must find all districts that have *any* charter schools and then use the `NOT IN` operator to exclude them from your results.

#### 4. The Grouping Rule
Whenever you use an aggregate function like `AVG()` or `COUNT()` alongside a regular column (like `d.name` in Problem 6), you **must** include a `GROUP BY` clause for that column. This tells SQL how to "bucket" the data before it calculates the average for each group.
