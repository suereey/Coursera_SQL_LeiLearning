# Subqueries and Joins in SQL

## Using Subqueries
- What is subqueries
    - Queries embedded into other queries
    - Relational databases store data in multiple table
    - Subqueries merge data from multiple sources togeter
    - Helps with adding other filtering criteria

- Example, subqueries to filter

    ![50](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/50_subquery.png)
    ![51](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/51_subquery.png)
    ![52](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/52_subquery.png)

- Working with Subquery Statements
    - Always perform the innermost SELECT portion first
    - DBMS is performing 2 operations
        - getting the order number for the product selected
        - adding that to the WHERE clause and processing the voerall SELECT statement

## Subquery Best Practices and Considerations
- Example of subquery in subquery. Use **Indent**

    ![53]()

- [PoorSQL Website](https://poorsql.com/)
    - helps pre-format code
    - helps proper indenting
    - makes code easier to read and troubleshoot

- Example subqueries for calculation

    ![54](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/54_subquery.png)

- The Power of subqueries
    - subqueries are powerfule tools
    - not always the best option due to performance

## Joining Tables: An Introduction
- Joins
    - associate the correct records from each table on the fly.
    - allow data retrieval from multiple tables in one query
    - joins are not physical - they persist for the duration of the query execution

    ![55](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/55_join.png)

## Cartesian (Cross) Joins
- what is cross join?
    - not frequently used
    - computationally taxing
    - will return products with the incorrect vendor or no vendor at all

    ![56](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/56_cartesian%20join.png)
    ![57](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/57_cartesian%20join.png)


## Inner Joins
- what is inner join?

    ![58](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/58_innerjoin.png)
    ![59](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/59_innerjoin.png)
    ![60](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/60_innerjoin.png)
    ![61](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/61_innerjoin.png)

- Best practices with joins
    - make sure youare pre-qualifying names
    - do not make unnecessary joins
    - think about the type of join you are making
    - how are you connecting records?

## Aliases and Self Joins
- what is alias

    ![62](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/62_alias.png)
    ![63](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/63_alias.png)

- Self Joins

    ![64](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/64_selfjoin.png)
    ![65](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/65_selfjoin.png)

## Advanced Joins: Left, Right, and Full Outer Joins
- SQL Lite vs. Other Sql DBMS
    - SQL Lite only does left joins
    - other database management systems use all joins

- Left Join, Right Join, Full Outer Join
    - differece between right and left is the order the tables are relating

    - left joins can be turned into right joins by reversing the order of the tables

    ![66](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/66_leftjoin.png)
    ![69](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/69_leftjoin.png)
    ![67](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/67_rightjoin.png)
    ![70](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/70_rightjoin.png)
    ![68](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/68_fulljoin.png)
    ![71](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/71_fulljoin.png)


## Unions
- What is union?
    - UNION is used to combine the results of two or more queries or table sets into one table and one statement.
    - Each select statement with UNION must have the same number of columns
    - Columns must have similar data types
    - The columnsin each SELECT statement must be in the same order

    ![72](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/72_union.png)

## Summary
- Best Practices using Joins
    - Check for duplicates
    - check the number of records each time you make a new join
    - are you getting the results you expected?
    - start small: one table at a time

- SQL joins diagram

    ![73](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/73_sqljoins.png)


## Others
- Recommend reading: 
[Difference Between Union and Union All - Optimal Performance Comparison](https://blog.sqlauthority.com/2009/03/11/sql-server-difference-between-union-vs-union-all-optimal-performance-comparison/)