# Database

PostgreSQL 9.6 with PostGIS 2.x is expected.

## Schemas

- **src_ruian** holds the source data coming from RUIAN
- **api_monitor** holds the stats coming from quarterly land use statistics published by CUZK

## Running migrations

Database versioning is done solely via liquibase, no direct modifications of database structures are expected.

Make sure the database `cadastre` with the user `c_install` and the schema `c_install` exists before running migration scripts.

### Initial run

Run migrations inside `database` folder first, followed by others.
