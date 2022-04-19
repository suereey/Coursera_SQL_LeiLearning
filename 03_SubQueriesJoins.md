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

    ![54]()

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

    ![58]()
    ![59]()
    ![60]()
    ![61]()

- Best practices with joins
    - make sure youare pre-qualifying names
    - do not make unnecessary joins
    - think about the type of join you are making
    - how are you connecting records?

## Aliases and Self Joins
- what is alias

    ![62]()
    ![63]()

- Self Joins

    ![64]()
    ![65]()

## Advanced Joins: Left, Right, and Full Outer Joins
- SQL Lite vs. Other Sql DBMS
    - SQL Lite only does left joins
    - other database management systems use all joins

## Unions