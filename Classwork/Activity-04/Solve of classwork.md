### Task 3:
Retrieve all customer’s id, name, city and account number using
1. Inner Join:
```sql
MariaDB [bank]> select c2.customer_id, c1.customer_name, c1.customer_city ,c2.account_number from customer c1 inner join depositor c2 on c1.customer_id = c2.customer_id;
```

```
+-------------+---------------+---------------+----------------+
| customer_id | customer_name | customer_city | account_number |
+-------------+---------------+---------------+----------------+
| C-101       | Jones         | Harrison      | A-217          |
| C-201       | Smith         | Rye           | A-215          |
| C-211       | Hayes         | Harrison      | A-102          |
| C-215       | Lindsay       | Pittsfield    | A-222          |
| C-220       | Turner        | Stamford      | A-305          |
| C-226       | Johnson       | Palo Alto     | A-101          |
| C-226       | Johnson       | Palo Alto     | A-201          |
+-------------+---------------+---------------+----------------+
```
2. Left Join:
```sql
MariaDB [bank]> select c2.customer_id, c1.customer_name, c1.customer_city ,c2.account_number from customer c1 left join depositor c2 on c1.customer_id = c2.customer_id;
```

```
+-------------+---------------+---------------+----------------+
| customer_id | customer_name | customer_city | account_number |
+-------------+---------------+---------------+----------------+
| C-101       | Jones         | Harrison      | A-217          |
| C-201       | Smith         | Rye           | A-215          |
| C-211       | Hayes         | Harrison      | A-102          |
| NULL        | Curry         | Rye           | NULL           |
| C-215       | Lindsay       | Pittsfield    | A-222          |
| C-220       | Turner        | Stamford      | A-305          |
| NULL        | Williams      | Princeton     | NULL           |
| NULL        | Adams         | Pittsfield    | NULL           |
| C-226       | Johnson       | Palo Alto     | A-101          |
| C-226       | Johnson       | Palo Alto     | A-201          |
| NULL        | Glenn         | Woodside      | NULL           |
| NULL        | Brooks        | Brooklyn      | NULL           |
| NULL        | Green         | Stamford      | NULL           |
+-------------+---------------+---------------+----------------+
```
3. Right Join
```sql
select c2.customer_id, c1.customer_name, c1.customer_city ,c2.account_number from customer c1 right join depositor c2 on c1.customer_id = c2.customer_id;
```
```
+-------------+---------------+---------------+----------------+
| customer_id | customer_name | customer_city | account_number |
+-------------+---------------+---------------+----------------+
| C-101       | Jones         | Harrison      | A-217          |
| C-201       | Smith         | Rye           | A-215          |
| C-211       | Hayes         | Harrison      | A-102          |
| C-215       | Lindsay       | Pittsfield    | A-222          |
| C-220       | Turner        | Stamford      | A-305          |
| C-226       | Johnson       | Palo Alto     | A-101          |
| C-226       | Johnson       | Palo Alto     | A-201          |
+-------------+---------------+---------------+----------------+
```
4. Full join
```sql
MariaDB [bank]> select c2.customer_id, c1.customer_name, c1.customer_city ,c2.account_number from customer c1 left join depositor c2 on c1.customer_id = c2.customer_id union select c2.customer_id, c1.customer_name, c1.customer_city ,c2.account_number from customer c1 right join depositor c2 on c1.customer_id = c2.customer_id;
```

```
+-------------+---------------+---------------+----------------+
| customer_id | customer_name | customer_city | account_number |
+-------------+---------------+---------------+----------------+
| C-101       | Jones         | Harrison      | A-217          |
| C-201       | Smith         | Rye           | A-215          |
| C-211       | Hayes         | Harrison      | A-102          |
| NULL        | Curry         | Rye           | NULL           |
| C-215       | Lindsay       | Pittsfield    | A-222          |
| C-220       | Turner        | Stamford      | A-305          |
| NULL        | Williams      | Princeton     | NULL           |
| NULL        | Adams         | Pittsfield    | NULL           |
| C-226       | Johnson       | Palo Alto     | A-101          |
| C-226       | Johnson       | Palo Alto     | A-201          |
| NULL        | Glenn         | Woodside      | NULL           |
| NULL        | Brooks        | Brooklyn      | NULL           |
| NULL        | Green         | Stamford      | NULL           |
+-------------+---------------+---------------+----------------+
```
