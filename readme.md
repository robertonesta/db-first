# Database Intro used car dealer;

## Data types:
- strings: [varchar(number), char(number), text, longtext]
- numbers: [tinyint, smallint, mediumint, int, bigint]
- decimals: [float(i,d), double(i,d), decimal(i,d)]
- dates: [datetime, date, time, year, timestamp]

## Attributes:
- NULL / NOT NULL
- DEFAULT(value)
- PRIMARY_KEY
- AUTO_INCREMENT
- UNIQUE

## Entity name: car

## Table name: cars

## Table Columns

-id             | BIGINT, PRIMARY_KEY, AUTO_INCREMENT, NOTNULL, UNIQUE, INDEX
-brand          | VARCHAR(30), NOTNULLABLE, INDEX
-model          | VARCHAR(50), NULLABLE,INDEX
-setup          | VARCHAR(30), NULLABLE
-fuel           | VARCHAR(30), NOTNULL
-width          | VARCHAR(10), NULLABLE
-length         | VARCHAR(10), NULLABLE
-height         | VARCHAR(10), NULLABLE
-year           | YEAR, NOTNULL, INDEX
-engine_size    | SMALLINT, NOTNULL
-horsepower     | SMALLINT | NOTNULL
-mileage        | NOTNULL, MEDIUMINT
-transmission   | VARCHAR(20) NOTNULL
-description    | TEXT, NULLABLE
-cover_image    | VARCHAR(150), NOTNULL
-price          | DECIMAL(8, 2)
-color          | VARCHAR(40), NOTNULL
-seats          | TINYINT, NOTNULL
-doors          | TINYINT, NOTNULL
-owners         | TINYINT, DEFAULT(1)
-car_state      | VARCHAR(30), NOTNULL
-is_available   | TINYINT, DEFAULT (0)
-emission       | CHAR(5), NULL
-optional       | TEXT, NULLABLE
-plate          | CHAR(7), NOTNULL, UNIQUE