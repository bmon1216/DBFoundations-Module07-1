# More on Functions in Microsoft SQL Server

Steven Sparks  
March 3, 2021  
Foundations of Databases & SQL Programming  
Assignment 07  

## Introduction
This paper discusses using Functions in a relational database like Microsoft SQL Server.  SQL User-Defined Functions (“UDFs”) are routines that accept parameters, perform actions, and return the result as a value, just like Functions in other programming languages.  Scalar, Inline, and Multi-Statement Functions can return values as a single result or in tables, and each has some unique syntax.  

## When to Use a UDF in SQL
User-Defined Functions allow for more efficient programming, faster execution, and reduced network traffic than other Microsoft SQL Server features that yielding similar results.  
  
>**1.	Efficiency.**  Developers can create and store a UDF once, call it back an unlimited amount of times in the program, and modify the UDF independently of the database source code.  
  
>**2.	Speed.**  UDFs reduce the cost of compiling SQL code by parsing and optimizing the plans, then caching and using them for each repeated execution resulting in significantly faster execution times.  
  
>**3.	Reduced Traffic.**  Developers can express complex operations as a Function and then call them the Where clause to lessen the number of individual rows sent to the server client.  
  
(Microsoft website, <https://docs.microsoft.com/en-us/sql/relational-databases/user-defined-functions/user-defined-functions?view=sql-server-ver15> (external site), 2021.03.02).
