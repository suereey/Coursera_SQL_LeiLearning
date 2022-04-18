# Filtering, Sorting and Calculating Data with SQL

## Basics of Filtering with SQL.
- WHERE
    - select for the matched one

    ![22](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/22_WHERE.png)
    ![23](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/23_WHERE.png)
    ![24](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/24_WHERE.png)

    - filter out a certain string

    ![25](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/25_WHERE.png)

    - select between a range

    ![26](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/26_WHERE.png)

    - select null

    ![27](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/27_WHERE.png)
    
## Advanced Filtering: IN, OR, and NOT
- IN Operator
    - Specifies a range of conditions
    - Comma delimited list of values
    - Enclosed in ()

    ![28](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/28_IN.png)

- OR Operator

    ![29](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/29_OR.png)

- OR with AND
    - sql process or before. use () to be safe
    ![30](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/30_ORAND.png)

- NOT Operator
    ![31](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/31_NOT.png)

## Using Wildcards in SQL
- using % wildcards:
    - % wildcard will not match NULLs
    - NULL represents no value in a column

    ![32](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/33_wildcards.png)
    ![33](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/34_wildcards.png)

- unsing underscore(_) wildcard:
    - matches a single charater
    - is not suported by DB2
    
    ![34]()

- using Bracket [] wildcard
    - used to specify a set of characters in a specific location
    - Does not work with all DBMS
    - Does not work with SQLite

- Downsides of wildcards

    ![35]()