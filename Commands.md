
## Entity Framework
### 1. Creating database from code base, no db exists yet
Create model, then enable migration, no db created yet
```
PM> enable-migrations
```
Add initial migration class, no db created yet
```
PM> add-migration Initial
```
Creating database
```
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
### 2. Changing model and update database
Make changes to model, then run command
```
PM> add-migration <migration_name>
```
Update database after changing model
```
PM> update-database -verbose
```
