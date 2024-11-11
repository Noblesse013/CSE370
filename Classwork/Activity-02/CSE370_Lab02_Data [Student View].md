**Lab 02 Data** 

**Initial Table: It's a bit different than Lab 01\!**

| std\_id | name | major | section | days\_present | project\_marks | cgpa | submission\_date |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| s001 | Abir | CS | 1 | 10 | 18.5 | 3.91 | 2018-09-15 |
| s002 | Nafis | CSE | 1 | 12 | 20 | 3.86 | 2018-08-15 |
| s003 | Tasneem | CS | 1 | 8 | 18 | 3.57 | 2018-09-18 |
| s004 | Nahid | ECE | 2 | 7 | 16.5 | 3.25 | 2018-08-20 |
| s005 | Arafat | CS | 2 | 11 | 20 | 4.0 | 2018-09-13 |
| s006 | Tasneem | CSE | 1 | 12 | 17.5 | 3.7 | 2018-08-15 |
| s007 | Muhtadi | ECE | 1 | 10 | 19 | 3.67 | 2018-09-16 |

| CREATE DATABASE CSE370Lab02; |
| :---- |
| USE CSE370Lab02; |
| CREATE TABLE Lab\_Grades (      std\_id char(4),      name varchar(30),      major char(3),      section char(1),      days\_present int,      project\_marks double,      cgpa decimal(3,2),      submission\_date date ); |
| INSERT INTO Lab\_Grades values ('s001', 'Abir', 'CS', '1', 10, 18.5, 3.91, '2018-09-15'), ('s002', 'Nafis', 'CSE', '1', 12, 20, 3.86, '2018-08-15'), ('s003', 'Tasneem', 'CS', '1', 8, 18, 3.57, '2018-09-18'), ('s004', 'Nahid', 'ECE', '2', 7, 16.5, 3.25, '2018-08-20'), ('s005', 'Arafat', 'CS', '2', 11, 20, 4, '2018-09-13'), ('s006', 'Tasneem', 'CSE', '1', 12, 17.5, 3.7, '2018-08-15'), ('s007', 'Muhtadi', 'ECE', '1', 10, 19, 3.67, '2018-09-16'); |

