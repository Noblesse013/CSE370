**Department of Computer Science and Engineering**

| Course Code: CSE 370 | Credits: 3.0 |
| :---- | ----: |
| **Course Name: Database Systems** | **Semester: Fall 2024** |

**Lab Assignment 1**

Soon after joining Google’s elite dev team, Area 120, you were assigned to a project using MySQL since it was your specialty. The project was a social media platform specialized in allowing developers from all over the globe to connect to each other, and it would have features similar to Facebook. For your first task, you have been assigned to work on the tables of one of the project databases. 

You will use a database called **Google\_\<Your8DigitStudentID\>.**

| Format: CREATE DATABASE Google\_\<Your8DigitStudentID\>; CREATE DATABASE Google\_12345678; |
| :---- |
| **USE** Google\_12345678; |

The table name is **"Developers"** which is shown below. 

| member\_id | name | email | influence\_count | Joining\_date | multiplier |
| :---: | :---: | :---: | :---: | :---: | :---: |
| 1 | Taylor Otwell | otwell@laravel.com | 739360 | 2020-6-10 | 10 |
| 2 | Ryan Dahl | ryan@nodejs.org | 633632 | 2020-04-22 | 10 |
| 3 | Brendan Eich | eich@javascript.com | 939570 | 2020-05-07 | 8 |
| 4 | Evan You | you@vuejs.org | 982630 | 2020-06-11 | 7 |
| 5 | Rasmus Lerdorf | lerdorf@php.net | 937927 | 2020-06-3 | 8 |
| 6 | Guido van Rossum | guido@python.org | 968827 | 2020-07-18 | 19 |
| 7 | Adrian Holovaty | adrian@djangoproject.com | 570724 | 2020-05-07 | 5 |
| 8 | Simon Willison | simon@djangoproject.com | 864615 | 2020-04-30 | 4 |
| 9 | James Gosling | james@java.com | 719491 | 2020-05-18 | 5 |
| 10 | Rod Johnson | rod@spring.io | 601744 | 2020-05-18 | 7 |
| 11 | Satoshi Nakamoto | nakamoto@blockchain.com | 630488 | 2020-05-10 | 10 |

Write the queries of the tasks given below \[6 \* 2 \= 12\]. 

1\. Create the above table with the appropriate data type for each column.

2\. Change the column name "influence\_count". The new name should be "followers," and the data type should be integer. 

3\. Update the number of followers of each developer by \+10.

4\. There is a formula to find the efficiency of the developers. Efficiency \= ((followers\*100/1000000) \* (multipliers\*100/20))/100. Show the efficiency of each developer in a column named "Efficiency" along with their name.

5\. Show the name of the developers in UpperCase and the descending order of their Joining\_date.   

6\. Retrieve the member\_ id, name, email and followers of the developers who have either ".com" or ".net" in their email address. 

   

