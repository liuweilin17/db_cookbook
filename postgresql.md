PostgreSQL

Here is the [official website](https://www.postgresql.org/)

Here is the [v12 documentation](https://www.postgresql.org/docs/12/index.html)

1. Install

   In Mac:

   ``` 
   brew install postgresql
   ```

   

2. Starting the Database server

```postgres``` is the database server program. The ```postgres``` program know where to find the data it is supposed to use with ```-D``` option.

```
postgres -D /usr/local/pgsql/data
```

Apart from ```postgres``` , ```pg_ctl``` is a wrapper program to initialize, start, stop, or control a PostgreSQL server.

start server in Mac:

```
pg_ctl -D /usr/local/var/postgres start
```

stop server in Mac:

```
pg_ctl -D /usr/local/var/postgres stop
```

3. connect database

   ``` psql``` is the interactive terminal for working with Postgres.

   connect to the default database ```postgres```:

   ```
   psql postgres
   ```
   
   In ```psql``` terminal, there are some frequently used commands:
   
   ```\l```: get a list of all available databases
   
   ```\dt```: listing the available tables in the current database
   
   ```\c <database_name>```: switching to another database
   
   ```\d <table_name>```: describe  a particular table
   
   ```SELECT version();```: find the version of PostgreSQL
   
   ```\e```: `psql` + text editor
   
   
   
   

