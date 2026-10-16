# Backup Script Guide

## 1. Backup Script

The `backup.sh` script automates the process of backing up the `app-data` directory. It creates a timestamped compressed archive inside the `backups` directory.

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

## 2. Making the Script Executable

The command `chmod +x backup.sh` gives the script permission to execute. Without this permission, running `./backup.sh` may return a `Permission denied` error.

## 3. Cron Job Configuration

The following Cron Job schedules the backup script to run every day at 2:00 AM.

```cron
0 2 * * * /root/backup.sh
```

### Cron Schedule Breakdown

- **Minute (`0`):** Runs at minute zero.
- **Hour (`2`):** Runs at 2 AM.
- **Day of Month (`*`):** Runs every day of the month.
- **Month (`*`):** Runs every month.
- **Day of Week (`*`):** Runs every day of the week.
- **Command (`/root/backup.sh`):** Executes the backup script.

## 4. Importance of Automation

Automated backups help reduce repetitive manual work and make backup routines more consistent. However, the script and schedule should be tested and monitored to ensure that backups are created correctly.
