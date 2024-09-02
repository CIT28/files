# CS50 Problem Set 0 Part 1 
## Normals 7 thru 10

### Setup
- We will continue working in the ps0/normals folder. 
    - Create a file to store the queries name it p2-q.sql and in README.md add an heading for each problem 7 thru 10, commit with message:
      - **COMMIT MESSAGE - "setup complete"**
### For each problem you need to do the following
- For each problem, you need to:
1. Write the query in the p2-q.sql file and make sure you get the correct output (see below) 
2. In the README.md, as covered in the Week 4 attendance, create a new heading for this work name Normals Problem Set Part 2 and a heading for each problem. 
3. Open another terminal session to change the standard output to sent the output to powp2.txt, commit with message:
  - **COMMIT MESSAGE - "7. query, pow and README.md complete"**
  - Comment out the current query and then work on next query and use the same commit message, just updating the number (ex. "8. query, pow  and README.md complete")
 
## Schema
The data in normals.db can be visualized as shown:
https://cs50.harvard.edu/sql/2024/psets/0/normals/normals.jpg
Notice that the earth is divided into a grid of coordinates—points that can identify most any location on earth. Each coordinate is a combination of latitude and longitude. And notice how each coordinate over an ocean has some normal ocean surface temperature associated with it!

In normals.db you’ll find a single table of coordinates, normals. In the normals table, you’ll find the following columns:

- id, which uniquely identifies each row (coordinate) in the table
- latitude, which is the degree of latitude (expressed in decimal format) for the coordinate
- longitude, which is the degree of longitude (expressed in decimal format) for the coordinate
- 0m, which is the normal ocean surface temperature (i.e., the normal temperature at 0 meters of depth), in degrees Celsius, at the coordinate
- 5m, which is the normal ocean temperature at 5 meters of depth, in degrees Celsius, at the coordinate
- 10m, which is the normal ocean temperature at 10 meters of depth, in degrees Celsius, at the coordinate

And observations continue until 5500m, or 5500 meters of depth, for some coordinates!

Since normals is a wide table, if you want to preview the contents, consider SELECTing only the latitude, longitude, and a few depth columns.

## Specification

For each of the following questions, you should write a single SQL query that outputs the results specified by each problem. Your response must take the form of a single SQL query. You should not assume anything about the ids of any particular observations: your queries should be accurate even if the id of any particular observation were different. Finally, each query should return only the data necessary to answer the question.

7. Write a SQL query to find the average ocean surface temperature, rounded to two decimal places, along the equator. Call the resulting column “Average Equator Ocean Surface Temperature”.
    - The equator’s ocean surface temperatures can be found at all longitudes between the latitudes -0.5° and 0.5°, inclusive.
8. Write a SQL query to find the 10 locations with the lowest normal ocean surface temperature, sorted coldest to warmest. If two locations have the same normal ocean surface temperature, sort by latitude, smallest to largest. Include latitude, longitude, and surface temperature columns.
9. Write a SQL query to find the 10 locations with the highest normal ocean surface temperature, sorted warmest to coldest. If two locations have the same normal ocean surface temperature, sort by latitude, smallest to largest. Include latitude, longitude, and surface temperature columns.

10. There are 180 whole degrees of latitude. Write a SQL query to determine how many points of latitude we have at least one data point for. (Why might we not have data points for all latitudes?)


## How to Test
Executing 7 results in a table with 1 column and 1 row.
Executing 8 results in a table with 3 columns and 10 rows.
Executing 9 results in a table with 3 columns and 10 rows.
Executing 10 results in a table with 1 column and 1 row.

## Grading
- Submit your commit history URL your normals in your private repo for grading
- This is how I will grade your work:
1. Did you provide the correct URL for normals folder commits = 5 points.
2. Did you do all the commits required for this work = 65 points
    -  There should be 5 commits, 1 for the setup and 4 that show the current query (uncommented), proof of work and autenciate work in README.md
3. Did your README.md file show authenicate work =  30 points
4. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 