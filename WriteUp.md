# DBFoundations-Module07
# Assignment 07

## Introduction
In this paper I will review the concept of an SQL User-defined functions, and the difference between scalar, inline, and multi-statement UDFs. I hope this review will help students and my peers to understand when and how to use SQL View and when a Function or a Stored Procedure is a better option. 

## When to use SQL UDF
User-defined functions (UDF) in SQL language are created by the user objects that can perform a requested operation based on accepted parameters. 
UDFs are useful to optimize coding work. Once created function can be repurposed/called multiple times. UDF, once created, is stored in the database and can be changed without impacting the program source code. User-defined function allows for fasted database querying, as function parameters don’t need to be built manually every single time. 

## Differences between Scalar, Inline, and Multi-Statement Functions
**Scalar functions** return a single data value of the type defined in the RETURNS clause. Scalar UDF accepts 0-to-many input parameter and returns one of the scalar data types: int, char, varchar, etc. Text, ntext, image, cursor, and timestamp are not supported.

**Inline function** returns a table-based result set. Result table values are results of the single SELECT statement. Because of that BEGIN/END block are not required to CREATE this function.  User doesn’t specify the structure of the called table. 

**Multi-statement function** returns a table-type result set. Result table value meet the requirements of the query included in the function. As user is creating a virtual table they have to declare all the variables for it. Multi-statement UDF use BEGIN/END syntax. This function can include one or a series of Transact-SQL statements that return the single value. The return type can be any data type except text, ntext, image, cursor, and timestamp. 

## Summary
Based on the video and reading materials provided for the sixth session of our course, I reviewed answers to questions on use of SQL UDFs. I presented differences between Scalar, Inline, and Multi-statement functions.  
