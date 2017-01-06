
## Entity Framework
### 1. Creating database from code base, no db exists yet
```
PM> enable-migrations
...
PM> add-migration Initial
...
PM> update-database
```
or display SQL statements applied to DB while updating it.
```
PM> update-database -Verbose 
```
or create script for running in sql, no changes applied to db in this case
```
PM> update-database -script
```

