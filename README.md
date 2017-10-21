# Explanation

This role is used to create cron jobs that use borg to backup the content of
docker volumes. Very useful in conjunction with wordpress or vpn role to replace
the crude tar based backups.

# Tags

* *borg_install*: install borg and sshfs and add ssh keys to borg repository
(it's a push backup for now)
* *borg_setup* add borg backup script and cron job
* *borg_restore* restore borg data to volumes using *borg_restore* list
* *borg_keys* only copy keys to destination host
* *borg_init* together with borg_install: create backup repository. Added mostly
  so we could skip it.
