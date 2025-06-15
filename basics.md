# Postgres Basics

### Basic commands
```js
Database exists:
\l

To switch database:
\c database_name

Table exists in database:
\d  d for describe and this show along with sequence
\dt this show without sequence

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

### Insert Data Into Table
```js
INSERT INTO table_name(
    column_name
)
VALUES('values')

Eg:
INSERT INTO person (
    first_name,
    last_name,
    gender,
    date_of_birth,
    email
)
VALUES('Leo', 'Das', 'male', date '1999-01-01', 'riyas@gmail.com');

```