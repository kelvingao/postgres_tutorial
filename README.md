# postgres_tutorial

## Retrieving Records from Your Database
   
* Retrive values
    ```SQL
    SELECT * FROM people;
    ```
* Specific columns
    ```SQL
    SELECT first_name, last_name FROM people;
    ``` 
* Conditional Query

    **OR** statement usage:
    ```SQL
    SELECT * FROM people
    WHERE last_name = 'Doe'
    OR last_name = 'Smith';
    ```

    **AND** statement usage:
    ```SQL
    SELECT * FROM people
    WHERE last_name = 'Doe'
    AND age < 30;
    ```

    **ORDER BY** statement usage (ASC order is the default):
    ```SQL
    SELECT * FROM people
    WHERE age < 36
    ORDER BY age DESC;
    ```
    order by serval columns

    ```SQL
    SELECT * FROM people
    WHERE age < 36
    ORDER BY first_name, last_name;
    ```