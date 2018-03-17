


### Drop table with IF EXISTS

for backwards compatibility with all versions of sql-server, use this:

```sql
IF OBJECT_ID('dbo.emplocations') IS NOT NULL
DROP TABLE dbo.emplocations;
```

----

