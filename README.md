# busdb

Back up sqlite3 database.

A backup shell script for sqlite3 database.

----
### Prerequisites

Bash version 4+, sqlite3 and the following tools.

* file
* mkdir

----
### Installing

Put the busdb script somewhere in your PATH.

----
### Example
```shell
 -f /path/to/the/database/mydatabase -d /path/to/the/directory/whereto/backup/
```
```shell
 --file /path/to/the/database/mydatabase --directory /path/to/the/directory/whereto/backup/
```
```shell
 --file=/path/to/the/database/mydatabase --directory=/path/to/the/directory/whereto/backup/
```

----
### AUTOMATED BACKUP
Using cron:

```cron
0 * * * * "$HOME/bin/busdb" -f "$HOME/.bash_history.sqlite" -d /Data
```

The script is in "$HOME/bin"

The database is "$HOME/.bash_history.sqlite"

The destination/directory is /Data

This runs every hour on openSUSE, consult the documentation of your cron see **man 5 crontab**

----
## Author

* **Jason V. Ferrer** - [Jetchisel](https://github.com/Jetchisel)
