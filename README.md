# postgres_tutorial

## Modifying and Removing Records from Your Database
   
* **UPDATE** all the records
    ```SQL
    UPDATE test_table
    SET location = 'Unknown';
    ```
* **DELETE** all the recores
    ```SQL
    DELETE FROM test_table
    ```
* **UPDATE** specific records
    
    before update, you should make a CHECK query
    ```SQL
    SELECT * FROM people
    WHERE first_name = 'John'
    AND last_name = 'Smith';
    ```
    and, then update
    ```SQL
    UPDATE people
    SET occupation = 'Programmer'
    WHERE first_name = 'John'
    AND last_name = 'Smith';
    ```

    delete records
    ```SQL
    DELETE FROM people
    WHERE occupation = 'Scientist'
    AND age < 58; 
    ```