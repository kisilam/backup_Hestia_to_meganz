# Backup_Hestia_to_meganz

Copy Heastia backup file to a Mega.nz one time at the week 
1. Need to create container which will be use to copy files to remote folder
   docker pull megacmd-ubuntu:18.04
   docker run --name=meganz -ti -v /backup:/backup megacmd-ubuntu:18.04  /bin/bash
   exit
   docker stop meganz
3. Put the script in /etc/cron.weekly
