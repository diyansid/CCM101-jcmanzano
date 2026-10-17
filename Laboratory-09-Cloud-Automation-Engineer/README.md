
# Laboratory 09 - Cloud Automation Engineer

## Mission Overview

This laboratory activity focused on automating routine cloud operations using Bash scripting and Linux Cron. The mission involved creating a backup script, modifying file permissions, testing the backup process, and scheduling automatic backups.

## Objectives

- Understand the basic syntax of Bash scripts.
- Learn how variables are used in automation.
- Create an automated backup script.
- Modify executable permissions using chmod.
- Compress directories into `.tar.gz` files.
- Configure scheduled tasks using Cron.
- Document automation processes using Markdown.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt

nano backup.sh
./backup.sh
chmod +x backup.sh
./backup.sh

ls -l backups/

crontab -l
env EDITOR=nano crontab -e
crontab -l
```

## Skills Learned

- Writing and executing Bash scripts.
- Using variables for file paths and timestamps.
- Creating compressed backups automatically.
- Managing Linux file permissions.
- Scheduling automated tasks using Cron.
- Understanding Cron expressions and time fields.
- Using Linux terminal commands for automation.
- Documenting cloud automation procedures.
