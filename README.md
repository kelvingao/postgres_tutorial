# postgres_tutorial

## Installing PostgreSQL and Creating Your First Database

* Install Mac Version

    > [Mac Version Downloads](https://postgresapp.com/downloads.html)

    > [GUI](http://www.psequel.com/)

* Create First Database via Postgress Terminal

    > create a database
    ```SQL
    $ create database sample_db;
    ```

    >  List your database
    ```SQL
    $ \l
    ```
    > quit your database
    ```SQL
    $ \q
    ```
* Create a Table via Psequel
    > create a table
    ```SQL
    CREATE TABLE test_table (
        a INTEGER
    )
    ```