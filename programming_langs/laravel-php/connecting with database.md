---
tags: mysql, database, laravel
---

# connecting with MySQL database

## in `.env`

> set the following lines

- DB_CONNECTION
    - > type of database
- DB_HOST
    - > URL to server hosting the database
- DB_PORT
    - > port on which the database is served
- DB_DATABASE
    - > name of the database
- DB_USERNAME
- DB_PASSWORD

## making the connection

run

```shell
php artisan migrate
```
