For back up
COmmands

1. mongodump :> it will back up all the available databses in default dump folder

2. mongodump --db DATABASE_NAME ==> it will backup selected database in default dump folder

3. mongodump --db(-d) DATABASE_NAME --out(-o) PATH_TO_DESTINATION_FOLDER ==> it will backup the selected database in specific folder

RESTORE
Commands

1. mongorestore ==> it looks for default dump folder and restore all available database

2. mongorestore --drop ==> it looks fro defaule dump folder and restore all available database

3. mongorestre PATH_TO_SOURCE ==> It looks for backup for backup db in givern source folder

CSV AND JSON

JSON
BACKUP
mongoexport ==> mongoexport --db DB_NAME --collection COLLECTION_NAME --out PATH_TO_DESTINATION_WITH_JSON_EXTENSION
