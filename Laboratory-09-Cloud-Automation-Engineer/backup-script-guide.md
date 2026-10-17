
# Backup Script Guide

## Overview

In this laboratory activity, I created an automated backup script using Bash. The script compresses a folder containing client data and saves it as a backup file with a timestamp.

## Bash Backup Script

The following Bash script was used:

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

## Executable Permissions

The following command was used:

```bash
chmod +x backup.sh
```

The `chmod +x` command adds executable permission to the backup script. Without this permission, running the script directly using `./backup.sh` may result in a "Permission denied" error.

## Executing the Backup Script

The script was executed using:

```bash
./backup.sh
```

The generated backups were verified using:

```bash
ls -l backups/
```

The script successfully created compressed `.tar.gz` backup files.

## Cron Job Configuration

The following Cron expression was used to schedule automated backups:

```cron
0 2 * * * /root/backup.sh
```

### Cron Schedule Explanation

- **Minute (0):** Runs at minute 0.
- **Hour (2):** Runs at 2:00 AM.
- **Day of Month (*):** Runs every day of the month.
- **Month (*):** Runs every month.
- **Day of Week (*):** Runs every day of the week.

This configuration schedules the backup script to run automatically every night at 2:00 AM according to the server's timezone.

## Conclusion

This activity helped me understand how Bash scripting and Cron can automate repetitive tasks such as backing up important files. Automation reduces the need for manual execution and helps ensure that backup operations follow a consistent schedule.
