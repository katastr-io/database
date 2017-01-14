# Database

PostgreSQL 9.6 with PostGIS 2.x is expected.

## Schemas

- **src_ruian** holds the source data coming from RUIAN
- **api_monitor** holds the stats coming from quarterly land use statistics published by CUZK

## Running migrations

Database versioning is done solely via liquibase, no direct modifications of database structures are expected.

Make sure the following already exists when running migrations:

- `katastriospace` tablespace
- `katastrio` database
- `katastrio` user
- `katastrio` schema

### Initial run

Run migrations inside the `database` folder first, followed by others.

Note that the user needs to be superuser to run migrations inside the `database` folder.

## Deployment

Changes are deployed with codeship, but **not applied automatically.**
