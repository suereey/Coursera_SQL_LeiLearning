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


## 