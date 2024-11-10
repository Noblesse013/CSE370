To find the total population of all cities in the `CITY` table where the `District` is "California," you can use the following SQL query. This query sums the `Population` column for rows where the `District` column matches "California."

```sql
SELECT SUM(Population) AS total_population
FROM CITY
WHERE District = 'California';
```

### Explanation

1. **`SUM(Population) AS total_population`**: Calculates the total population of cities by summing up the values in the `Population` column and renames the output as `total_population`.
2. **`FROM CITY`**: Specifies the `CITY` table as the source of data.
3. **`WHERE District = 'California'`**: Filters the rows to include only those where the `District` column is equal to "California."

### Example Output

If the cities in the `CITY` table with `District` as "California" have populations of 500,000, 300,000, and 200,000, the output would be:

```
total_population
1000000
```

This query provides the total population for all cities in California.
