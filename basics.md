# Postgres Basics

### Basic commands
```js
Database exists:
\l

To switch database:
\c database_name

Table exists in database:
\d  d for describe

To view particular table:
\d table_name

To clear screen:
\! cls
```

### Create Table
```js

CREATE TABLE table_name (
    column_name + data_type + constrains [if needed]
)

Creating table without constrains:
CREATE TABLE person (
    id INT,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    gender VARCHAR(7),
    date_of_birth DATE
    );


Creating table with constrains:

CREATE TABLE person (
    id BIGSERIAL NOT NULL PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    gender VARCHAR(7) NOT NULL,
    date_of_birth DATE NOT NULL
    );

```

### Drop Database & Table
```js
DROP DATABASE database_name;

DROP TABLE table_name;
```

