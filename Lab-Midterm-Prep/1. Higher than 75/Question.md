# Querying Student Names Based on Marks

This solution queries the `STUDENTS` table to find the names of students who scored higher than a specified `Marks` value. The output is ordered by the last three characters of each student's name, and if multiple names end with the same three characters, the results are secondarily sorted by the `ID` in ascending order.

## Table Structure

The `STUDENTS` table is described as follows:
- **ID**: Unique identifier for each student.
- **NAME**: Contains uppercase (A-Z) and lowercase (a-z) letters only.
- **MARKS**: Represents the marks scored by each student.

## Query

```sql
SELECT name from STUDENTS where marks > 75 ORDER BY SUBSTRING(NAME, -3) ASC, ID ASC;

```
# Querying Student Names Based on Marks

This solution queries the `STUDENTS` table to find the names of students who scored higher than a specified `Marks` value. The output is ordered by the last three characters of each student's name, and if multiple names end with the same three characters, the results are secondarily sorted by the `ID` in ascending order.

## Table Structure

The `STUDENTS` table is described as follows:
- **ID**: Unique identifier for each student.
- **NAME**: Contains uppercase (A-Z) and lowercase (a-z) letters only.
- **MARKS**: Represents the marks scored by each student.

## Query

```sql
SELECT NAME
FROM STUDENTS
WHERE MARKS > [specified_marks]
ORDER BY RIGHT(NAME, 3), ID;

### Sample Output

Assuming the following students scored above 75:

| ID  | NAME    | MARKS |
|-----|---------|-------|
| 1   | Ashley  | 80    |
| 2   | Julia   | 85    |
| 3   | Belvet  | 90    |



```

### Explanation of Sample Output

- Only `Ashley`, `Julia`, and `Belvet` have `Marks > 75`.
- Sorting by the last three characters gives: 'ley' (Ashley), 'lia' (Julia), and 'vet' (Belvet), with no duplicate endings.
