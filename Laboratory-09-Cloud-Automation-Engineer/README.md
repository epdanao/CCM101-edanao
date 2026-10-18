# Laboratory 09 – Cloud Automation Engineer

## Mission Overview

This laboratory focuses on automating application data backups using Bash scripting and the Linux Cron scheduler in the KillerCoda Ubuntu Playground. The goal is to reduce manual work and help protect important client data.

## Objectives

- Understand the basics of Bash scripting.
- Create a dummy application directory and test file.
- Write and execute an automated backup script.
- Use `chmod +x` to grant executable permission.
- Verify the generated compressed backup file.
- Configure a Cron job to run the backup every day at 2:00 AM.
- Document the implementation and results.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

- **Bash scripting:** Writing commands to automate repetitive tasks.
- **Variables:** Storing directory paths and timestamps for reuse.
- **Linux permissions:** Using `chmod +x` to make a script executable.
- **Backup management:** Compressing application data into `.tar.gz` archives.
- **Cron scheduling:** Configuring automated tasks to run at a specified time.
- **Technical documentation:** Recording code, commands, configurations, and verification results in Markdown.
