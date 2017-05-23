# Dump a table schema only for create the table on another DB

`mysqldump` provides `--no-data`/`-d` option.

When `--no-data` is given, `mysqldump` print only show `CREATE` statement for the table.

```
$ mysqldump --no-data -u ${USER} -p${PASSWORD} ${DB_NAME} ${TABLE_NAME}
```

This is useful to create the table on another database.
