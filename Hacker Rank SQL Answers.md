
*[Revising the Select Query I](https://www.hackerrank.com/challenges/revising-the-select-query)
```sql
SELECT *
FROM CITY
WHERE POPULATION > 100000 AND COUNTRYCODE = 'USA'
```

*[Revising the Select Query II](https://www.hackerrank.com/challenges/revising-the-select-query-2)

```sql
SELECT NAME
FROM CITY
WHERE POPULATION >  120000 AND COUNTRYCODE = 'USA'
```

* [Select All](https://www.hackerrank.com/challenges/select-all-sql)
```sql
SELECT * 
FROM CITY 
```
* Problem : Weather Observation Station 6

```sql
SELECT DISTINCT CITY 
FROM STATION 
WHERE LOWER(LEFT(CITY,1)) IN ('a', 'e', 'i', 'o', 'u');
```
--Alternatively
   
* [Problem: Weather Observation Station 7](https://www.hackerrank.com/challenges/weather-observation-station-7)

```sql
SELECT DISTINCT CITY 
FROM STATION 
WHERE LOWER(RIGHT(CITY,1)) IN ('a', 'e', 'i', 'o', 'u');
```

* [Problem: Weather Observation Station 8](https://www.hackerrank.com/challenges/weather-observation-station-8)

```sql
SELECT DISTINCT CITY 
FROM STATION 
WHERE LOWER(RIGHT(CITY,1)) IN ('a', 'e', 'i', 'o', 'u') AND
LOWER(LEFT(CITY,1)) IN ('a', 'e', 'i', 'o', 'u');
```

* [Problem: Weather Observation Station 9](https://www.hackerrank.com/challenges/weather-observation-station-9)

```sql
SELECT DISTINCT CITY 
FROM STATION
WHERE LOWER(LEFT(CITY,1)) NOT IN ('a', 'e', 'i', 'o', 'u');
```

*[Problem: Weather Observation Station 10](https://www.hackerrank.com/challenges/weather-observation-station-10)

```sql
SELECT DISTINCT CITY 
FROM STATION 
WHERE LOWER(RIGHT(CITY,1)) NOT IN ('a', 'e', 'i', 'o', 'u');
```

* [Problem: Weather Observation Station 11](https://www.hackerrank.com/challenges/weather-observation-station-11)

```sql
SELECT DISTINCT CITY 
FROM STATION 
WHERE LOWER(RIGHT(CITY,1)) NOT IN ('a', 'e', 'i', 'o', 'u') OR
LOWER(LEFT(CITY,1)) NOT IN ('a', 'e', 'i', 'o', 'u');
```

*[Problem: Weather Observation Station 12](https://www.hackerrank.com/challenges/weather-observation-station-12)

```sql
SELECT DISTINCT CITY 
FROM STATION 
WHERE LOWER(RIGHT(CITY,1)) NOT IN ('a', 'e', 'i', 'o', 'u') AND
LOWER(LEFT(CITY,1)) NOT IN ('a', 'e', 'i', 'o', 'u');
```

### [Aggregation Challenges](https://www.hackerrank.com/domains/sql/aggregation)

* [Revising Aggregations - The Count Function](https://www.hackerrank.com/challenges/revising-aggregations-the-count-function)

```sql
SELECT COUNT(NAME)
FROM CITY 
WHERE POPULATION > 100000
```

* [Revising Aggregations - The Sum Function](https://www.hackerrank.com/challenges/revising-aggregations-sum)

```sql
SELECT SUM(POPULATION)
FROM CITY 
WHERE DISTRICT = 'CALIFORNIA'
```

* [Revising Aggregations - Averages](https://www.hackerrank.com/challenges/revising-aggregations-the-average-function)

```sql
SELECT AVG(POPULATION)
FROM CITY 
WHERE DISTRICT = 'CALIFORNIA'
```

[Average Population](https://www.hackerrank.com/challenges/average-population)

```sql
SELECT ROUND(AVG(POPULATION),0)
FROM CITY 
```

*[Japan Population](https://www.hackerrank.com/challenges/japan-population)

```sql
SELECT SUM(POPULATION)
FROM CITY 
WHERE COUNTRYCODE = 'JPN'
```

* [Population Density Difference](https://www.hackerrank.com/challenges/population-density-difference)

```sql
SELECT MAX(POPULATION) - MIN(POPULATION)
FROM CITY
```

* [Weather Observation Station 2](https://www.hackerrank.com/challenges/weather-observation-station-2)

```sql
SELECT ROUND(SUM(LAT_N),2), ROUND(SUM(LONG_W),2)
FROM STATION
```


* [Weather Observation Station 13](https://www.hackerrank.com/challenges/weather-observation-station-13)

```sql
SELECT ROUND(SUM(LAT_N),4)
FROM STATION
WHERE LAT_N > 38.7880 AND LAT_N < 137.2345
```
* [Weather Observation Station 14](https://www.hackerrank.com/challenges/weather-observation-station-14)

```sql
SELECT ROUND(MAX(LAT_N),4)
FROM STATION
WHERE LAT_N < 137.2345
```

* [Weather Observation Station 15](https://www.hackerrank.com/challenges/weather-observation-station-15)

```sql
SELECT ROUND(LONG_W, 4)
FROM STATION
WHERE LAT_N < 137.2345 AND CASE WHEN LAT_N = MAX(LAT_N)
```


-- AGGREGATION CHALLENGES
--https://www.hackerrank.com/challenges/the-blunder


*[Top Earners](https://www.hackerrank.com/challenges/earnings-of-employees)

```sql
SELECT MAX(months*salary) AS earnings, COUNT(earnings)
FROM EMPLOYEE
```

















































































