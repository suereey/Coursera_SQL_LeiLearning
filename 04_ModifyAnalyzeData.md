# Modifying and Analyzing Data with SQL

## Working with Text Strings
- Concatenations

    ![74](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/74_concatenations.png)

- trim

    ![75](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/75_trim.png)

- Substring

    ![76](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/76_substring.png)
    ![77](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/77_substring.png)

- Upper and Lower

    ![78](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/78.png)

## Working with Date and Time Strings
- data types for storing a date or a date/time value in the database:

    DATE - format YYYY-MM-DD
    DATETIME - format: YYYY-MM-DD HH:MI:SS
    TIMESTAMP - format: YYYY-MM-DD HH:MI:SS

    ![79](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/79_date.png)

- SQLite supoorted function

    ![80](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/80_date.png)

- Timestrings

    ![81](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/81_date.png)

- Modifiers: The time value can be followed by zero or more modifiers that alter date and/or time. Each modifier is a transformation that is applied to the time value to its left. Modifiers are applied from left to right; order is important. The available modifiers are as follows.

    ![82](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/82_modifier.png)

## Date and Time Strings Examples
- **STRFTIME**, Example:

    ![83](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/83_Example1.png)

- Compute current date
```
SELECT DATE('now');
```

- Compute year, month and day for the current date
```
SELECT STRFTIME('%Y %m %d', 'now');
```

- Compure hour, minute, second and milliseconds from curent datetime
```
SELECT STRFTIME('%H %M %S %s', 'now');
```

## Case Statements
- What is case statement

    ![84](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/84_casestatement.png)
    ![85](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/85_casestatement.png)

- Search case statement

    ![86](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/86_casestatement.png)

## Views
- Overview of Views
    - a stored query
    - can add or remove columns without changing schema
    - use it to encapsulate queries
    - the view will be removed after database coneections has ended

    ```
    CREATE [TEMP] VIEW [IF NOT EXISTS]
    viewname(column-name-list)
    AS
    select-statement
    ```

- Example

    ![87](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/87_views.png)
    ![88](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/88_views.png)
    ![89](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/89_views.png)

## Data Governance and Profiling
- what is data profiling 
    - Looking at descriptive statistics or object data information - examining data for completeness and accuracy

    - Important to understand your data before you query it

- Object data profile
    - number of rows
    - table size
    - when the object was last updated

- column data profile
    - column data type
    - number of discintct values
    - number of rows with NULL values
    - Descriptive statistics: maixmum, average and standard devaition for column values

- Governance best practices
    - understand your read and write capabilities
    - clean up your environments
    - understand your promotion process

## Using SQL for Data Science
- Data understanding
    - most impotrant step
    - understanding relationships in your data
    - NULL values
    - String values
    - Dates and times

- Subject area understanding 
    - until you gain business understanding, writing queries may take more time
    - understanding where data joins are
    - differentiating integers from strings
    - investing time to understand your subject will help later during data analysis

- Business understanding and Beware of the unspoken need

    ![90](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/90_.png)
    ![91](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/91_.png)

- Detail steps:

    ![92](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/92_.png)
    ![93](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/93_.png)
    ![94](https://raw.githubusercontent.com/suereey/Coursera_SQL_LeiLearning/main/screenshot/94_.png)
    ![95]()

    ![95]()

