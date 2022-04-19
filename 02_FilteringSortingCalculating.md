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

    ![33](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/33_wildcards.png)
    ![34](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/34_wildcards.png)

- unsing underscore(_) wildcard:
    - matches a single charater
    - is not suported by DB2
    
    ![35](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/35_wildcards.png)

- using Bracket [] wildcard
    - used to specify a set of characters in a specific location
    - Does not work with all DBMS
    - Does not work with SQLite

- Downsides of wildcards

    ![36](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/36_wildcarddownside.png)

## Sorting with ORDER BY
- Why sorting

    ![37](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/37_sorting.png)

- Sorting by column poisiton

    ![38](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/38_sorting.png)

- Sorting direction
    - DESC descending order
    - ASC ascending order


## Math Operator
- Example

    ![39](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/39_mathoperator.png)
    ![40](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/40_mathoperator.png)

## Aggregate Functions
- AVG()

    ![41](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/41_aggregatefunc.png)

- COUNT()

    ![42](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/42_aggregatefunc_COUNT.png)

- MIN(), MAX()

    ![43](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/43_aggregatefunc_minmax.png)

- SUM()

    ![44](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/44_aggregatefunc_sum.png)


- **Distinct**


    ![45](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/45_distinct.png)

## Grouping Data with SQL

- Groupby example

    ![46](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/46_groupby.png)

- **Having clause** -filtering for groups
    - WHERE does not work for groups
    - WHERE filters on rows
    - Instead use HAVING clause to filter for groups

    ![47](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/47_groupby.png)

- WHERE vs. HAVING
    - WHERE filters before data is grouped
    - HAVING filters after data is grouped
    - Rows eliminated by the WHERE clause will not be included in the group

    ![48](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/48_groupby.png)

## Summary

![49](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/49_.png)