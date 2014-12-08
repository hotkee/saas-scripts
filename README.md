Jamotion SaaS Scripts
=====================

docker-backup
-------------

This script is made for writing backups of customer containers and the productive database.

### Usage

    docker-backup -c [config file]
    
This command will read the given config file (or /etc/jamotion/backup.conf as default) and write the database and data backups into the folder /jamoshared/backup

