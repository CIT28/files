# CS50 Problem Set 1 - Devious Delivery Nested Subquery and JOIN

## Devious Delivery Nested Subquery

1. Review the problem
    - Good day to you, deliverer of the mail. You might remember that not too long ago I made my way over from the town of Fiftyville. I gave a certain box into your reliable hands and asked you to keep things low. My associate has been expecting the package for a while now. And yet, it appears to have grown wings and flown away. Ha! Any chance you could help clarify this mystery? Afraid there’s no “From” address. It’s the kind of parcel that would add a bit more… quack to someone’s bath times, if you catch my drift.

    - Unlike the CS50 example here is what you will need to write query(s) to answer - "What was the Drop off address"? 
        - Here is the final output for nested subquery:
        <pre>
        ┌──────────────────┐
        │     address      │
        ├──────────────────┤
        │ 7 Humboldt Place │
        └──────────────────┘
        </pre>

2. Write nested query
- In your README.md file create a heading 2 for "Nested Queries for Devious Delivery - Proof of Effect.
- In the packages folder create a new file named dd-q.sql and copy previous sql file, update pow reference to be pow-dd.txt and update the bash reference.
    - Then write the nested subquery to solve the Devious Delivery,  only 1 nested subquery here. 
    - Once you have a working query complete the poe, pow and git workflow with message 
        - **COMMIT MESSAGE - "Lost Letter nested subquery"**

## BREAK OPTIONAL  
- If you got this far you can take a break and complete the rest of this work by the Thursday night deadline.  
- To "GET" this break you will submit your commit history for the packages folder now.
- I will do a review and give you feedback.
- If you complete before Thurs morning, then you can submit again your commit history URL and tell me that you are ready for a second review. 

3. Write JOIN query
- In your README.md file create a heading 2 for "Join Query for Devious Delivery - Proof of Effect.  
    - Then write the nested subquery to solve the Devious Delivery, there should be at 1 JOIN query here. 
    - Here the output is different but the query logic is these same:
    - <pre>
┌──────────────────┬─────────────────────┐
│ Drop Off Address │ Contents of Package │
├──────────────────┼─────────────────────┤
│ 7 Humboldt Place │ Duck debugger       │
└──────────────────┴─────────────────────┘
</pre>
    - Once you have a working query complete the poe, pow and git workflow with message 
        - **COMMIT MESSAGE - "Devious Delivery Join Query"**

## Grading
- Submit your commit history URL the packages folder in your private repo for grading

This is how I will grade your work:
1. Did you provide the correct URL for packages folder commits = 5 points.
2. Did you do all the commits required for this work = 20 points
3. Did your poe show authenticate work =  45 points
4. Did you get the correct output for both static and nested queries = 30 points
- Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 