# Laboratory 09 - Cloud Automation Engineer

## Mission Overview

This laboratory focuses on Linux automation using Bash scripting and Cron Jobs. The task involves creating a backup script, making it executable, and scheduling it to run automatically.

## Objectives

- Understand Bash scripts and variables.
- Create an automated backup using a Bash script.
- Use `chmod +x` to make a script executable.
- Schedule tasks using Cron Jobs.
- Document the process and results in GitHub.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
./backup.sh
chmod +x backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

- Writing and executing Bash scripts.
- Creating compressed backup files using `tar`.
- Managing file permissions in Linux.
- Scheduling recurring tasks using Cron.
- Documenting technical work using Markdown and GitHub.

## Screenshots

- `screenshots/script-execution.png`
- `screenshots/cron-schedule.png`
