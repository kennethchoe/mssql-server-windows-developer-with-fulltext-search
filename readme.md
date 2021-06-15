Source: https://github.com/microsoft/mssql-docker/tree/master/windows/mssql-server-windows-developer

This docker image creates MS SQL Developer edition for Windows container with Full Text Search. 

To run, clone the repo and run the following:

```
docker build . -t kenny-sql
docker run --rm -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=yourStrong(!)Password' -p 1433:1433 -d kenny-sql
```

## References

https://stackoverflow.com/a/46101463/1459310

The fulltext search feature is not yet included in the docker image.

https://docs.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server-from-the-command-prompt?view=sql-server-ver15#sample-syntax

To install a new, stand-alone instance with the SQL Server Database Engine, Replication, and Full-Text Search components and enable instant file initialization for SQL Server Database Engine.
