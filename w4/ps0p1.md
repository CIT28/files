# CS50 Problem Set 0 Part 1 
## Normals 1 thru 6

In the video I will walk how to complete this work:
### Setup
- In the ps0 folder, create another folder named normals.   
- Change the current folder to normals, then use the following command to copy the database file:
    - ```curl -o normals.db https://raw.githubusercontent.com/CIT28/files/main/w4/normals.db```
    - Create a file to store the queries name it p1-q.sql and a README.md with a heading for each problem 1 thru 6, commit with message:
      - **COMMIT MESSAGE - "setup complete"**
### For each problem you need to do the following
- For each problem, you need to:
1. Write the query in the p1-q.sql file and make sure you get the correct output (see below) 
2. In the README.md, authenicate your work by copying the steps you took to get the correct output, do this under the heading for each problem.    
3. Open another terminal session to change the standard output to sent the output to powp1.txt, commit with message:
  - **COMMIT MESSAGE - "1. query, pow  and README.md complete"**
  - Comment out the current query and then work on next query and use the same commit message, just updating the number (ex. "2. query, pow  and README.md complete")
 
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

1. Write a SQL query to find the normal ocean surface temperature in the Gulf of Maine, off the coast of Massachusetts. To find this temperature, look at the data associated with 42.5° of latitude and -69.5° of longitude.
    - Recall that you can find the normal ocean surface temperature in the 0m column, which stands for 0 meters of depth!
2. Write a SQL query to find the normal temperature of the deepest sensor near the Gulf of Maine, at the same coordinate above.
    - The deepest sensor records temperatures at 225 meters of depth, so you can find this data in the 225m column.
3. Choose a location of your own and write a SQL query to find the normal temperature at 0 meters, 100 meters, and 200 meters. You might find Google Earth helpful if you’d like to find some coordinates to use!
4. Write a SQL query to find the lowest normal ocean surface temperature.
5. Write a SQL query to find the highest normal ocean surface temperature.
6 Write a SQL query to return all normal ocean temperatures at 50m of depth, as well as their respective degrees of latitude and longitude, within the Arabian Sea[https://en.wikipedia.org/wiki/Arabian_Sea]. Include latitude, longitude, and temperature columns. For simplicity, assume the Arabian Sea is encased in the following four coordinates:
    - 20° of latitude, 55° of longitude
    - 20° of latitude, 75° of longitude
    - 0° of latitude, 55° degrees of longitude
    - 0° of latitude, 75° degrees of longitude

## How to Test
Executing 1. results in a table with 1 column and 1 row.
Executing 2.  results in a table with 1 column and 1 row.
3.sql is up to you!
Executing 4. results in a table with 1 column and 1 row.
Executing 5. results in a table with 1 column and 1 row.
Executing 6 results in a table with 3 columns and 383 rows.

## Grading
- Submit your commit history URL your normals in your private repo for grading
- This is how I will grade your work:
1. Did you provide the correct URL for normals folder = 5 points.
2. Did you do all the commits required for this work = 65 points
    -  There should be 7 commits, 1 for the setup and 6 that show the current query (uncommented), proof of work and autenciate work in README.md
3. Did your README.md file show authenicate work =  30 points
4. Work submitted after the due date will be reduced by 25 points. If you completed all the requirements above, but submitted after the due date you will get 75 points (100 - 25) on this work. 