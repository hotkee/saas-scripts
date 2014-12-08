Jamotion SaaS Scripts
=====================

docker-backup
-------------

This script is made for creating backups of customer containers and their productive databases. The script will create two files per customer:
- `<dbname>_<timestamp>.dump` The database dump
- `<dbname>_<timestamp>.tar`  The customer specific odoo files.

### Usage

#### Running backup manually for a single customer container and database

    docker-backup <customer> <database>
    
This command will create the backup files for only one data container and one database.

#### Running backup based on a config file

    docker-backup -c [config file]
    
This command will read the given config file (or `/etc/jamotion/backup.conf` as default) and write the database and data backups into the folder `/jamoshared/backup`.

### Todo

- Allowing to define the target path directly in config file (with regions like `[options]` and `[customers]`.

