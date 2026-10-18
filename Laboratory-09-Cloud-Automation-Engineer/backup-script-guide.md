# Backup Script Guide

## 1. Backup Script Code

The following Bash script compresses the application data into a timestamped `.tar.gz` backup file.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. File Permissions

The command `chmod +x backup.sh` gives the script executable permission. This allows Linux to run the script as a program using `./backup.sh` instead of treating it only as a text file.

## 3. Cron Job Configuration

The Cron expression used is:

```cron
0 2 * * * /root/backup.sh
```

This schedules the backup script to run every day at 2:00 AM.

### Cron Field Breakdown

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | Runs at minute zero. |
| Hour | `2` | Runs at 2:00 AM. |
| Day of Month | `*` | Runs every day of the month. |
| Month | `*` | Runs every month. |
| Day of Week | `*` | Runs every day of the week. |

## 4. Verification

The command `./backup.sh` was used to execute the script manually. The command `ls -l backups/` was used to verify that a compressed backup file was created. The command `crontab -l` was used to check the installed Cron schedule.
